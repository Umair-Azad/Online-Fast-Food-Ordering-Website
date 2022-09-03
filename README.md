# Online-Fast-Food-Ordering-Website

                   FOLLOW BELLOW STEPS TO RUN THIS PROJECT

 1) Download all files.
 
 2) Move this project to Root Directory
Local Disc C: -> xampp -> htdocs -> 'this project'
Local Disk C is the location where xampp was installed

 3) Open XAMPP Control Panel and Start 'Apache' and 'MySQL'


 4) Import Database

 a. Open 'phpmyadmin' in your browser
 b. Create a Database  
 c. Import the SQL file provided with this project


 4) Make Changes to settings
 Go to 'config' folder and Open 'constants.php' file. Then make changes in DB_USERNAME,DB_PASSWORD and DB_NAME.

<?php 
//Start Session
session_start();

//Create Constants to Store Non Repeating Values
define('SITEURL', 'http://localhost/Codes/'); //Update the home URL of the project if you have changed port number or it's live on server
define('LOCALHOST', 'localhost');
define('DB_USERNAME', 'root');
define('DB_PASSWORD', '');
define('DB_NAME', 'food_order');
    
$conn = mysqli_connect(LOCALHOST, DB_USERNAME, DB_PASSWORD) or die(mysqli_error()); //Database Connection
$db_select = mysqli_select_db($conn, DB_NAME) or die(mysqli_error()); //SElecting Database 

?>

 5) Now, Open the project in your browser. It should run perfectly.
