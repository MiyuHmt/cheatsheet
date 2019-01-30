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
```bash
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
```bash
var text = 'Je m\'appelle Marine';
```
