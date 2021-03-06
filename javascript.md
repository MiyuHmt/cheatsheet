# JavaScript

## Values types
7 types: 

* `number` : for numbers (integer or floating-point)
* `string` : for strings
* `boolean` : for `true` or `false`
* `object` : for complex data structures
* `undefined` : variable with no affected value
* `null` : only one value: `null`
* `symbol` : for unique identifiers. New type from ECMAScript 6.

## Assign a value
Use the `=` symbol to assign a value. Example:
```javascript
var num = 3;
```

You can create a variable with no assignment. In this case the value of the variable is `undefined`.

If you increment a `undefined` variable, you will receive the `NaN` error, `Not A Number`. Because you can't make an addition with an `undefined` variable. You must first initialize the variable.

## Camel Case
In JavaScript we use the `lower camel case` convention to name our variables. So the first word start with a lower case, the other ones with an upper case, like: `var greatPassword;`

## Operations
* `+` : addition
* `-` : substration
* `*` : multiplication
* `/` : division
* `%` : modulo

## Escape a character
If you want escape a character, put a `\` before it.
Example:
```javascript
var text = 'Je m\'appelle Marine';
```

### Escape a backslash
If you want write a backslach, you must escape it with a second one: `\\`.
Example:
```javascript
var text = 'I am a backslash: \\';
```

### Go on a new line
To go on a new line: `\n`.
Example:
```javascript
var toto = "Hello \nWorld!";
```

### Add a tabulation 
To add a tabulation: `\t`.
Example:
```javascript
var toto = "Hello \tWorld!";
```

## Size of a string
To have the size of a string, use `string.length`.
To have the last character of a string, you can do:
```javascript
var name = 'Marine';
console.log(name[name.length -1]);
```

## Immutability
Strings are immutable ; so we can't change only a part of it.

## Arrays
Access to a value from an array in an array:

```javascript
var name = 'Marine';
var age = 23;
var address = ['street', 'city'];
var array = [name, age, address];

// access to 'city'
console.log(array[2][1]);
```

Add a value in an array: `array.push(value);`

Add a value in the first position in the array: `array.unshift(value);`

Delete the first value from an array: `array.shift();`

Delete the last value from an array: `array.pop();`

### Map method
The `map()` method can be called on an array: `array.map()` and into it you can add a function that is called on all array element. It's like a `for` loop but directly on an array.

```javascript
var arr = [1,2,3,4];

var arr2 = arr.map(function(nb) { return nb+2; });
```

## Conditional (ternary) operator

```javascript
condition ? exprTrue : exprFalse
```

If `condition` is truthy, the opeator returns value of `exprTrue` ; otherwise, it returns the value of `exprFalse`.

## If / Else condition

```javascript
if (cond) {
  // do something
} else if (cond) {
  // do something
} else {
  // do something else
}
```

## Objects

```javascript
var ninja = {
  "strength": 80,
  "speed": 50,
  "weaknesses": ["alien", "magus"]
};
```
You can have an object into an object:
```javascript
var ninja = {
  "strength": 80,
  "speed": 50,
  "weaknesses": ["alien", "magus"],
  "buddy": {
    "animal": "rabbit"
  }
};
```

To access to an oject property, use the `.` : 
```javascript
ninja.speed
```
An other way to access to a property:
```javascript
ninja["speed"]
```
When you want to access to a property but you don't know now which one:

```javacript
var ask = "speed";

ninja[ask];
```
### Manipulate objects

To update a property: 
```javascript
ninja.speed = 100;
```
To add a new property:
```javascript
ninja.weapon = "shuriken";
```

To remove a property:
```javascript
delete ninja.weapon;
```

Check if object has a property:
```javascript
ninja.hasOwnProperty('speed');
```
Send a `boolean`.

## While loop
Execute a block of code as long as the `condition` is `true`.
```javascript
var i = 0;
while (i <= 10) {
  console.log(i);
  i++;
}
```
## For loop
```javascript
for(part1; part2; part3) {}
```

`part1`: is executed before the execution of the code block.
`part2`: defines the condition for executing the code block.
`part3`: is executed after the code block has been executed, until the condition becomes false.

```javascript
for(var i = 0; i <= 10; i++) {
  console.log(i);
}
```


## Generate a random number
Generate a random float number between 0 and 1:
```javascript
var random = Math.random();
console.log(random);
```
Generate a random float number between 0 and 6:
```javascript
var random = Math.random() * 6;
console.log(random);
```

Generate a random number between 0 and 6:
```javascript
var random = Math.floor(random() * 6);
console.log(random);
```
Generate a random number into a rank:
```javascript
Math.floor(Math.random() * (max - min + 1) + min); // + 1 is to include the min
```

## ES6 + ES7

JavaScript is based on the ECMAScript standard. The ES6 version bring a lot of new stuffs to JavaScript.

### Var
`var` should not be ever used in ES6.
Why?
* Too permissive: you can declare multiple variables with the same name in the same scope with `var`.
* With `var` you have a `function scope`, not a `block scope`.
* Your values go back to the beginning of the document.

### Let and Const
With `let` you can declare a variable and change it's value after the declaration. A `let` variable has a `block scope`.

`const` is for constant variable so you can't change the value. A `const` variable has a `block scope` too.

### Templates Strings
Templates Strings are great if you want display some variables into a String. 
You must use backquotes and to display a variable use: `${}`.
```javascript
const fruit = "banana";
const a = `I eat a ${fruit} !`;
```
You can put all JavaScript code that you want into the brackets (ternary...).

### Arrow functions
An other syntax to write functions
```javascript
(param1, param2) => {}
```

If you have only one parameter, parenthesis are not mandatory:

```javascript
param => {}
```
Example:

```javascript
number => `I have ${number} eggs.`;
```

Without params: 
```javascript
() => {}
```
Arrows functions are always anonymous. To resolve this "problem" you can put the arrow function in a variable:
```javascript
const maFunc = number => console.log(`I have ${number} eggs.`)
```
### Default parameter in a function
To have a default value if user put nothing in parameter:
```javascript
function myFruit(fruit = "apple") {}
```

### Destructuring

```javascript
user = {
  name: "Marine",
  age: 23,
  city: "Paris"
};
const {name, age, city} = user;
```

To give a different name to the variable and the parameter: 
```javascript
user = {
  name: "Marine",
  age: 23,
  city: "Paris"
};
const {name: firstname, age, city: town} = user;
```
Put a default value: 
```javascript
user = {
  name: "Marine",
  age: 23
};
const {name, age, city="Lille"} = user;
```
Table destructuring:
```javascript
const weather = ["cloudly", "sunny", "rainy", "windy", "foggy", "snowy", "icy"];
const [a, b, c, d, e, f, g] = weather;
```
Exchange values: 
```javascript
let mine = "Pizza";
let yours = "Pasta";

[mine, yours] = [yours, mine];
```

### Spread operator
The Spread operator: `...`. It's to say that you will all the elements from an element:
```javascript
const ingredientsA = ["carrot", "egg", "ham"];
const ingredientsB = ["tomato", "chicken", "bread"];
const list = [...ingredientsA, ...ingredientsB];
```
