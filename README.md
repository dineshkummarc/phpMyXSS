phpMyXSS
========
A XSS Project

### AUTHOR
[zeng.ambulong@gmail.com](mailto:zeng.ambulong@gmail.com)

### RELEASE INFORMATION
*phpMyXSS 1.0*

### Demo
Project Management
![Project Management](https://github.com/dineshkummarc/phpMyXSS/blob/master/doc/project-management.png)
Add Project
![Add Project](https://github.com/dineshkummarc/phpMyXSS/blob/master/doc/add-project.png)
Host Management
![Host Management](https://github.com/dineshkummarc/phpMyXSS/blob/master/doc/host-management.png)
Module Management
![Module Management](https://github.com/dineshkummarc/phpMyXSS/blob/master/doc/module-management.png)

### SYSTEM REQUIREMENTS
PHP 5.3.9 or later; we recommend using the
latest PHP version whenever possible.

### INSTALLATION

Import the file `./phpmyxss.sql` to your MySQL database

Config the php file `./config.php`
```php
/** The username for phpMyXSS */
define ( 'PMX_USERNAME', 'root' );
/**
 * The password(phpass) for phpMyXSS
 */
define ( 'PMX_PASSWORD', '' );
```

If you want to use 'new message alert', you need to config PHPMailer in file `./includes/functions.php` at pmx_mail(...)

###Reporting Potential Security Issues

If you have encountered a potential security vulnerability in this project, please report it to us at [zeng.ambulong@gmail.com](mailto:zeng.ambulong@gmail.com). We will work with you to verify the vulnerability and patch it.

###common problem

1. Installation related
    Import phpmyxss.sql into the database and modify the database connection information in ./config.php
    PMX does not support multi-user support at the moment. If you need to change the user name and password, you need to modify it in config.php (default 123456). Please generate the password (PMX_PASSWORD) by yourself with phpass, or generate it with genpass.php in the directory.
    Email reminder, please go to ./includes/functions.php to modify the configuration in the function pmx_mail()
   
2. To understand the project, you can read pages 1 to 2 of the document in the doc

3. Project screenshots are also available behind the doc

4. If you have other questions or suggestions, you can send an email to ask

###Update

    September 25, 2016
       1. Fix infinite redirection problem
       2. Add a script to generate phpass password, genpass.php

###Want to contribute?

Fork us!

### LICENSE

This software is licenced under the [GPL 2.0](http://www.gnu.org/licenses/gpl-2.0.html). Please read LICENSE for information on the
software availability and distrib
