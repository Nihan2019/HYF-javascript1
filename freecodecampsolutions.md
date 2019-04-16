```

.js 
```
create a var variable 
```
// Example
   var myName;

// Declare myName below this line
```
---
assigning a value
```// Setup 
var a;
var b = 2;

// Only change code below this line
var a = 7; 
var b = 7;
b = a;
```
---
to define a variable
```
var ourVar = 19;

// Only change code below this line 
var a = 9;
```
---
initializing a number or undefined
```
// Initialize these three variables 
var a = 5;
var b = 10; 
var c ="I am a";

// Do not change code below this line

a = a + 1; 
b = b + 5;
c = c + " String!";
```
---
to learn about case 
```
// Declarations var studlyCapVar;
   var properCamelCase; 
    var titleCaseOver;
```
---
Assignments 
```
studlyCapVar = 10; 
properCamelCase = "A String"; 
titleCaseOver = 9000;
```
---
adding the numbers
```
var sum = 10 + 10;
```
---
find the difference between the numbers
```
var difference = 45 - 33;
```
---
product the numbers
```
var product = 8 * 10;
```
---
finding the quotient
```
var quotient = 66 / 33;
```
---
increasing numbers one
```
var myVar = 87;

// Only change code below this line 
  myVar++;
```
---
decreasing numbers one 
```
var myVar = 11;

// Only change code below this line
myVar--;
```
---
create a decimal number
```
var ourDecimal = 5.7;

// Only change code below this line

var myDecimal = 3.6;
```
---
multiplying two decimals 
```
var product = 2.0 * 2.5;
```
---
dividing decimals
```
var quotient = 4.4 / 2.0; // Fix this line

```
---
finding the remainder of a division
```
var remainder; remainder = 11 % 3;

```
---
adding numbers in a short way
```
var a = 3; var b = 17; var c = 12;

// Only modify code below this line

a+= 12; b+= 9; c+= 7;
```
---

subtracting numbers in a short way
```
var a = 11; var b = 9; var c = 3;

// Only modify code below this line

a-= 6; b-= 15; c-= 1;

``` 
---
multiplying numbers in a short way
```
var a = 5; var b = 12; var c = 4.6;

// Only modify code below this line

a*= 5; b*= 3; c*= 10;

```
---
dividing in a short way
``` var a = 48; var b = 108; var c = 33;

// Only modify code below this line

a/= 12; b/= 4; c/= 11;
```
---

assigning a name
```// Example var firstName = "Alan"; 
            var lastName = "Turing";

// Only change code below this line
var myFirstName = "Nihan"; 
var myLastName = "Akkose";

```
---
about two times quotes
``` var myStr = "I am a "double quoted" string inside "double quotes".";
// Change this line
```
---
Quoting Strings with Single Quotes
``` var myStr =' Link';

```
---
it was hard to solve
```
var myStr = "FirstLine\n\t\SecondLine\nThirdLine";// Change this line

```
---
concenating strings
```
var ourStr = "I come first. " + "I come second.";

// Only change code below this line

var myStr; 
myStr = "This is the start. " + "This is the end."

```
---
concenating with plus
```
// Example 
var ourStr = "I come first. "; ourStr += "I come second.";

// Only change code below this line

var myStr;

myStr = "This is the first sentence. " ; 
myStr += "This is the second sentence.";

```
---
concenating three strings
``` var ourName = "freeCodeCamp"; 
var ourStr = "Hello, our name is " + ourName + ", how are you?";

// Only change code below this line 
var myName;
var myStr; 
myName = "Nihan"; 
myStr = "My name is " + myName + " and I am well!";

```
---
Appending Variables to Strings
``` // Example
var anAdjective = "awesome!"; 
var ourStr = "freeCodeCamp is "; 
ourStr += anAdjective;

// Only change code below this line

var someAdjective = "challenging!"; 
var myStr = "Learning to code is ";
myStr += someAdjective;

```
---
finding the length of a string 
```
// Example
var anAdjective = "awesome!"; 
var ourStr = "freeCodeCamp is "; 
ourStr += anAdjective;

// Only change code below this line

var someAdjective = "challenging!"; 
var myStr = "Learning to code is "; 
myStr += someAdjective;

```
---
using bracket to find the first letter
```// Example 
var firstLetterOfFirstName = ""; 
var firstName = "Ada";

firstLetterOfFirstName = firstName[0];

// Setup var firstLetterOfLastName = ""; 
var lastName = "Lovelace";

// Only change code below this line 
firstLetterOfLastName = lastName[0];

```
---
string immutability
``` 
// Setup var myStr = "Jello World";

// Only change code below this line

myStr = "Hello World";// Fix Me

```
---
the nth letter
```
// Example var firstName = "Ada"; 
var secondLetterOfFirstName = firstName[1];

// Setup var lastName = "Lovelace";

// Only change code below this line. 
var thirdLetterOfLastName = lastName[2];

```
---
the last letter
``` // Example var firstName = "Ada"; 
var lastLetterOfFirstName = firstName[firstName.length - 1];

// Setup var lastName = "Lovelace";

// Only change code below this line. 
var lastLetterOfLastName = lastName[lastName.length - 1];

```
---
nth to last letter of a string
```
// Example
var firstName = "Ada";
var thirdToLastLetterOfFirstName = firstName[firstName.length - 3];

// Setup var lastName = "Lovelace";

// Only change code below this line
var secondToLastLetterOfLastName = lastName[lastName.length - 2];

```
---
word blanks
```
function wordBlanks(myNoun, myAdjective, myVerb, myAdverb) { 
// Your code below this line 
var result = "My"+" " + myAdjective +" "+ myNoun +" " + myVerb +" " + "very" + " " +myAdverb+ ".";

// Your code above this line return result; 
}

// Change the words here to test your function wordBlanks("dog", "big", "ran", "quickly");

```
---
Arrays
```
// Example var ourArray = ["John", 23];

// Only change code below this line. 
var myArray = ["Nihan",43];
```
---
Multi-dimensional Array 
```// Example var ourArray = [["the universe", 42], ["everything", 101010]];

// Only change code below this line. 
var myArray = [["Aydin",46],["Nihan",43]];

```
---
indexes
```
// Example var ourArray = [50,60,70]; 
var ourData = ourArray[0]; // equals 50

// Setup var myArray = [50,60,70];
var myData = myArray[0];

// Only change code below this line.

```
---
mutable array indexes
```
// Example
var ourArray = [18,64,99];
ourArray[1] = 45; // ourArray now equals [18,45,99].

// Setup var myArray = [18,64,99]; 
myArray[0] = 45;

// Only change code below this line.

```
---
Array of arrays
```
// Setup var myArray = [[1,2,3], [4,5,6], [7,8,9], [[10,11,12], 13, 14]];

// Only change code below this line. 
var myData = myArray[2][1];
```
---
Manipulate Arrays With push()
```
// Example
var ourArray = ["Stimpson", "J", "cat"]; ourArray.push(["happy", "joy"]);
// ourArray now equals ["Stimpson", "J", "cat", ["happy", "joy"]]

// Setup var myArray = [["John", 23], ["cat", 2]];
myArray.push(["dog",3]);

// Only change code below this line. 
```
---
Manipulate Arrays With pop()
```
/ Example var ourArray = [1,2,3]; 
var removedFromOurArray = ourArray.pop(); 
// removedFromOurArray now equals 3, and ourArray now equals [1,2]

// Setup var myArray = [["John", 23], ["cat", 2]];

// Only change code below this line. 
var removedFromMyArray = myArray.pop();

```
---
Manipulate Arrays With unshift()
```

/ Example 
var ourArray = ["Stimpson", "J", "cat"]; 
ourArray.shift();
// ourArray now equals ["J", "cat"] ourArray.unshift("Happy"); 
// ourArray now equals ["Happy", "J", "cat"]

// Setup var myArray = [["John", 23], ["dog", 3]];
myArray.shift(); 
myArray.unshift(["Paul",35] );

// Only change code below this line.

```
---
Shopping List
```
var myList = [["Cereal",2],["Apple",5],["egg",30],["peer",10],["Cake",1]];

```
---
Creating functions
```
// Example= function ourReusableFunction() {
console.log("Heyya, World"); 
}
ourReusableFunction();

// Only change code below this line function reusableFunction(){ 
console.log("Hi World");
} 
reusableFunction();

```
---
Functions with arguments
```
// Example function ourFunctionWithArgs(a, b) { 
console.log(a - b);
} 
ourFunctionWithArgs(10, 5); // Outputs 5

// Only change code below this line.
function functionWithArgs(a, b) { 
console.log(a + b);
} 
functionWithArgs(10, 5);

```
---
Local scope functionshard
``` 
// Declare your variable here var myGlobal = 10;

function fun1() { 
// Assign 5 to oopsGlobal Here

oopsGlobal = 5;
}

// Only change code above this line 
function fun2() { 
var output = ""; 
if (typeof myGlobal != "undefined") { 
output += "myGlobal: " + myGlobal;
} if (typeof oopsGlobal != "undefined") { 
output += " oopsGlobal: " + oopsGlobal; 
} console.log(output);
}

```
---
Local scopeI didnt understan but I passed.
```
function myLocalScope() { var myVar='use strict'; // you shouldn't need to edit this line

console.log(myVar); 
}
myLocalScope();

// Run and check the console // myVar is not defined outside of myLocalScope

// Now remove the console log line to pass the test 


return a value a function
```
---
```
// Example
function minusSeven(num) { 
return num - 7; 
}

// Only change code below this line
function timesFive(num) { 
return num*5; 
}
console.log(minusSeven(10));

```
---
Understanding Undefined Value returned from a Function
```
// Example var sum = 0; function addThree() {
sum = sum + 3; 
}

// Only change code below this line
function addFive(){ 
sum= sum + 5; 
}

// Only change code above this line
var returnedValue = addFive();

```
---
Assigment with areturned value
```

return arr.shift() ; // Change this line 

// Test Setup var testArr = [1,2,3,4,5];

// Display Code console.log("Before: " + JSON.stringify(testArr)); 
console.log(nextInLine(testArr, 6)); 
// Modify this line to test console.log("After: " + JSON.stringify(testArr));

```
---
Boolean values
```
function welcomeToBooleans() {

// Only change code below this line.

return true; // Change this line

// Only change code above this line. 
} 
```
---
If statements
```
// Example 
function ourTrueOrFalse(isItTrue) { 
if (isItTrue) { 
return "Yes, it's true";
} 
return "No, it's false"; 
}
```
---
```
// Setup function trueOrFalse(wasThatTrue) {

// Only change code below this line. 
if (wasThatTrue) { 
return "Yes, that was true"; 
}
return "No, that was false" ; 
// Only change code above this line.

}

// Change this value to test trueOrFalse(true);

```
---

```
// Example 
function ourTrueOrFalse(isItTrue) { 
if (isItTrue) { 
return "Yes, it's true"; 
} return "No, it's false";
}
```
---
```
// Setup function trueOrFalse(wasThatTrue) {

// Only change code below this line.
if (wasThatTrue) { 
return "Yes, that was true"; 
}
return "No, that was false" ;
// Only change code above this line.

}

// Change this value to test trueOrFalse(true);
```
---

strict equality operator
```
function testStrict(val) { 
if (val===7) {
// Change this line return "Equal";
} return "Not Equal"; }

// Change this value to test testStrict(10);
```
---

comparison equality
```
// Setup function compareEquality(a, b) { 
if (a === 'b') { 
// Change this line return "Equal";
} return "Not Equal";
}

// Change this value to test compareEquality(10, "10");

```
---
comparison inequality
```
function testNotEqual(val) { 
if (val!= 99) { 
// Change this line return "Not Equal"; 
} return "Equal"; 
}

// Change this value to test testNotEqual(10);

```
---
Comparison with the Greater Than Or Equal To Operator
```
function testGreaterOrEqual(val) {
if (val>=20) { 
// Change this line return "20 or Over";
}
if (val>=10) {
// Change this line return "10 or Over"; 
}
return "Less than 10";
}
// Change this value to test testGreaterOrEqual(10);

```
---
less than operator
```
function testLessThan(val) {
if (val<25) {
// Change this line return "Under 25";
}

if (val<55) {
// Change this line return "Under 55";
}

return "55 or Over"; 
}

// Change this value to test testLessThan(10);

```
---
less than or equal to
```
function testLessOrEqual(val) {
if (val<=12) {
// Change this line return "Smaller Than or Equal to 12";
}

if (val<=24) { 
// Change this line return "Smaller Than or Equal to 24"; 
}

return "More Than 24"; 
}

// Change this value to test testLessOrEqual(10);

```
---
Comparision with logical operetor 
```
function testLogicalAnd(val) { 
// Only change code below this line

if (val >= 25 && val <=50 ) {

  return "Yes";
}

// Only change code above this line return "No";
}

// Change this value to test testLogicalAnd(10);

```
---
Comparisons with the Logical Or Operator
```
function testLogicalOr(val) { 
// Only change code below this line

if (val > 20 || val <10 ) { 
return "Outside"; 
}

// Only change code above this line return "Inside";
}

// Change this value to test testLogicalOr(15);

```
---
Else statement
```
function testElse(val) {
var result = ""; 
// Only change code below this line

if (val > 5) { 
result = "Bigger than 5";
}

else {
result = "5 or Smaller";
}

// Only change code above this line return result;
}

// Change this value to test testElse(4);

```
---
Else if statement
```
function testElseIf(val) { 
if (val > 10) {
return "Greater than 10";
}

else if (val < 5) {
return "Smaller than 5";
} else { return "Between 5 and 10"; 
}
}
// Change this value to test testElseIf(7);

```
---
Logical Order in If Else Statements
```
function orderMyLogic(val) { 
if (val < 5) { 
return "Less than 5"; 
} else if (val < 10) { 
return "Less than 10";
} else { 
return "Greater than or equal to 10"; 
}
}
// Change this value to test orderMyLogic(7);

```
---
Chaining If Else Statements
```
function testSize(num) { 
// Only change code below this line

if(num < 5 ){
return "Tiny"; 
}else if (num < 10) { 
return "Small"; 
} else if (num < 15 ) {
return "Medium"; 
} else if (num < 20) { 
return "Large";
} else if (num >= 20){
return "Huge"; 
} else{ 
return "Change Me";
}
// Only change code above this line 
}

// Change this value to test testSize(7);
```
---
