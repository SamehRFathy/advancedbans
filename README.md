# ab-web-addon
A simple, but sleek, web addon for AdvancedBan.
- You can find the example [here](https://whatisin.space/ab-web-addon).

## Using the Addon
To use the AdvancedBan web addon, you must first upload all PHP pages to your site.
The database.php file is the only file that requires editing.
```php
$con = mysqli_connect("host","username","password","database"); //Enter your MYSQL details here.

$info = array(
	'title'=>'AdvancedBan Web Addon', //This will be displayed in the title, main jumbotron, and navigation bar.
	'description'=>'A simple, but sleek, web addon for AdvancedBan.', //This will be displayed under the title on all pages.
	'table'=>'PunishmentHistory'); //The table of your MYSQL database for which punishments are saved.

if (mysqli_connect_errno()) {
	die('Failed to connect to database.');
}
```
Once you have correctly entered in your database details and table name, the addon should start working.
## Credit and Problems
The site theme and framework are by Bootswatch and Bootstrap.
The addon itself by [mathhulk](https://theartex.net).
All credit for AdvancedBan goes to its original author, whose link can be found on the example page.
## Issues
- Weird database loop not returning all rows
