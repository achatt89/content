# Arrays
author: alexjmackey

levels:

  - beginner

type: normal

inAlgoPool: false

category: must-know

---
## Content

Arrays are an important concept in JavaScript and used frequently.
 
Declaring an array:
```
var myArray = [1,2,3];
var anotherArray =["a","b","c"];
```

Array's are *zero based/indexed* so if you want to retrieve the first value you use 0 as the index parameter:

```
console.log(myArray[0]);
```

We can retrieve the last value of an array by using the *length* property and subtracting 1 from it (don’t use this on an empty array!)

```
var arrayLength=myArray.length;
var lastVal= myArray[arrayLength-1];
console.log(lastVal);
```

Values can be added to the array with the *push* method which returns the new length of the array:
```
myArray.push(4); //4
myArray.push(5,6,7); //7
```
Or the last item can be returned and removed using *pop*:
```
myArray.pop();
```
You can find the position of any item with the *indexOf* operator:
```
var pos = myArray.indexOf(3);//2
```
We can loop over all the array items with *forEach*:
```
myArray.forEach(
function (item, index, array) {
  console.log(item, index);
}
);
```

---
## Practice

How would you get the last value in the `myArray` array?
```
var myLength = myArray.???
var last = ???[??? ???];
```
*`length`
*`myArray`
*`myLength`
*`-1`
*`+0`
*`+1`
*`array`
*`[0]`
*`.getLast`
*`.tail`

---
## Revision

Fill the gaps such that you get the first element of `enkiArray`:
```
var enkiArray = [1, 2, 3];
var firstElement = ??????;
```

*`enkiArray`
*`[0]`
*`[1]`
*`array`
*`getLast()`
*`getFirst()`
*`push`
*`pop`