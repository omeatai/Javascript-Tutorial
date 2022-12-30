# Javascript-Tutorial

Learn Javascript by Ifeanyi Omeata

## Tutorial

---

### [1-JAVASCRIPT COURSE - W3SCHOOLS](#)

+ARRAYS

<details>
  <summary>1. Creating an Array</summary>

Arrays are a special kind of objects, with numbered indexes. <br>
Arrays use numbered indexes, while objects use named indexes.<br>

```js
const cars = ["Saab", "Volvo", "BMW"];
```

```js
const cars = new Array("Saab", "Volvo", "BMW");
```

```js
// [Saab,Volvo,BMW]
```

</details>

<details>
  <summary>2. Assign Values to Array</summary>

```js
const cars = [];
cars[0] = "Saab";
cars[1] = "Volvo";
cars[2] = "BMW";
```

```js
// [Saab,Volvo,BMW]
```

</details>

<details>
  <summary>3. Accessing Array Elements</summary>

```js
const cars = ["Saab", "Volvo", "BMW"];
let car = cars[0];
```

```js
// Saab
```

</details>

<details>
  <summary>4. Changing an Array Element</summary>

```js
const cars = ["Saab", "Volvo", "BMW"];
cars[0] = "Opel";
```

```js
// [Opel,Volvo,BMW]
```

</details>

+ARRAY PROPERTIES AND METHODS

<details>
  <summary>5. Array Length</summary>

```js
const fruits = ["Banana", "Orange", "Apple", "Mango"];
let length = fruits.length;
```

Accessing the First Array Element:

```js
const fruits = ["Banana", "Orange", "Apple", "Mango"];
let fruit = fruits[0];
```

Accessing the Last Array Element:

```js
const fruits = ["Banana", "Orange", "Apple", "Mango"];
let fruit = fruits[fruits.length - 1];
```

</details>

<details>
  <summary>6. Looping Array Elements with For Loop</summary>

```js
const fruits = ["Banana", "Orange", "Apple", "Mango"];
let fLen = fruits.length;

let text = "<ul>";
for (let i = 0; i < fLen; i++) {
  text += "<li>" + fruits[i] + "</li>";
}
text += "</ul>";
```

```js
// Banana
// Orange
// Apple
// Mango
```

</details>

<details>
  <summary>7. Looping Array Elements with For Each Loop</summary>

```js
const fruits = ["Banana", "Orange", "Apple", "Mango"];
let fLen = fruits.length;

let text = "<ul>";
for (let i = 0; i < fLen; i++) {
  text += "<li>" + fruits[i] + "</li>";
}
text += "</ul>";
```

```js
// Banana
// Orange
// Apple
// Mango
```

</details>

<details>
  <summary>8. Array push()</summary>

The push() method adds a new element to an array (at the end).<br>
The push() method returns the new array length.<br>

```js
const fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo1").innerHTML = fruits.push("Kiwi");
document.getElementById("demo2").innerHTML = fruits;
```

```js
// 5
// Banana,Orange,Apple,Mango,Kiwi
```

```js
const fruits = ["Banana", "Orange", "Apple"];
fruits[fruits.length] = "Lemon"; // Adds "Lemon" to fruits
```

```js
// [Banana,Orange,Apple,Lemon]
```

</details>

<details>
  <summary>9. Array pop()</summary>

The pop() method removes the last element from an array.<br>
The pop() method returns the value that was "popped out".<br>

```js
const fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo1").innerHTML = fruits.pop();
document.getElementById("demo2").innerHTML = fruits;
```

```js
// Mango
// Banana,Orange,Apple
```

</details>

<details>
  <summary>10. Array shift()</summary>

The shift() method removes the first array element and "shifts" all other elements to a lower index.<br> Shifting is equivalent to popping, but working on the first element instead of the last.<br>
The shift() method returns the value that was "shifted out".<br>

```js
const fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo1").innerHTML = fruits.shift();
document.getElementById("demo2").innerHTML = fruits;
```

```js
// Banana
// Orange,Apple,Mango
```

</details>

<details>
  <summary>11. Array unshift()</summary>

The unshift() method adds a new element to an array (at the beginning), and "unshifts" older elements.<br>
The unshift() method returns the new array length.<br>

```js
const fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo1").innerHTML = fruits.unshift("Lemon");
document.getElementById("demo2").innerHTML = fruits;
```

```js
// 5
// Lemon,Banana,Orange,Apple,Mango
```

</details>

<details>
  <summary>12. Array isArray() and instanceof</summary>

The isArray Method returns true if an object is an Array:

```js
const fruits = ["Banana", "Orange", "Apple"];
Array.isArray(fruits);
```

```js
// true
```

The instanceof operator returns true if an object is created by a given constructor:

```js
const fruits = ["Banana", "Orange", "Apple"];

fruits instanceof Array;
```

```js
// true
```

</details>

<details>
  <summary>13. Array toString()</summary>

The JavaScript method toString() converts an array to a string of (comma separated) array values.

```js
const fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo").innerHTML = fruits.toString();
```

```js
// Banana,Orange,Apple,Mango
```

</details>

<details>
  <summary>14. Array join()</summary>
The join() method also joins all array elements into a string. <br>
It behaves just like toString(), but in addition you can specify the separator.<br>

```js
const fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo").innerHTML = fruits.join(" * ");
```

```js
// Banana * Orange * Apple * Mango
```

</details>

<details>
  <summary>15. Array concat()</summary>

The concat() method creates a new array by merging (concatenating) existing arrays.<br>
The concat() method can take any number of array arguments.<br>

```js
const myGirls = ["Cecilie", "Lone"];
const myBoys = ["Emil", "Tobias", "Linus"];
const myChildren = myGirls.concat(myBoys);
```

```js
// [Cecilie,Lone,Emil,Tobias,Linus]
```

```js
const arr1 = ["Cecilie", "Lone"];
const arr2 = ["Emil", "Tobias", "Linus"];
const arr3 = ["Robin", "Morgan"];
const myChildren = arr1.concat(arr2, arr3);
```

```js
// [Cecilie,Lone,Emil,Tobias,Linus,Robin,Morgan]
```

```js
const arr1 = ["Emil", "Tobias", "Linus"];
const myChildren = arr1.concat("Peter");
```

```js
// [Emil,Tobias,Linus,Peter]
```

</details>

<details>
  <summary>16. Array splice()</summary>

The splice() method adds new items to an array. <br>
The first parameter (2) defines the position where new elements should be added (spliced in). <br>
The second parameter (0) defines how many elements should be removed.<br>
The rest of the parameters ("Lemon" , "Kiwi") define the new elements to be added.<br>
The splice() method returns an array with the deleted items.<br>

```js
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.splice(2, 0, "Lemon", "Kiwi");
```

```js
// Banana,Orange,Lemon,Kiwi,Apple,Mango
```

```js
const fruits = ["Banana", "Orange", "Apple", "Mango"];
let removed = fruits.splice(2, 2, "Lemon", "Kiwi");
document.getElementById("demo").innerHTML = "Removed Items:<br> " + removed;
```

```js
// Removed Items:
// Apple,Mango
```

```js
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.splice(0, 1);
```

```js
// Orange,Apple,Mango
```

</details>

<details>
  <summary>17. Array slice()</summary>

The slice() method slices out a piece of an array into a new array.<br>
This example slices out a part of an array starting from array element 1 ("Orange").<br>
The slice() method creates a new array.<br>
The slice() method does not remove any elements from the source array.<br>
The slice() method can take two arguments like slice(1, 3).<br>
The method then selects elements from the start argument, and up to (but not including) the end argument.<br>

```js
const fruits = ["Banana", "Orange", "Lemon", "Apple", "Mango"];
const citrus = fruits.slice(1);
```

```js
// Orange,Lemon,Apple,Mango
```

```js
const fruits = ["Banana", "Orange", "Lemon", "Apple", "Mango"];
const citrus = fruits.slice(3);
```

```js
// Apple,Mango
```

```js
const fruits = ["Banana", "Orange", "Lemon", "Apple", "Mango"];
const citrus = fruits.slice(1, 3);
```

```js
// Orange,Lemon
```

</details>

<details>
  <summary>18. Array sort()</summary>

The sort() method sorts an array alphabetically.

```js
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.sort();
```

```js
// Apple,Banana,Mango,Orange
```

```js

```

```js

```

</details>

<details>
  <summary>19. Array reverse()</summary>
The reverse() method reverses the elements in an array.<br>
You can use it to sort an array in descending order.<br>

```js
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.sort();
fruits.reverse();
```

```js
// Orange,Mango,Banana,Apple
```

</details>

<details>
  <summary>20. Array Numeric Sort()</summary>
By default, the sort() function sorts values as strings.<br>
This works well for strings ("Apple" comes before "Banana").<br>
However, if numbers are sorted as strings, "25" is bigger than "100", because "2" is bigger than "1".<br>
Because of this, the sort() method will produce incorrect result when sorting numbers.<br>
You can fix this by providing a compare function.<br>
The purpose of the compare function is to define an alternative sort order.<br>
The compare function should return a negative, zero, or positive value, depending on the arguments.<br>
When the sort() function compares two values, it sends the values to the compare function, and sorts the values according to the returned (negative, zero, positive) value.<br>
If the result is negative, a is sorted before b.<br>
If the result is positive, b is sorted before a.<br>
If the result is 0, no changes are done with the sort order of the two values.<br>

```js
const points = [40, 100, 1, 5, 25, 10];
points.sort(function (a, b) {
  return a - b;
}); //Sort ascending
```

```js
// 1,5,10,25,40,100
```

```js
const points = [40, 100, 1, 5, 25, 10];
points.sort(function (a, b) {
  return b - a;
}); //Sort descending
```

```js
// 100,40,25,10,5,1
```

</details>

<details>
  <summary>21. The Fisher Yates Method</summary>
The random implementation for array.sort() is not accurate.<br>
It will favor some numbers over the others.<br>
The most popular correct method, is called the Fisher Yates shuffle, and was introduced in data science as early as 1938!<br>
In JavaScript the method can be translated to this.<br>

```js
const points = [40, 100, 1, 5, 25, 10];

for (let i = points.length - 1; i > 0; i--) {
  let j = Math.floor(Math.random() * (i + 1));
  let k = points[i];
  points[i] = points[j];
  points[j] = k;
}
```

```js
// 10,100,5,1,40,25
```

The random implementation for array.sort():

```js
const points = [40, 100, 1, 5, 25, 10];
points.sort(function () {
  return 0.5 - Math.random();
});
```

</details>

<details>
  <summary>22. Find the Highest Array Value - Math.max.apply()</summary>
There are no built-in functions for finding the max or min value in an array.<br>
However, after you have sorted an array, you can use the index to obtain the highest and lowest values.<br>
Sorting a whole array is a very inefficient method if you only want to find the highest (or lowest) value.<br>
You can use Math.max.apply to find the highest number in an array.<br>
Math.max.apply(null, [1, 2, 3]) is equivalent to Math.max(1, 2, 3).<br>

```js
const points = [40, 100, 1, 5, 25, 10];
points.sort(function (a, b) {
  return a - b;
});
points[0];
// now points[0] contains the lowest value
// and points[points.length-1] contains the highest value
```

```js
const points = [40, 100, 1, 5, 25, 10];
Math.max.apply(null, points);
```

```js
// 100
```

Find Max "home made" method:

```js
function myArrayMax(arr) {
  let len = arr.length;
  let max = -Infinity;
  while (len--) {
    if (arr[len] > max) {
      max = arr[len];
    }
  }
  return max;
}
```

</details>

<details>
  <summary>23. Find the Lowest Array Value - Math.min.apply()</summary>
There are no built-in functions for finding the max or min value in an array.<br>
However, after you have sorted an array, you can use the index to obtain the highest and lowest values.<br>
Sorting a whole array is a very inefficient method if you only want to find the highest (or lowest) value.<br>
You can use Math.min.apply to find the lowest number in an array.<br>
Math.min.apply(null, [1, 2, 3]) is equivalent to Math.min(1, 2, 3).<br>

```js
const points = [40, 100, 1, 5, 25, 10];
points.sort(function (a, b) {
  return b - a;
});
points[0];
// now points[0] contains the highest value
// and points[points.length-1] contains the lowest value
```

```js
const points = [40, 100, 1, 5, 25, 10];
Math.min.apply(null, points);
```

```js
// 1
```

Find Min "home made" method:

```js
function myArrayMin(arr) {
  let len = arr.length;
  let min = Infinity;
  while (len--) {
    if (arr[len] < min) {
      min = arr[len];
    }
  }
  return min;
}
```

</details>

<details>
  <summary>24. Sorting Objects in Arrays</summary>
JavaScript arrays often contain objects.<br>
Even if objects have properties of different data types, the sort() method can be used to sort the array.<br>
The solution is to write a compare function to compare the property values.<br>
Comparing string properties is a little more complex.

```js
const cars = [
  { type: "Volvo", year: 2016 },
  { type: "Saab", year: 2001 },
  { type: "BMW", year: 2010 },
];

cars.sort(function (a, b) {
  return a.year - b.year;
});
```

```js
// [
//   { type: "Saab", year: 2001 },
//   { type: "BMW", year: 2010 },
//   { type: "Volvo", year: 2016 },
// ];
```

```js
const cars = [
  { type: "Volvo", year: 2016 },
  { type: "Saab", year: 2001 },
  { type: "BMW", year: 2010 },
];

cars.sort(function (a, b) {
  let x = a.type.toLowerCase();
  let y = b.type.toLowerCase();
  if (x < y) {
    return -1;
  }
  if (x > y) {
    return 1;
  }
  return 0;
});
```

```js
// [
//   { type: "BMW", year: 2010 },
//   { type: "Saab", year: 2001 },
//   { type: "Volvo", year: 2016 },
// ];
```

</details>

<details>
  <summary>25. sample</summary>

```js

```

```js

```

```js

```

```js

```

</details>

<details>
  <summary>26. sample</summary>

```js

```

```js

```

```js

```

```js

```

</details>

<details>
  <summary>27. sample</summary>

```js

```

```js

```

```js

```

```js

```

</details>

<details>
  <summary>28. sample</summary>

```js

```

```js

```

```js

```

```js

```

</details>

<details>
  <summary>29. sample</summary>

```js

```

```js

```

```js

```

```js

```

</details>

<details>
  <summary>30. sample</summary>

```js

```

```js

```

```js

```

```js

```

</details>

### [2-JAVASCRIPT COURSE - DAVE GRAY](#)

+INTRODUCTION

<details>
  <summary>1. Javascript Comments</summary>

```js
// this is a comment
```

</details>

<details>
  <summary>2. Data Types</summary>

```js
typeof "Dave";
//'string'

typeof 7;
//'number'

typeof true;
//'boolean'

typeof {};
//'object'

typeof [];
//'object'

let userName;
undefined;

typeof userName;
//'undefined'
```

</details>

<details>
  <summary>3. Script Tag Inline</summary>

index.html:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>My Page</title>
    <link rel="stylesheet" href="css/main.css" />
    <script defer>
      console.log("Hello World");
    </script>
  </head>
  <body>
    <main><h1>My Page</h1></main>
  </body>
</html>
```

</details>

<details>
  <summary>4. Script Tag External</summary>

index.html:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>My Page</title>
    <link rel="stylesheet" href="./css/main.css" />
    <script src="./js/main.js" defer></script>
  </head>

  <body>
    <main>
      <h1>My Page</h1>
    </main>
  </body>
</html>
```

main.js:

```js
console.log("Hello World");
```

</details>

+STRING METHODS

<details>
  <summary>5. Length Method</summary>

main.js:

```js
// Strings
const myVariable = "Mathematics";

// The length property
console.log(myVariable.length);
```

```js
// 11
```

</details>

<details>
  <summary>6. CharAt Method</summary>

```js
// Strings
const myVariable = "Mathematics";

// String Methods
console.log(myVariable.charAt(0));
```

```js
// M
```

</details>

<details>
  <summary>7. IndexOf Method</summary>

Provides First occurrence of a string or character:

```js
// Strings
const myVariable = "Mathematics";

// String Methods
console.log(myVariable.indexOf("m"));
```

```js
// 5
```

</details>

<details>
  <summary>8. LastIndexOf Method</summary>

Provides Last occurrence of a string or character:

```js
// Strings
const myVariable = "Mathematics";

// String Methods
console.log(myVariable.lastIndexOf("at"));
```

```js
// 6
```

</details>

<details>
  <summary>9. Slice Method</summary>

```js
// Strings
const myVariable = "Mathematics";

// String Methods
console.log(myVariable.slice(4));
```

```js
// ematics
```

```js
// Strings
const myVariable = "Mathematics";

// String Methods
console.log(myVariable.slice(4, 7));
```

```js
// ema
```

</details>

<details>
  <summary>10. toUpperCase and toLowerCase Method</summary>

```js
// Strings
const myVariable = "Mathematics";

// String Methods
console.log(myVariable.toUpperCase());
```

```js
// MATHEMATICS
```

```js
// Strings
const myVariable = "Mathematics";

// String Methods
console.log(myVariable.toLowerCase());
```

```js
// mathematics
```

</details>

<details>
  <summary>11. Includes Method</summary>

```js
// Strings
const myVariable = "Mathematics";

// String Methods
console.log(myVariable.includes("mat"));
```

```js
// true
```

</details>

<details>
  <summary>12. Split Method</summary>

```js
// Strings
const myVariable = "Mathematics";

// String Methods
console.log(myVariable.split("e"));
```

```js
// ['Math', 'matics']
```

```js
// Strings
const myVariable = "Mathematics";

// String Methods
console.log(myVariable.split(""));
```

```js
// ['M', 'a', 't', 'h', 'e', 'm', 'a', 't', 'i', 'c', 's']
```

</details>

+NUMBER METHODS

<details>
  <summary>13. Comparing Number Data Types</summary>

```js
// Numbers
const myNumber = 42;

const myFloat = 42.0;

const myString = "42";

console.log(myNumber === myFloat);
console.log(myNumber === myString);
console.log(myFloat === myString);
```

```js
// true
// false
// false
```

</details>

<details>
  <summary>14. Number Function (Type Casting)</summary>

```js
const myNumber = 42;

const myFloat = 42.0;

const myString = Number("42");

console.log(typeof myString);
console.log(myFloat === myString);
```

```js
// number
// true
```

</details>

<details>
  <summary>15. isInteger method</summary>

```js
// Number Methods
//The Number.isInteger() method determines whether the passed value is an integer.

const myNumber = 42;

const myFloat = 42.01;

const myString = "42";

console.log(Number.isInteger(myNumber));
console.log(Number.isInteger(myFloat));
console.log(Number.isInteger(myString));
```

```js
// true
// false
// false
```

</details>

<details>
  <summary>16. parseFloat Method</summary>

```js
// Number Methods
//The Number.parseFloat() method parses an argument and returns a floating point number. If a number cannot be parsed from the argument, it returns NaN.

const myNumber = 42;

const myFloat = 42.01;

const myString = "42.01";

console.log(Number.parseFloat(myNumber));
console.log(Number.parseFloat(myFloat));
console.log(Number.parseFloat(myString));
```

```js
// 42
// 42.01
// 42.01
```

</details>

<details>
  <summary>17. toFixed Method</summary>

```js
// Number Methods
//The toFixed() method formats a number according to how many decimal points you provide as the parameter.

const myNumber = 42;

const myFloat = 42.0155667;

const myString = "42.01234abc";

console.log(Number.parseFloat(myNumber).toFixed(2));
console.log(Number.parseFloat(myFloat).toFixed(2));
console.log(Number.parseFloat(myString).toFixed(2));
```

```js
// '42.00'
// '42.02'
// '42.01'
```

</details>

<details>
  <summary>18. parseInt Method</summary>

```js
// Number Methods
//The Number.parseInt() method parses an argument and returns a whole number. If a number cannot be parsed from the argument, it returns NaN.

const myNumber = 42;

const myFloat = 42.01235235;

const myString = "42.013425335";

console.log(Number.parseInt(myNumber));
console.log(Number.parseInt(myFloat));
console.log(Number.parseInt(myString));
```

```js
// 42
// 42
// 42
```

</details>

<details>
  <summary>19. toString Method</summary>

```js
// Number Methods
//The toString() method returns a string representing the number.

const myNumber = 42;

const myFloat = 42.01235235;

const myString = "42.013425335";

console.log(myNumber.toString());
console.log(myFloat.toString());
console.log(myString.toString());
```

```js
// '42'
// '42.01235235'
// '42.013425335'
```

</details>

+MATH OBJECT METHODS

<details>
  <summary>20. Math.PI</summary>

```js
// Math Methods

console.log(Math.PI);
```

```js
// 3.141592653589793
```

</details>

<details>
  <summary>21. Math.trunc Method</summary>

```js
// Math Methods

console.log(Math.trunc(Math.PI));
```

```js
// 3
```

</details>

<details>
  <summary>22. Math.round Method</summary>

```js
// Math Methods

console.log(Math.round(3.64));
```

```js
// 4
```

</details>

<details>
  <summary>23. Math.ceil Method</summary>

```js
// Math Methods

console.log(Math.ceil(3.14));
```

```js
// 4
```

</details>

<details>
  <summary>24. Math.floor Method</summary>

```js
// Math Methods

console.log(Math.floor(3.74));
```

```js
// 3
```

</details>

<details>
  <summary>25. Math.pow Method</summary>

```js
// Math Methods

console.log(Math.pow(2, 3));
console.log(Math.pow(2, 4));
console.log(Math.pow(2, 10));
console.log(Math.pow(5, 2));
```

```js
// 8
// 16
// 1024
// 25
```

</details>

<details>
  <summary>26. Math.min and Math.max Method</summary>

```js
// Math Methods

console.log(Math.min(2, 4, 6, 8, 10));
console.log(Math.max(2, 4, 6, 8, 10));
```

```js
// 2
// 10
```

</details>

<details>
  <summary>27. Math.random Method</summary>

```js
// Math Methods

console.log(Math.random());
console.log(Math.random());
console.log(Math.random());
console.log(Math.random());
console.log(Math.random());
```

```js
// 0.36200306252129133
// 0.3547990279443072
// 0.8440334640521379
// 0.11641092554022392
// 0.3834524936794077
```

</details>

+CONDITIONALS

<details>
  <summary>28. If-Else-If Statements</summary>

```js
// Conditionals: If Statements
// Conditionals: If Else Statements
// Conditionals: If Else If Statements

const customerIsBanned = false;
let soup = "chicken noodle soup";
let crackers = true;
let reply;

if (customerIsBanned) {
  reply = "No soup for you!";
} else if (soup && crackers) {
  reply = `Here's your order of ${soup} & crackers.`;
} else if (soup) {
  reply = `Here's your order of ${soup}`;
} else {
  reply = "Sorry, we're out of soup.";
}
console.log(reply);
```

```js
// Conditionals: If Statements
// Conditionals: If Else Statements
// Conditionals: If Else If Statements

let testScore = 89;
let collegeStudent = true;
let grade;

if (testScore >= 90) {
  grade = "A";
} else if (testScore >= 80) {
  grade = "B";
} else if (testScore >= 70) {
  grade = "C";
} else if (testScore >= 60) {
  grade = "D";
} else {
  if (collegeStudent) {
    grade = "U";
  } else {
    grade = "F";
  }
}

console.log(grade);
```

</details>

<details>
  <summary>29. *RPS Game 1*</summary>

index.html:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>My Page</title>
    <link rel="stylesheet" href="./css/main.css" />
    <script src="./js/main.js" defer></script>
  </head>

  <body>
    <main>
      <h1>RPS GAME</h1>
      <select id="userChoice">
        <option value="Rock">Rock</option>
        <option value="Paper">Paper</option>
        <option value="Scissors">Scissors</option>
      </select>
      <button id="btn">Submit</button>
    </main>
  </body>
</html>
```

main.js:

```js
// Conditionals: If Statements
// Conditionals: If Else Statements
// Conditionals: If Else If Statements

const win = "You Win!";
const Loss = "You Lose!";
const choice = ["Rock", "Paper", "Scissors"];

data = {
  RP: Loss,
  RS: win,
  RR: "Tie!",
  SP: win,
  SS: "Tie!",
  SR: Loss,
  PP: "Tie!",
  PS: Loss,
  PR: win,
};

document.getElementById("btn").addEventListener("click", () => {
  const userChoice = document.getElementById("userChoice").value;
  const computerChoice = choice[Math.floor(Math.random() * choice.length)];
  if (userChoice) {
    console.log(data[userChoice[0] + computerChoice[0]]);
    console.log(`You chose: ${userChoice}`);
    console.log(`Computer chose: ${computerChoice}`);
  }
});
```

</details>

<details>
  <summary>30. Switch Statements</summary>

```js
// Conditionals: Switch Statements
// syntax
switch (expression OR value) {
    case value1:
        // code block
        break;
    case value2:
        // code block
        break;
    default:
        // code block
}
```

main.js:

```js
let playerOne = "rock";
let computer = "paper";

switch (playerOne) {
  case computer:
    console.log("Tie game!");
    break;
  case "rock":
    if (computer === "paper") {
      console.log("computer wins!");
    } else {
      console.log("playerOne wins!");
    }
    break;
  case "paper":
    if (computer === "scissors") {
      console.log("computer wins!");
    } else {
      console.log("playerOne wins!");
    }
    break;
  default:
    if (computer === "rock") {
      console.log("computer wins!");
    } else {
      console.log("playerOne wins!");
    }
}
```

</details>

<details>
  <summary>31. Ternary Operator</summary>

```js
// Conditionals: Ternary Operator

//syntax
//condition? ifTrue: ifFalse;

let soup = "Chicken Noodle Soup";
let response = soup ? "Yes, we have soup." : "Sorry, no soup today.";

console.log(response);
```

```js
// Conditionals: Ternary Operator

//syntax
//condition ? ifTrue: iffalse;

let soup = "Chicken Noodle Soup";
let isCustomerBanned = false;
let soupAccess = isCustomerBanned
  ? "Sorry, no soup for you!"
  : soup
  ? `Yes, we have ${soup} today.`
  : "Sorry, no soup today.";

console.log(soupAccess);
```

```js
// Conditionals: Ternary Operator
//syntax
//condition? ifTrue: iffalse;

let playerOne = "rock";
let computer = "paper";

let result =
  playerOne === computer
    ? "Tie game!"
    : playerOne === "rock" && computer === "paper"
    ? "Computer wins!"
    : playerOne === "paper" && computer === "scissors"
    ? "Computer wins!"
    : playerOne === "scissors" && computer === "rock"
    ? "Computer wins!"
    : "playerOne wins!";

console.log(result);
```

</details>

+USER INPUTS

<details>
  <summary>32. Alert Input</summary>

```js
// User Input
alert("Hello World!");
```

</details>

<details>
  <summary>33. Confirm Input</summary>

```js
// User Input
const result = confirm("Ok === True\nCancel === False");
console.log(result);
```

```js
// User Input
const result = confirm("Are you sure you want to delete this file?");
console.log(result);
```

</details>

<details>
  <summary>34. Prompt Input</summary>

```js
// User Input
let name = prompt("Please enter your name.");
console.log(name ?? "You didn't enter your name.");
```

```js
// User Input
let name = prompt("Please enter your name.");
const warning = "You didn't enter your name.";

if (name && name.trim() !== "") {
  console.log(name.trim());
} else {
  console.log(`${warning} Please try again.`);
}
```

</details>

<details>
  <summary>35. *RPS Game 2*</summary>

```js
// RPS Game
const options = ["rock", "paper", "scissors"];
const draw = "It was a Tie!";
const win = "You Win!";
const lose = "You Lose!";

function start() {
  const playGame = confirm("Do you want to play RPS?");
  if (playGame) {
    let userChoice = prompt("Choose rock, paper, or scissors").toLowerCase();
    if (options.includes(userChoice)) {
      let computerChoice = options[Math.floor(Math.random() * options.length)];
      const result =
        userChoice === computerChoice
          ? draw
          : userChoice === "rock" && computerChoice === "scissors"
          ? win
          : userChoice === "paper" && computerChoice === "rock"
          ? win
          : userChoice === "scissors" && computerChoice === "paper"
          ? win
          : lose;
      alert(
        `You chose ${userChoice} and the computer chose ${computerChoice}. ${result}`
      );
      location.reload();
    } else if (userChoice || userChoice === "") {
      const retry = confirm(
        "Please choose a valid option. Do you want to try again?"
      );
      if (retry) {
        console.log("Starting again...");
        location.reload();
      } else {
        alert("Sorry to see you go. Goodbye!");
      }
    } else {
      alert("Sorry to see you go. Goodbye!");
    }
  } else {
    alert("Ok, maybe next time. Goodbye!");
  }
}

start();
```

```js
// You chose rock and the computer chose scissors. You Win!
```

</details>

+LOOPS

<details>
  <summary>36. While Loop</summary>

```js
// Loops
let myNumber = 0;

while (myNumber < 50) {
  console.log(myNumber);
  myNumber++;
}
```

```js
// Loops
let myNumber = 0;

while (myNumber < 50) {
  myNumber += 2;
  console.log(myNumber);
}
```

</details>

<details>
  <summary>37. Do While Loop</summary>

```js
// Loops
let myNumber = 0;

do {
  console.log(myNumber);
  myNumber += 2;
} while (myNumber < 10);
```

```js
// 0
// 2
// 4
// 6
// 8
```

</details>

<details>
  <summary>38. For Loop</summary>

```js

```

```js

```

</details>

<details>
  <summary>39. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>40. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>41. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>42. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>43. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>44. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>45. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>46. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>47. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>48. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>49. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>50. sample</summary>

```js

```

```js

```

</details>
