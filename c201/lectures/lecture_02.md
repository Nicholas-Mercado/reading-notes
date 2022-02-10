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

## Class_07

### Constructor

- a function that create object instance
- Uses parameters to assign properties
- Name starts with Capitol letter

```js

function Student(name, pronouns) {
  this.studentName = name;
  this.pronouns = pronouns;
  //can hardcode
  this.currentClass = 'c201';
  //add methods
  this.greetClass = function(){
    console.log('yo');
  }
  //add student to array
  student.all.push(this)
}

// add student objects to a array global
Student.all = []
// create student object

let lauren = new Student('lauren', 'they/them');

//call function 
lauren.greeClass();

//call student array
console.log(student.all);

```

### Protoytpe inharadence

```js
// keyword inharet
Student.Protoytpe.greetClass = function (){
  console.log('hey!');
}
```

### refactore

```js
let kittenSection = document.getElementById('profile');

const kittenCaboodle = [];

// the order of the argument is important for instantiation 
function Kitten(name, interests,isGoodwithDogs,isGoodwithkids,isGoodwithCats,photo){
// use this for same everytime
this.name = name;
this.interest = interest;
this.isGoodwithDogs = isGoodwithDogs;
this.isGoodwithkids = isGoodwithkids;
this.isGoodwithCats = isGoodwithCats;
this.age = null;
this.photo = photo;
//connect array
kittenCaboodle.push(this);
}

// adding methods via Protoytpe
Kitten.Protoytpe.getAge = function() {
  this.age = `${randomAge(3,12)} months`;
};

// instantiate
// add 
let frankie = new Kitten('frankie', interests,isGoodwithDogs,isGoodwithkids,isGoodwithCats,photo)
let Sarah = new Kitten('frankie', interests,isGoodwithDogs,isGoodwithkids,isGoodwithCats,photo)
let bill = new Kitten('frankie', interests,isGoodwithDogs,isGoodwithkids,isGoodwithCats,photo)
```

```js
//refactor render

kitten.Protoytpe.renderKitten = function() {
  // make sure to change kitten

  //change for loop render call
  currentKitten.renderKitten();
}
```

### Tables

```js

//steps
// 2nd- Create element
// 3rd give element context
// 4th append the dom

//adding table to js

const TableElem = document.createElement('table'); //creates table
articleElem.appendChild(tableElem);

const tableHeadElem = document.createElement('thread'); //creates thread
tableElem.appendChild(tableHeadElem);

const row1 = document.createElement('tr');
tableHeadElem.appendChild(row1);

//adding contents
const th1Elem = document.createElement('th');
th1Elem.textContent = 'good with dogs'; // hardcode title
row1.appendChild(th1Elem);
const th2Elem = document.createElement('th');
th2Elem.textContent = 'good with cats'; // hardcode title
row1.appendChild(th2Elem);
const th3Elem = document.createElement('th');
th3Elem.textContent = 'good with Kids'; // hardcode title
row1.appendChild(th3Elem);

// add row 2

const row2 = document.createElement('tr'); // chrome takles care of this
tableElem.appendChild(row2);

const td1 = document.createElement('td');
td1.textContent= this.isGoodwithDogs; // connect to object
row2.appendChild(td1);



//HJerader is store hours
```

## Class_09

### Events

- asynchronous code- runs out of order

```js

element.addEventListener('event', callback function);

// callback function = function that is passed in as a argument to anther function

buttun.addEventListener('submit',handleSubmit);

```

```js

// step one grab teh element that we want to listen though

//step three Define our event handler- callback funtion


// add evetlistener - 2 args (event, callback function)
myContainer

```

#### Build a fomr HTml

```js

<form id="my-form">
//  default box around 
  <fieldset>
  // basic info in legend
    <legend>Context</legend>
    // inputs
    // label for and id must match
    //type controls input style
    <label for="name"></label>
    // can use type number or type etc..
    // use name="" attribute for targeting
    <input id="name" type="text" name="Firstname">

  // Second input style nested
  <label>age
  // not need for for=
  <input type="number" name="age">
  </label>

  // adding options
  <label>fave housewaives</label>
  <select name="housewives" id="housewives">
  <options value="">----Please Choose---</options>
  <options value="choice"></options>
  <option>
  </fieldset>
  // must be in fomr
  <button type="submit"></button>
</form>


```

```js

function handleSubmit(event){
  event.preventDefault();
// target name= "value"<---
  let name = event.target.firstName.value;

  let age = event.target.age.value;

  let housewives = event.target.housewives.value;
}

myContainer.addEventListener('click', handleClick);

myForm.addEventListener('submit', handleSubmit);

```

#### build form

```html

// constructor argumetsn in order

//name, interests,isGoodwithDogs,isGoodwithkids,isGoodwithCats,photo

<form id="add-store">
  <fieldset>
    <legend>basic info</legend>

    <label for ="name">Name</label>
    <input id="name" type="text" name="storeName">

    <label for="interest">Name (seperate by comma)</label>
    <input id="interest" type="text" name="interest">
    
  </fieldset>
  <button type="submit">Submit</button>
</form>
```

//step three Define our event handler- callback funtion

```js

// / step one grab teh element that we want to listen though

const kittenform = document.getElementById('add-kitten');

// add evetlistener - 2 args (event, callback function)

kittenform.addEventListener('submit', handleSubmit);

//step three Define our event handler- callback funtion

funtion handleSubmit(){
  event.preventDefault(); // stop sending data off
 /// now parseint()
  let name = event.target.storeName.value;
  //adding array
  let interest = event.target.interest.value;
// use split to seperate with comma into array
// split argument is what you want split on comma, space, letter
  interest = interest.split(',')
  // How to do checkboxes
let isGoodwithCats = event.target.isGoodwithCats.checked;

// use constrotor

let newKitten = new Kitten(name, interest, isGoodwithDogs,isGoodwithCats,isGoodwithkids,photo);
/// make sure to add all functions that are stand alone
newKitten.getAge();
newKitten.renderKittens();
//resets form
kittenform.reset();
}
```

## Class_11

### Css Grid

- must be in a Container

- parent element must have display: grid;

```css

.grid-Container{

  display: grid;


}

```

### busmail

What we need

#### Global variables

#### constructor

#### Executable

- number of votes user has sumbited



### Local Storage

```js



// what data do i want to persist
//Where do you want to grab

function handleResults(event) {
  if (totalRounds === 0) {
    renderChart();
  }
// *****LOCACL STORAGE********?
// step one - stringinfy data

let stringAllItems = JSON.stringinfy(allItems);

// step two Set the Item in Storage

localStorage.setItem('items',stringAllItems);
}

// step three get items back from local Storage
// parse the JSON

let retrieveItems = localStorage.getItem('items');

let parsedItems = JSON.parse(retrieveItems);

// or one listen

// let parsedItems = JSON.parse(retrieveItems);

// Step four If i have items in LS use those,  if not instantiate new items

if(retrieveItems){
allItems = parsedItems;
   }else{
   
    new Item('bag');
    new Item('banana');
    new Item('bathroom');
    new Item('boots');
    new Item('breakfast');
    new Item('bubblegum');
    new Item('chair');
    new Item('cthulhu');
    new Item('dog-duck');
    new Item('dragon');
    new Item('pen');
    new Item('pet-sweep');
    new Item('scissors');
    new Item('shark');
    new Item('sweep', 'png');
    new Item('tauntaun');
    new Item('unicorn');
    new Item('water-can');
    new Item('wine-glass');
  
}


console.log(allItems);
```

## Lab14

```js

