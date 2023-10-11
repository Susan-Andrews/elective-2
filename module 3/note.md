## Intro

`Use w3 php server :` [w3 ](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_syntax )
- PHP is an acronym for "PHP: Hypertext Preprocessor"
- PHP is a widely-used, open source scripting language
- PHP scripts are executed on the server
- PHP is free to download and use 
- PHP files can contain text, HTML, CSS, JavaScript, and PHP code
- PHP code is executed on the server, and the result is returned to the browser as plain HTML
- PHP files have extension ".php" 
- PHP can generate dynamic page content
- PHP can create, open, read, write, delete, and close files on the server
- PHP can collect form data
- PHP can send and receive cookies
- PHP can add, delete, modify data in your database
- PHP can be used to control user-access
- PHP can encrypt data
- A PHP script can be placed anywhere in the document.
- A PHP script starts with <?php and ends with ?>

##### Syntax

```php
<?php
// PHP code goes here
?>
```
##### Echo/Print 

- The default file extension for PHP files is ".php". A PHP file normally contains HTML tags, and some PHP scripting code. PHP script that uses a built-in PHP function `"echo"` to output the text 

```php
<!DOCTYPE html>
<html>
<body>
<h1>My first PHP page</h1>
<?php
echo "Hello World!";
?>
</body>
</html>
```
##### Variables 

- In PHP, a variable starts with the $ sign, followed by the name of the variable 
- The PHP echo statement is often used to output data to the screen.

```bash 
<?php
$txt = "Hello world!";
$x = 5;
$y = 10.5;
?>
```
##### Sum of two numbers  

```php 
<?php
$x = 5;
$y = 4;
echo $x + $y;
?> 
```
##### Global keyword  

- The global keyword is used to access a global variable from within a function.To do this, use the global keyword before the variables (inside the function) 

```php
<?php
$x = 5;
$y = 10;

function myTest() {
  global $x, $y;
  $y = $x + $y;
}

myTest();
echo $y; // outputs 15
?>

```
##### Sum of numbers using function  

```php 
<?php
// Function to add two numbers
function addNumbers($num1, $num2) {
    $sum = $num1 + $num2;
    return $sum;
}

// Input numbers
$number1 = 5;
$number2 = 7;

// Call the function and store the result in a variable
$result = addNumbers($number1, $number2);

// Display the result
echo "The sum of $number1 and $number2 is: $result";
?>

```