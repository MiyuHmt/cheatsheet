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

### Size of a string
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

## Conditional (ternary) operator

```javascript
condition ? exprTrue : exprFalse
```

If `condition` is truthy, the opeator returns value of `exprTrue` ; otherwise, it returns tue value of `exprFalse`.
