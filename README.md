# Android-Login-And-Registration
Android Login And Registration System with PHP, MySQL and SQLite Databases.

Read Full tutorial
[Develop a Complete Android Login Registration System with PHP, MySQL](https://www.androidlearning.com/android-login-registration-with-php-mysql-sqlite/)

## Download Android Learning Application
<a href="https://play.google.com/store/apps/details?id=snow.androidlearning.app">
<img src="https://play.google.com/intl/en_us/badges/images/badge_new.png" title="Android Learning App" target="_blank"/></a>

## Login Screen
<a href="https://github.com/akrajilwar/Android-Login-And-Registration/blob/master/project_2_login_screen.png">
<img src="https://github.com/akrajilwar/Android-Login-And-Registration/blob/master/project_2_login_screen.png" height="640px" /></a>

## Registration Screen
<a href="https://github.com/akrajilwar/Android-Login-And-Registration/blob/master/project_2_registration_screen.png">
<img src="https://github.com/akrajilwar/Android-Login-And-Registration/blob/master/project_2_registration_screen.png" height="640px" /></a>

## Email Verify Screen
<a href="https://github.com/akrajilwar/Android-Login-And-Registration/blob/master/project_2_email_verify_screen.png">
<img src="https://github.com/akrajilwar/Android-Login-And-Registration/blob/master/project_2_email_verify_screen.png" height="640px" /></a>

## Home Screen
<a href="https://github.com/akrajilwar/Android-Login-And-Registration/blob/master/project_2_home_screen.png">
<img src="https://github.com/akrajilwar/Android-Login-And-Registration/blob/master/project_2_home_screen.png" height="640px" /></a>


## Steps for WINDOWS ON XAMPP
  - Git clone this Repository
  - Copy android_login folder to XAMPP=>htdocs
  - Create database android_login =>

         CREATE TABLE `users` (`id` int(11) NOT NULL, `unique_id` varchar(23) NOT NULL, `name` varchar(50) NOT NULL, `email` varchar(100) NOT NULL, `encrypted_password` varchar(250) NOT NULL, `otp` int(6) NOT NULL, `verified` int(1) NOT NULL, `created_at` datetime NOT NULL) ENGINE=MyISAM DEFAULT CHARSET=latin1 COLLATE=latin1_swedish_ci;

  - Change Config.php file for username and password
      
      $username = "root"; 
      $password = "pass"; 
      $host = "localhost"; 
      $dbname = "android_login"; 

  - Change Main Url inside Functions.Java File 
  - If you are using localhost:[PORT] change Mainurl to MAIN_URL = "http://10.0.2.2:[PORT]/android_login/"
  - If you are using just localhost change Mainurl to MAIN_URL = "http://10.0.2.2/android_login/"

## Steps for WEBHOSTING
  - Git clone this Repository
  - Copy android_login folder to cpanel=>www
  - Create database android_login =>
  
        CREATE TABLE `users` (`id` int(11) NOT NULL, `unique_id` varchar(23) NOT NULL, `name` varchar(50) NOT NULL, `email` varchar(100) NOT NULL, `encrypted_password` varchar(250) NOT NULL, `otp` int(6) NOT NULL, `verified` int(1) NOT NULL, `created_at` datetime NOT NULL) ENGINE=MyISAM DEFAULT CHARSET=latin1 COLLATE=latin1_swedish_ci;
    
  - Change Config.php file for username and password
      $username = "username"; 
      $password = "pass"; 
      $host = "localhost"; 
      $dbname = "username_android_login"; //Check at phpmyadmin whats the name of database
      
  - Change Main Url inside Functions.Java File // HTTP[S] not HTTP TRY BOTH
  - Change Mainurl to MAIN_URL = "https://hostname.example.com/username_android_login/" example "https://cpanel.example.com/username_android_login/"
