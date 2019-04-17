# Reference Type Exercises



### Index
* [examples to study](#examples-to-study)
* [reference exercises](#reference-exercises)
* [array exercises](#array-exercises)
* [object exercises](#object-exercises)
* [arrays vs objects](#arrays-vs-objects)
* nesting -> for week 3

---




## Reference Exercises

__Swap the Object & the Array__  
[on pytut](http://www.pythontutor.com/javascript.html#code=let%20obj%20%3D%20%5B%5D%3B%0Alet%20arr%20%3D%20%7B%7D%3B%0Alet%20_%20%3D%20null%3B%0A%0A//%20swap%20the%20object%20and%20the%20array%0A_%20%3D%20obj%3B%0Aobj%20%3D%20arr%3B%0Aarr%20%3D%20_%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
let obj = [];
let arr = {};
let _ = null;

// --- swap below here ---
_ = obj;
obj = arr;
arr = _;

```

__Complete this code__  
[(read this first)](https://github.com/janke-learning/reference-vs-value)  
[on pytut](http://www.pythontutor.com/javascript.html#code=%20%20let%20value_1%20%3D%205%3B%0A%20%20let%20reference_1%20%3D%20%5B%5D%3B%0A%0A%20%20let%20value_2%20%3D%20value_1%3B%0A%20%20console.assert%28value_2%20%3D%3D%3D%20value_1%29%3B%0A%0A%20%20let%20reference_2%20%3D%20reference_1%3B%0A%20%20console.assert%28reference_2%20%3D%3D%3D%20reference_1%29%3B%0A%0A%20%20value_1%20%3D%203%3B%20//%20write%20this%20line%0A%20%20console.assert%28value_1%20!%3D%3D%20value_2%29%3B%20%20%0A%20%20%20%20%0A%20%20reference_1%3D%5B0%5D,reference_2%3D%5B0%5D%3B%20//%20write%20this%20line%0A%20%20console.assert%28reference_1%5B0%5D%20%3D%3D%3D%20reference_2%5B0%5D%29%3B%0A%0A%20%20//%20remove%20the%20array%20from%20memory%0A%20%20%20%20%20reference_1%20%3D%20null%3B%20//%20write%20this%20line%0A%20%20%20%20%20reference_2%3D%20null%3B%20//%20write%20this%20line&curInstr=0&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
let value_1 = 5;
let reference_1 = [];

let value_2 = value_1;
console.assert(value_2 === value_1);

let reference_2 = reference_1;
console.assert(reference_2 === reference_1);

value_1 = 3; ; 
console.assert(value_1 !== value_2);  

reference_1=[0],reference_2=[0]   ; 
console.assert(reference_1[0] === reference_2[0]);

 reference_1 = null   ;
 reference_2 = null  ;
```

[TOP](#reference-type-exercises)

---

## Array Exercises

__Complete the Assertions__  
[on pytut](http://www.pythontutor.com/javascript.html#code=let%20a_1%20%3D%20%5B%5D%3B%0Alet%20a_2%20%3D%20a_1%3B%0Aconsole.assert%28a_1%20%3D%3D%3D%20a_2%29%3B%0A%0Alet%20b_1%20%3D%20%5B%5D%3B%0Alet%20b_2%20%3D%20%5B%5D%3B%0Aconsole.assert%28b_1%20%20!%3D%3D%20%20b_2%29%3B%0A%0A//%20---%0A%0A%20a_1.push%283%29%3B%0A%20a_2.push%283%29%3B%0Aconsole.assert%28a_1%20%20%3D%3D%3D%20a_2%29%3B%0A%0A%20b_1.push%285%29%3B%0A%20b_2.push%285%29%3B%0Aconsole.assert%28b_1%20!%3D%3D%20b_2%29%3B&curInstr=0&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
let a_1 = [];
let a_2 = a_1;
console.assert(a_1 === a_2);

let b_1 = [];
let b_2 = [];
console.assert(b_1 !== b_2);

// ---

 a_1.push(3);
 a_2.push(3);
console.assert(a_1 === a_2);

 b_1.push(5);
 b_2.push(5);
console.assert(b_1 !== ? b_2);
```

__Complete the Assertions__  
[on pytut](http://www.pythontutor.com/javascript.html#code=let%20a_1%20%3D%20%5B%5D%3B%0Alet%20a_2%20%3D%20a_1%3B%0Aconsole.assert%28a_1%20%3D%3D%3D%20%20a_2%29%3B%0A%0Alet%20b_1%20%3D%20%5B%5D%3B%0Alet%20b_2%20%3D%20%5B%5D%3B%0Aconsole.assert%28b_1%20!%3D%3D%20%20b_2%29%3B%0A%0A//%20---%0A%0Aconst%20key%20%3D%200%3B%0A%0A%20a_1%5Bkey%5D%20%3D%203%3B%0A%20a_2%5Bkey%5D%20%3D%203%3B%0Aconsole.assert%28a_1%20%20%3D%3D%3D%20a_2%29%3B%0A%0A%20b_1%5Bkey%5D%20%3D%205%3B%0A%20b_2%5Bkey%5D%20%3D%205%3B%0Aconsole.assert%28b_1%20!%3D%3D%20%20b_2%29%3B&curInstr=13&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
let a_1 = [];
let a_2 = a_1;
console.assert(a_1 === a_2);

let b_1 = [];
let b_2 = [];
console.assert(b_1 !== b_2);

// ---

const index = 0;

 a_1[index] = 3;
 a_2[index] = 3;
console.assert(a_1 === a_2);

 b_1[index] = 5;
 b_2[index] = 5;
console.assert(b_1 !==  b_2);
```

__Fill in the Blanks__  
[on pytut](http://www.pythontutor.com/javascript.html#code=let%20arr_1%20%3D%20%5B0,1,2%5D%3B%0Alet%20arr_2%20%3D%20%5B0,1,2%5D%3B%20%0Aconsole.assert%28arr_1%20!%3D%3D%20arr_2%29%3B%0Aconsole.assert%28arr_1%5B1%5D%20%3D%3D%3D%20arr_2%5B1%5D%29%3B%0A%0Alet%20key%20%3D%200%3B%0Aconsole.assert%28arr_1%5Bkey%5D%20%3D%3D%3D%20arr_2%5Bkey%5D%29%3B%0A%0A%20arr_1%5Barr_2%5B2%5D%5D%20%3D2%20%3B%20//%20write%20this%20line%0A%20arr_2%5Barr_1%5B2%5D%5D%20%3D2%3B%20//%20write%20this%20line%0Aconsole.assert%28arr_1%5Barr_2%5B2%5D%5D%20%3D%3D%3D%20arr_2%5Barr_1%5B2%5D%5D%29%3B%0A%0Alet%20arr_3%20%3D%5B0,1,1%5D%3B%20//%20write%20this%20line%0A%20%20arr_1%20%3Darr_2%20%20%3B%20//%20write%20this%20line%0Aconsole.assert%28arr_1%20%3D%3D%3D%20arr_2%29%3B%0Aconsole.assert%28arr_3%20!%3D%3D%20arr_1%29%3B%0Aconsole.assert%28arr_3%20!%3D%3D%20arr_2%29%3B%0Aconsole.assert%28arr_3%5Bkey%5D%20%3D%3D%3D%20arr_1%5B0%5D%29%3B%0A%0A%20let%20obj_2%20%3D%20%5B1,%202%5D%3B%0A%20let%20obj_3%20%3D%20%5B0,%201%5D%3B%20%0Aconsole.assert%28obj_3%5B1%5D%20%3D%3D%3D%20obj_2%5Bkey%5D%29%3B&curInstr=18&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
let arr_1 = [0,1,2];
let arr_2 = [0,1,2];       
console.assert(arr_1 !== arr_2);
console.assert(arr_1[1] === arr_2[1]);

let key = 0;
console.assert(arr_1[key] === arr_2[key]);

 arr_1[arr_2[2]] =2; 
 arr_2[arr_1[2]] =2; 
console.assert(arr_1[arr_2[2]] === arr_2[arr_1[2]]);

let arr_3 =[0,1,1];  
   arr_1 =arr_2  ; 
console.assert(arr_1 === arr_2);
console.assert(arr_3 !== arr_1);
console.assert(arr_3 !== arr_2);
console.assert(arr_3[key] === arr_1[0]);

let obj_2 = [1, 2];
let obj_3 = [0, 1]; 
console.assert(obj_3[1] === obj_2[key]);
```

[TOP](#reference-type-exercises)

---

## Object Exercises

__Complete the Assertions__  
[on pytut](http://www.pythontutor.com/javascript.html#code=let%20a_1%20%3D%20%7B%7D%3B%0Alet%20a_2%20%3D%20a_1%3B%0Aconsole.assert%28a_1%20%3D%3D%3D%20a_2%29%3B%0A%0Alet%20b_1%20%3D%20%7B%7D%3B%0Alet%20b_2%20%3D%20%7B%7D%3B%0Aconsole.assert%28b_1%20!%3D%3D%20%20b_2%29%3B%0A%0A//%20---%0A%0A%20a_1.x%20%3D%203%3B%0A%20a_2.x%20%3D%203%3B%0Aconsole.assert%28a_1%20%3D%3D%3D%20a_2%29%3B%0A%0A%20b_1.x%20%3D%205%3B%0A%20b_2.x%20%3D%205%3B%0Aconsole.assert%28b_1%20%3D%3D%3D%20b_2%29%3B&curInstr=11&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
let a_1 = {};
let a_2 = a_1;
console.assert(a_1 === a_2);

let b_1 = {};
let b_2 = {};
console.assert(b_1 !==  b_2);

// ---

let a_1.x = 3;
let a_2.x = 3;
console.assert(a_1 ===  a_2);

let b_1.x = 5;
let b_2.x = 5;
console.assert(b_1  !==  b_2);
```

__Complete the Assertions__  
[on pytut](http://www.pythontutor.com/javascript.html#code=%20%20let%20a_1%20%3D%20%7B%7D%3B%0A%20%20let%20a_2%20%3D%20a_1%3B%0A%20%20console.assert%28a_1%20%3D%3D%3D%20a_2%29%3B%0A%0A%20%20let%20b_1%20%3D%20%7B%7D%3B%0A%20%20let%20b_2%20%3D%20%7B%7D%3B%0A%20%20console.assert%28b_1%20!%3D%3D%20b_2%29%3B%0A%0A%20%20//%20---%0A%20%20%0A%20%20const%20key%20%3D%20%22x%22%3B%0A%0A%20%20%20a_1%5Bkey%5D%20%3D%203%3B%0A%20%20%20a_2%5Bkey%5D%20%3D%203%3B%0A%20%20console.assert%28a_1%20%3D%3D%3D%20a_2%29%3B%0A%0A%20%20%20b_1%5Bkey%5D%20%3D%205%3B%0A%20%20%20b_2%5Bkey%5D%20%3D%205%3B%0A%20%20console.assert%28b_1%20!%3D%3D%20b_2%29%3B&curInstr=13&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
let a_1 = {};
let a_2 = a_1;
console.assert(a_1 === a_2);

let b_1 = {};
let b_2 = {};
console.assert(b_1  !== b_2);

// ---

const key = "x";

let a_1[key] = 3;
let a_2[key] = 3;
console.assert(a_1 === a_2);

let b_1[key] = 5;
let b_2[key] = 5;
console.assert(b_1 !== b_2);
```

__Fill in the Blanks__  
[on pytut](http://www.pythontutor.com/javascript.html#code=let%20obj_1%3D%7B%7D%3B%0Alet%20obj_2%3D%7B%7D%3B%0Aconsole.assert%28obj_1%20!%3D%3D%20obj_2%29%3B%0Aconsole.assert%28obj_1.x%20%3D%3D%3D%20obj_2.x%29%3B%0A%0Alet%20key%20%3D%20%22y%22%3B%0Aconsole.assert%28obj_1%5Bkey%5D%20%3D%3D%3D%20obj_2%5Bkey%5D%29%3B%0A%0A%20obj_1%5Bkey%5D%3B%0A%20obj_2%5Bkey%5D%3B%0Aconsole.assert%28obj_1%5Bobj_2.y%5D%20%3D%3D%3D%20obj_2%5Bobj_1.y%5D%29%3B%0A%0Alet%20%20obj_3%20%3D%20%5Bkey%5D%3B%0A%20%20obj_1%20%3Dobj_2%3B%20%0Aconsole.assert%28obj_1%20%3D%3D%3D%20obj_2%29%3B%0Aconsole.assert%28obj_3%20!%3D%3D%20obj_1%29%3B%0Aconsole.assert%28obj_3%20!%3D%3D%20obj_2%29%3B%0Aconsole.assert%28obj_3%5Bkey%5D%20%3D%3D%3D%20obj_1.y%29%3B%0A%0A%20%20obj_3.x%20%3D%20obj_2%5Bkey%5D%3B%0Aconsole.assert%28obj_3.x%20%3D%3D%3D%20obj_2%5Bkey%5D%29%3B&curInstr=17&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
 let obj_1={};
 let obj_2={};
console.assert(obj_1 !== obj_2);
console.assert(obj_1.x === obj_2.x);

let key = "y";
console.assert(obj_1[key] === obj_2[key]);

obj_1[key];
obj_2[key];  
console.assert(obj_1[obj_2.y] === obj_2[obj_1.y]);

let  obj_3 = [key];
obj_1 =obj_2; 
console.assert(obj_1 === obj_2);
console.assert(obj_3 !== obj_1);
console.assert(obj_3 !== obj_2);
console.assert(obj_3[key] === obj_1.y);

obj_3.x = obj_2[key];
console.assert(obj_3.x === obj_2[key]);
```

[TOP](#reference-type-exercises)

---

## Comparison Exercises

__Swap 'em__  
[on pytut](http://www.pythontutor.com/javascript.html#code=const%20obj%20%3D%20%7Bprop%3A%20%22array%22%7D%3B%0Aconst%20arr%20%3D%20%5B%22object%22%5D%3B%0Alet%20_%20%3D%20null%3B%0A%0A//%20swap%20the%20values%20stored%20in%20each%20structure%0A_%20%3D%20arr%5B0%5D%3B%0Aarr%5B0%5D%3Dobj.prop%3B%0Aobj.prop%3D%20_%3B%0A//%20%20using%20dot%20notation%20for%20the%20object%0A_%20%3D%20obj.prop%3B%0Aobj.prop%3Darr%5B0%5D%3B%0Aarr%5B0%5D%3D_%3B%0A//%20%20using%20direct%20access%20for%20the%20array%0A&curInstr=9&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
const obj = {prop: "array"};
const arr = ["object"];
let _ = null;

// swap the values stored in each structure
_ = arr[0];
arr[0]=o;bj.prop;
obj.prop= _;
//  using dot notation for the object
//  using direct access for the array
_ = obj.prop;
obj.prop=arr[0];
arr[0]=_;

```

__Swap 'em__  
[on pytut](http://www.pythontutor.com/javascript.html#code=const%20obj%20%3D%20%7Bprop%3A%20%22array%22%7D%3B%0Aconst%20arr%20%3D%20%5B%22object%22%5D%3B%0Alet%20_%20%3D%20null%3B%0A%0A//%20swap%20the%20values%20stored%20in%20each%20structure%0A//%20%20using%20bracket%20notation%20for%20the%20object%0A//%20%20using%20variable%20access%20for%20the%20array%0Aconst%20obj_key%20%3D%20prop%3B%0Aconst%20arr_index%20%3D0%20%3B%0A%0A_%3D%20arr%5Barr_index%5D%3B%0Aarr%5Barr_index%5D%3Dobj%5Bobj_key%5D%3B%0Aobj%5Bobj_key%5D%3D_%3B&curInstr=4&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
const obj = {prop: "array"};
const arr = ["object"];
let _ = null;

// swap the values stored in each structure
//  using bracket notation for the object
//  using variable access for the array
const obj_key =prop ;
const arr_index = 0;

_= arr[arr_index];
arr[arr_index]=obj[obj_key];
obj[obj_key]=_;

```

__Relative vs Absolute__  
[on pytut](http://www.pythontutor.com/javascript.html#code=//%20array%20indices%20are%20relative%0Aconst%20arr%20%3D%20%5B%22a%22,%20%22b%22%5D%3B%0Aconst%20index%20%3D%200%3B%0A%0Aconst%20read_arr_1%20%3D%20arr%5Bindex%5D%3B%0Aarr.shift%28%29%3B%20//%20removes%20the%20first%20item%0Aconst%20read_arr_2%20%3D%20arr%5Bindex%5D%3B%0A%0Aconsole.assert%28read_arr_1%20!%3D%3D%20%20read_arr_2%29%3B%0A%0A//%20object%20keys%20are%20absolute%0Aconst%20obj%20%3D%20%7Bx%3A%20%22a%22,%20y%3A%20%22b%22%7D%3B%0Aconst%20key%20%3D%20%22y%22%3B%0A%0Aconst%20read_obj_1%20%3D%20obj%5Bkey%5D%3B%0Adelete%20obj.x%3B%0Aconst%20read_obj_2%20%3D%20obj%5Bkey%5D%3B%0A%0Aconsole.assert%28read_obj_1%20%3D%3D%3D%20read_obj_2%29%3B&curInstr=11&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)  
```js
// array indices are relative
const arr = ["a", "b"];
const index = 0;

const read_arr_1 = arr[index];
arr.shift(); // removes the first item
const read_arr_2 = arr[index];

console.assert(read_arr_1 !== read_arr_2);

// object keys are absolute
const obj = {x: "a", y: "b"};
const key = "y";

const read_obj_1 = obj[key];
delete obj.x;
const read_obj_2 = obj[key];

console.assert(read_obj_1 ===  read_obj_2);
```

[TOP](#reference-type-exercises)

---

## Nesting

-> coming in week 3


[TOP](#reference-type-exercises)

___
___
### <a href="http://janke-learning.org" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/50098409-22575780-021c-11e9-99e1-962787adaded.png" width="40" height="40"></img> Janke Learning</a>
