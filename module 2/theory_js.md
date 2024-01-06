W3-Schools


### javascript functions
```bash
<script>
function myFunction(p1, p2) {
  return p1 * p2;
}

let result = myFunction(4, 3);
document.getElementById("demo").innerHTML = result;
</script>
```
- A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses ().
- Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).
- The parentheses may include parameter names separated by commas: (parameter1, parameter2, ...)
- The code to be executed, by the function, is placed inside curly brackets: {}


```bash
// Define a function named test_prime that checks whether a given number n is a prime number
function test_prime(n) {

  // Check if the number is equal to 1, which is not a prime number
  if (n === 1) {
    return false;
  }
  // Check if the number is equal to 2, which is a prime number
  else if (n === 2) {
    return true;
  } else {
    // Iterate from 2 to n-1 to check for factors of n
    for (var x = 2; x < n; x++) {
      // If n is divisible by x without a remainder, it is not a prime number
      if (n % x === 0) {
        return false;
      }
    }
    // If no factors are found, the number is a prime number
    return true;  
  }
}

// Log the result of calling test_prime with the input number 37 to the console
console.log(test_prime(37));
```
### javascript arrays
initialisation 
```bash
//direct declaration of values
const cars = ["mercedes", "nissan", "BMW"];

//empty array then adding values
const cars = [];
cars[0]= "Saab";
cars[1]= "Volvo";
cars[2]= "BMW";

//using new keyword
const cars = new Array("mercedes", "mclaren", "BMW");

//using new Array()
const points = new Array();
const points = new Array(40, 100, 1, 5, 25, 10);
```

accessing elements

```bash
//using index number
const cars = ["suzuki", "honda", "BMW"];
let car = cars[0];

//changing a value

const cars = ["mercedes", "skoda", "BMW"];
cars[0] = "hyundai";

//length
const fruits = ["Banana", "Orange", "Apple", "Mango"];
let length = fruits.length;

//looping through array
const fruits = ["Banana", "Orange", "Apple", "Mango"];
let text = "<ul>";
fruits.forEach(myFunction);
text += "</ul>";

function myFunction(value) {
  text += "<li>" + value + "</li>";
}
```

### Associative arrays
- Arrays with named indexes are called associative arrays (or hashes).
- JavaScript does not support arrays with named indexes.
- In JavaScript, arrays always use numbered indexes.

- 
```bash
const person = [];
person[0] = "John";
person[1] = "Doe";
person[2] = 46;
person.length;    // Will return 3
person[0];        // Will return "John"

```
