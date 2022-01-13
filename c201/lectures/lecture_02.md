## if else
```
if(somethingEvaluatesTrue){
  do something
}
else if(somethingEvaluatesTrue){
    do this thing
}
else "no conditon needed {
  do this if all not true
}

```

```js
'use strict'; // must have
let isTrue = true;
let isFalse = false;

if(isTrue){
    console.log('code worked');
} else {
    console.log('naaaaa')
}
```

```js
'use strict'; // must have
let isTrue = true;
let isFalse = false;

if(isTrue){
    console.log('code worked');
} else if (isfalse) {
    console.log('naaaaa');
} else {
    console.log('runn');
}
```

### Comparison Operators
 - === striclty equals
 - == comparitvl;y equals
    ```
    let a = 5;
    console.log(a == '5');
    is true
    ```
- != not equal to
- !== striclty not true


### Logical Operators
- && - and
- || - or
- ! - not

```js
let isTrue = true;
let isFalse = false;

if(isTrue && !isTrue){
  console.log('both will run'); // if will not run
}

```
## git and github

A- add 

C- commit - meaningful msg

P- push

## Arrays **special type of Object**
 - a list or collection of elements
   - can be anything 
 - no predetermine size
 - -Every elements has a index(location ref)
 - zero based
   - first element in Array is index at 0
 - have built in methods
   - .push(),.pop(),includes()
 - properties- returns us values
   - lengths

```js
use 'strict'

let myArr = [1, 'hello', [2,3], true];
// prints Array contents
console.log(myArr);
// creates table with Array elements
console.table(myArr);
// pull index elements
console.log(myArr[0]);
// pull index elements form nested array
console.log(myArr[2][0]);
```

```js
let favBoyBands = ['bts', 'Backsteat boys', 'NSYNC', '98 Degreas'];
console.table(favBoyBands);

// change varibles in index
let nsync = favBoyBands[2];

// check array length
let arrLength = favBoyBands.length;
console.log(arrLength);

// accessing last item
console.log(favBoyBands[favBoyBands.length-1]);

//getting length of inner array
console.log(myArr[2].length);

// add to Arrays
myArr[4] = false;
// gives undefined for all index between 4 and 10
myArr[10] = 'yes';
console.log(myArr);

// built in methods for array

//adds to end of array
// much easier to use
favBoyBands.push('Boys to Men');

// removes last element out of array
favBoyBands.pop();
// can set to a variable
favBoyBands.pop();
let items = favBoyBands();

// use console for arrays
```

## for while loops

```js
'use strict'

// for loops
// do something a certian amount of times
// great for iterating through/ over arrays

 //for(starting val; condition; increment){
//  code block
//}

// looping though array
let arrayName
let userName // assign global variable 1

for(let i =0; i < students.length; i++){
    console.log(students[i]);
    // using if statment to add condition
    if(student[i] === 'Steve'){
        console.log('hay steve')
        //use as variable
        // make sure to assign global variable 1
        userName = student[i];
    }
}
```

## while loops
```js
//while(condition){
   // do something
// }

let myNum = 3;

let userNum = prompt('What number am I thinking of');

while( userNum != mynum){
    userNum = prompt('try again');
}

```
breaking while loop - guessing game
```js
let clueGuesses = 20
let suspect = 'Nicholas'
let foundsuspect = false;

while(clueGuesses && !foundsuspect)
    // use a prompt
    console.log(`it was ${userInput}`);
    clueGuesses--;
    if(userInput === suspect){
        foundsuspect = true;
    }
```

```js

// keeping score

let score = 0;

//add 
score++ to question logic