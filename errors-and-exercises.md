Errors


Index:

    learning objectives
    exercises
        malfomed while loop (completed example)
        missing variable name
        too-far object access
        access property direclty
        improper multi-line string
        improper end of statement
        malformed array
        missing arguments
        improper nested quotes 1
        improper nested quotes 2
        reassigning to constant
        unassigned const declaration
        is not a function
    study tools
        PythonTutor for JavaScript
        the Parsonizer
    resources

Exercises
malformed while loop

broken code:

let value = 0;
while (value < 9) 
  value++;
};

error message:

Uncaught SyntaxError: Unexpected token }

classification:

    creation phase
    syntax

the fix:

let value = 0;
while (value < 9) {
  value++;
};

your notes:open parantheses is missed.

TOP
missing variable name

broken code:

var = 5;

error message:

SyntaxError: Unexpected token

classification:

    creation phase
    semanitc

the fix:

var a = 5;

your notes:there is no variable name.

TOP
too-far object access

broken code:

let a = {b:3};
let b = a.b.3

error message: `SyntaxError: Unexpected number``

classification:
* creation phase 
* semanitc 

the fix:
```js
let a = {b:3};
let b = a.b

your notes:there is an unexpected number.

TOP
access property directly

broken code:

let x = {b:'e'};
let y = b.e;

error message: no error message``

classification:
* creation phase or execution phase ?
* syntax or semanitc ?

the fix:
```js

your notes:

TOP
improper multi-line string

broken code:

let a = 'this is 
two lines';

error message: `SyntaxError: Unexpected token ILLEGAL``

classification:
* creation phase
* syntax 
the fix:
```js
let a = 'this is two lines';

your notes:we can not write a string unnecessarily in two lines

TOP
improper end of statement

broken code:

let a = 1:

error message: ``SyntaxError: Unexpected token :`

classification:
* creation phase
* syntax 

the fix:
```js
let a = 1;

your notes:at the end of a string there must be semicolon

TOP
malformed array

broken code:

let myArray = [1, 2, 3;

error message: `SyntaxError: Unexpected token ;``

classification:
* creation phase 
*  semanitc 

the fix:
```js
let myArray = [1, 2, 3];

your notes:[] open and end

TOP
missing arguments

broken code:

function getNine {
  let x = 6;
  let y = 3;
  return x + y;
}
let result = getNine();

error message: `SyntaxError: Unexpected token {``

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

your notes:missing arguments

TOP
improper nested quotes 1

broken code:

let innerHtml = "<p>Click here to <a href="#Home">return home</a></p>";

error message: SyntaxError: Unexpected token ILLEGAL```

classification:
* creation phase 
* semanitc 

the fix:
```js
let innerHtml = '<p>Click here to <a href="#Home">return home</a></p>';

your notes:nested quotes single quote

TOP
improper nested quotes 2

broken code:

let nested_messages = 'remind yourself ''i can do this!'' at least once a day';

error message: `SyntaxError: Unexpected string``

classification:
* creation phase 
* syntax 

the fix:
```js
let nested_messages = 'remind yourself "i can do this!" at least once a day';

your notes:improper nested quotes

TOP
reassigning to constant

broken code:

const a = 9;
a = 0;

error message: `no error message``

classification:
*  execution phase 
*  semanitc 

the fix:
```js
const a=9;

your notes:you can not assign two times for const.

TOP
unassigned const declaration

broken code:

const a;
a = 0;

error message: ``SyntaxError: Missing initializer in const declaration`

classification:
* creation phase or execution phase ?
* syntax or semanitc ?

the fix:
```js
 const a = 0;

your notes:

TOP
is not a function

broken code:

let array = [];
array.length()

error message:

classification: *execution phase

    semanitc

the fix:

let array = [];
array.length

your notes:array length is not a function
