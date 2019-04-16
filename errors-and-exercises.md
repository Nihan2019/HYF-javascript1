# Errors



Practice using the devtools by clicking on the 'VM##:#' link to the right of the error message.  Devtools will automatically open the source code and highlight where the error appears.  With these super simple examples this feature may feel like overkill, but you will appreciate it's help once you move on to the next set of exercises.

### Index:
* [learning objectives](#learning-objectives)
* exercises
    * [malfomed while loop](#malformed-while-loop) (completed example)
    * [missing variable name](#missing-variable-name)
    * [too-far object access](#too-far-object-access)
    * [access property direclty](#access-property-directly)
    * [improper multi-line string](#improper-multi-line-string)
    * [improper end of statement](#improper-end-of-statement)
    * [malformed array](#malformed-array)
    * [missing arguments](#missing-arguments)
    * [improper nested quotes 1](#improper-nested-quotes-1)
    * [improper nested quotes 2](#improper-nested-quotes-2)
    * [reassigning to constant](#reassigning-to-constant)
    * [unassigned const declaration](#unassigned-const-declaration)
    * [is not a function](#is-not-a-function)
* study tools
    * [PythonTutor for JavaScript](http://pythontutor.com/javascript.html#)
    * [the Parsonizer](https://janke-learning.github.io/parsonizer/)
* [resources](https://github.com/janke-learning/errors-and-life-cycle)




---
# Exercises

### malformed while loop

*broken code:
```js
let value = 0;
while (value < 9) 
  value++;
};
```
error message:
```
Uncaught SyntaxError: Unexpected token }
```
classification:
* creation phase
* syntax

the fix:
```js
let value = 0;
while (value < 9) {
  value++;
};
```
your notes:open parantheses is missed.

[TOP](#errors)

---

### missing variable name
*broken code:
```js
var = 5;
```
error message:
```js
SyntaxError: Unexpected token
```
classification:
* creation phase 
*  semanitc 

the fix:
```js
var a = 5;
```
your notes:there is no variable name.

[TOP](#errors)

---

## too-far object access
broken code:
```js
let a = {b:3};
let b = a.b.3
```
error message:
`SyntaxError: Unexpected number``
```
classification:
* creation phase 
* semanitc 

the fix:
```js
let a = {b:3};
let b = a.b
```
your notes:there is an unexpected number.

[TOP](#errors)

---
###access property directly
*broken code:
```js
let x = {b:'e'};
let y = b.e;
```
error message:
no error message``
```
classification:
* creation phase or execution phase ?
* syntax or semanitc ?

the fix:
```js
```
your notes:

[TOP](#errors)

---
## improper multi-line string
*broken code:
```js
let a = 'this is 
two lines';
```
error message:
`SyntaxError: Unexpected token ILLEGAL``
```
classification:
* creation phase
* syntax 
the fix:
```js
let a = 'this is two lines';
```
your notes:we can not write a string  unnecessarily in two lines

[TOP](#errors)

---
### improper end of statement
*broken code:
```js
let a = 1:
```
error message:
``SyntaxError: Unexpected token :`
```
classification:
* creation phase
* syntax 

the fix:
```js
let a = 1;
```
your notes:at the end of a string there must be semicolon

[TOP](#errors)

---
### malformed array
*broken code:
```js
let myArray = [1, 2, 3;
```
error message:
`SyntaxError: Unexpected token ;``
```
classification:
* creation phase 
*  semanitc 

the fix:
```js
let myArray = [1, 2, 3];
```
your notes:[] open and end

[TOP](#errors)

---
## missing arguments
broken code:
```js
function getNine {
  let x = 6;
  let y = 3;
  return x + y;
}
let result = getNine();
```
error message:
`SyntaxError: Unexpected token {``
```
classification:
* creation phase 
* semanitc 

the fix:
```js
1	function getNine () {
2	  let  x = 6;
3	  let y = 3;
4	  return x + y;
5	}
6	let result =getNine();
```
your notes:*missing arguments*

[TOP](#errors)

---
### improper nested quotes 1
*broken code:
```js
let innerHtml = "<p>Click here to <a href="#Home">return home</a></p>";
```
error message:
SyntaxError: Unexpected token ILLEGAL```
```
classification:
* creation phase 
* semanitc 

the fix:
```js
let innerHtml = '<p>Click here to <a href="#Home">return home</a></p>';
```
your notes:nested quotes single quote

[TOP](#errors)

---
###improper nested quotes 2 
*broken code:
```js
let nested_messages = 'remind yourself ''i can do this!'' at least once a day';
```
error message:
`SyntaxError: Unexpected string``
```
classification:
* creation phase 
* syntax 

the fix:
```js
let nested_messages = 'remind yourself "i can do this!" at least once a day';
````
your notes:improper nested quotes

[TOP](#errors)

---
### reassigning to constant
*broken code:
```js
const a = 9;
a = 0;
```
error message:
`no error message``
```
classification:
*  execution phase 
*  semanitc 

the fix:
```js
const a=9;
```
your notes:_you can not assign two times for const._

[TOP](#errors)

---
## unassigned const declaration
*broken code:
```js
const a;
a = 0;
```
error message:
``SyntaxError: Missing initializer in const declaration`
```
classification:
* creation phase or execution phase ?
* syntax or semanitc ?

the fix:
```js
 const a = 0;
```
your notes*constant must be initialized*

[TOP](#errors)

---
## is not a function
*broken code:
```js
let array = [];
array.length()
```
error message:
```
```
classification:
*execution phase 
* semanitc 

the fix:
```js
let array = [];
array.length
```
your notes:array length is not a function



[TOP](#errors)
