# Language Style Guide
A collection of language standards that I have collected from various sources across the internet including my own experiences. The guides included cover concepts of the javascript language/style, vue, and SCSS.

## Vue Framework Guide
This section contains notes that refer to 'https://vuejs.org/v2/style-guide/'
- all concepts in sections priorities A, B, C, and D.
- a special emphasis is added to 'https://vuejs.org/v2/style-guide/#Component-instance-options-order-recommended'

## Javascript Language/Style Guide
The following is pulled from 'https://google.github.io/styleguide/javascriptguide.xml' and should be referred to for more details
- Two spaces for indention, not tabs.
- every think get a semi-colon, no automatic semi-colon insertions
- no horizonatal alignment
```javascript
  // bad
  {
    tiny:   42,  
    longer: 435, 
  };
  // good
  {
    tiny: 42, 
    longer: 435,
  };
```
- Declare all local variables with either const or let
- use arrow functions when possible
- Use template strings instead of concatenation
```javascript 
// bad
function sayHi(name) {
  return 'How are you, ' + name + '?';
}
// good
function sayHi(name) {
  return `How are you, ${name}?`;
}
```
- use template strings for long strings
```javascript
// bad
const longString = 'This is a very long string that ' + 
    'far exceeds the 80 column limit. It does not contain ' + 
    'long stretches of spaces since the concatenated ' +
    'strings are cleaner.';
// good
const longString = `This is a very long string that 
    far exceeds the 80 column limit. It does not contain 
    long stretches of spaces since the concatenated
    strings are cleaner.`;
```
- For loops: use 'for ... in' for objects and 'for ... of' for arrays.
- Constants should be named in ALL_UPPERCASE separated by underscores
- One variable per declaration
``` javascript
// bad
let a = 1, b = 2, c = 3;
// good
let a = 1;
let b = 2;
let c = 3;
```
- Use nested functions to encapsulate logic, but dont put functions within blocks
```javascript
/// bad
function AA(){
  if (x) {
    function foo() {}
  }
}
/// good
function AA(){
  if (x) {
    
  }
  function foo() {}
}
```
- Set the property of an object to null vs using delete
- Use Array and Object literals instead of Array and Object constructors.
```javascript
/// bad
// Length is 3.
var a1 = new Array(x1, x2, x3)

//good
var a = [x1, x2, x3];
```
- Never modify prototypes of built-in objects such as 'Array' or 'String'
- Comments: All files, classes, methods and properties should be documented with JSDoc comments with the appropriate tags and types. 'https://github.com/jsdoc3/jsdoc'
## SCSS Style Guild



   
