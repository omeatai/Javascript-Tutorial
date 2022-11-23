# Javascript-Tutorial

Learn Javascript by Ifeanyi Omeata

## Tutorial

---

### [1-JAVASCRIPT COURSE - DAVE GRAY](#)

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
  <summary>29. *Rock,Paper,Scissors Game*</summary>

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
  <summary>30. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>31. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>32. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>33. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>34. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>35. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>36. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>37. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>38. sample</summary>

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
