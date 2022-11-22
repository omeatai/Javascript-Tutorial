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

</details>

<details>
  <summary>13. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>14. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>15. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>16. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>17. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>18. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>19. sample</summary>

```js

```

```js

```

</details>

<details>
  <summary>20. sample</summary>

```js

```

```js

```

</details>
