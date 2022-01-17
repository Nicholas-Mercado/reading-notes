# Lecture notes

## Class_02

### if-else

```js
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

#### Comparison Operators

- === striclty equals
- == comparitvl;y equals

```js
let a = 5;
console.log(a == '5');
is true
```

- != not equal to
- !== striclty not true

#### Logical Operators

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

### git and github

A- add

C- commit - meaningful msg

P- push

### Arrays **special type of Object**

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

### for while loops

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

### while loops

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
```

### Class_04 Functions

parameter = bucket
arguments = stuff in bucket

```js

'use strict';

// function declaration

//define
function greeting(){
  console.log('heu');
}

//call
greeting();

// function expressions
// flaw. cant call before this function
// look up hosting
let greeting = function(){
      console.log('hey');
}

function newGreeting(firstName, lastName){
  console.log(`hey!${firstName}${lastName}`);
}

// invoke with arguments
newGreeting('nick', 'mercado');

// take in array
function multi(arr){
  for(let i = 0; 1<array.lengths; i++)
  console.log(arr[i])
}

//functions with retun
functions multi(a,b){
  retun a *b;
}

let result = multi(6,8);

```

### Arguments

```js
// must give all arguments
functions sub(a,b){
  retun a - b;
}
functions multi(a,b){
  retun a * b;
}

let result1 = multi(6,8);
let result2 = sub(6,8);

console.log(result1,result2);
```

### Scope

```js
function newGreeting(firstName, lastName){
  let message = (`hey!${firstName}${lastName}`);
  return message;
  //this wont work cause its not declared globally
}
```

### Css

#### positioning

2 types

- static-type

- relative-type

  -

  -

## Class_05

### Functions and returns

```js

//Multi returns

function newDev(){
  let firstName = 'nick';
  let lastName = 'mercado';

  return [firstName, lastName];\
}

let dev = newDev();
// access arry for names
let fname = newDev()[0];
let Lname = newDev()[1];

// group function calls adding to variable
// called destructing

let [fName, Lname] = newDev();
// array is assign to each var in order

```

#### Branching

Create a new Branch

```git

1. git checkout -b <branch name>

2. ACP- add commit are the same, push is different(git push origin <branch name>)

3. pull request- on github (pull into main) if no conflicts

4. git checkout main (scary) 

5 git pull origin main

```

## Class_06

### Objects

```js
'use strict'

let audrey = {
  name: 'Nick',
  positon: 'student',
  age: 35,
  isremote: true,
  course: '201d82',
  says: function() {
    console.log('yea yea yea');
  },
  classIntro; function() {
    console.log(`hello ${this.course}`);
  }
};
// add to object
Nick.interests = ['art','food',];
// use push() to add to the end of a key
Nick.interests.psuh('money');

// use chaining adds function to object
Nick.advise = function() {
  console.log('help!')
}

//accessing 
console.log(Nick.name);
console.log(Nick['course']); 

// Calling methods
Nick.classIntro();
Nick.advise();
```

Objects are not iterable. No for loops.

## THE DOM

```js
//shows dom tree
console.dir(document)

// minipulate the
document.body.innertext

```

## dom practice

```js
// use generate this from js:
<section id="profile"></section>

let frankie = {
  name: "Frankie",
  //assign null when using function later
  age: null,
  interests: ['wet food', 'cat food'];
  isGoodwithDogs: false,
  isGoodwithkids: true,
  isGoodwithCats: true,
  photo: 'img/frankie.jpg',
  getAge: function(){
    this.age = `${randomAge(3,12)} months`; 
  }

};

// use generate this from js:
<section id="profile"></section>

let jumper = {
  name: "Jumper",
  //assign null when using function later
  age: null,
  interests: ['dry food', 'dog food'];
  isGoodwithDogs: false,
  isGoodwithkids: false,
  isGoodwithCats: false,
  photo: 'img/frankie.jpg',
  getAge: function(){
    this.age = `${randomAge(3,12)} months`; 
  }

};

// use generate this from js:
<section id="profile"></section>

let serena = {
  name: "Serena",
  //assign null when using function later
  age: null,
  interests: ['mice', 'lazers','scratching'];
  isGoodwithDogs: true,
  isGoodwithkids: false,
  isGoodwithCats: false,
  photo: 'img/frankie.jpg',
  // use this to add random age to age: key
  getAge: function(){
    this.age = `${randomAge(3,12)} months`; 
  }

};

// use helper function for age plus random number generator
function randomAge(min, max){
  let number = return Math.floor(Math.random() * (max - min) + min);
  return number;
}

frankie.getAge();
Serena.getAge();
Jumper.getAge();

// instead of calling each use a helper function
// build array
const kittenCaboodle = [frankie, jumper, Serena];
function getAllKittenAges() {
  for(let i = 0; i < kittenCaboodle.length; i++){
    let currentKitten = kittenCaboodle[i];
    currentKitten.getAge();
  }
}
//call out kitten age helper function
getAllKittenAges();

```

### Dom manipulation

```js
//steps
// 2nd- Create element
// 3rd give element context
// 4th append the dom



// 1- grab a window into the Dom
let kittenSection = document.getElementById('profile');

// write function to render kittens to page

function renderKitten(kitten) {
  //2 create element
  const articleElem = document.createElement('article');
  // 4 append the dom
  kittenSection.appendChild(articleElem);

  const h2Elem = document.createElement('h2');
  h2Elem.textContent = kitten.name;
  articleElem.appendChild(h2Elem);
//create p tage
  const pElem = document.createElement('p');
  pElem.textContent = `${kitten.name} is adorable and is ${kitten.age} old`;
  articleElem.appendChild(pElem);

// create ul
  const ulElem = document.createElement('ul')
  articleElem.appendChild(ulElem);
// create li use for loop to array list
  for(let i=0; i <kitten.interest.length; i++);{
  let currentInternets = kitten.interest[i];
  const liElem = document.createElement('li');
  liElem.textContent = currentInternets;
  ulElem.appendChild(liElem);
  }
  //create img
  const imgElem = document.createElement('img');
  // this works with dom beacuse phot seen as object
  imgElem.src = kitten.photo;
  // set arrLength
  imgElem.alt = (`${kitten.name} is adorable and is ${kitten.age} old`);
  //append
  articleElem.appendChild(imgElem)

}

//Create helper function to render all kittens

function renderAllKittens(){
  for(let i = 0; i < kittenCaboodle.length; i++){
    let currentkitten = kittenCaboodle[i];
    renderkitten(currentkitten);
  }
}

renderkitten();

<h3><a"for somethingEvaluatesTrue></h3>

// let hours = global array
let hours = [12,1,2,3,4..]
//object
let seattle = {
  minCust:23,
  maxCust:65,
  avgCookie: 6.3;
}
```