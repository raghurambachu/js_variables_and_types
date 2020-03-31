1. In code below "Mark" is a string. What is name?

```js
var name = "Mark";
//Answer : `name` is a variable
```

2. Find the error if any

```js
  var product cost = 3.45;
  // Answer : There should be no space between the words.
  //var product_cost = 3.45 would have been the right declaration.
```

3. Write `Right or Wrong` next to the code below.

```js
  "Hello World" 
  'Hello World" 
  "Hello World' 
  'Hello World'
```
<!-- right wrong wrong right -->

## Write `VALID` and `INVALID` infront of the variable name defined below

```js
var man;        //valid 
var 1girl;      //invalid
var woman3;     //valid
var -girl;      //invalid
var blackDog;   //valid
var 42;         //invalid
var $42;        //valid
var userName;   //valid
var x, y, z;    //valid
var x = 5, y = 6, z = 7;    //valid
var x = 5 + 10 + 2;         //valid
var user = "Tyrion"; "Arya"; "John"; //invalid
```

## Basic Operations

Mathematical Operations:

Solve this using mathematical operations. (+, -, \*, / , etc)

```js
var amount = 2080;
// Define a new variable and store the value that is 80 less then the value of amount.
var decreasedAmount = amount - 80;

// Define a new variable and store the value that is 200 more then the value of amount.
var increasedAmount = amount + 20


// Define a new variable and store the value that is 4 times the value of amount.
var multipliedAmount = 4 * amount;

// Define a new variable and store the reminder when the value of amount is  divided by 21.
```
var remainderAmount = amount % 21;

## var, let and const

Write down the code or if there is any error write down the error.

```js
var user = "Sameer";
// Reassign the value of user to "Sam"
// Define a variable with name user with value "Irfan"
// Answer :
user = "Sam"
var user = "Irfan"
//In case we use "use 'strict'" then it is not possible to redeclare a variable, it will throw an error.

let number = 21;
// Reassign the value of number to 60
// Define another variable called number with the value of 100
//Answer :
number = 60;
//We cannot redeclare a new variable with same name that is number. We will get "Uncaught SyntaxError: Identifier 'number' has already been declared "


const username = "Admin";
// Reassign the value of username to "Arya"
// Define a variable called usernae with value "John"
//Answer : const variable cannot be reassigned. Nor can they be redeclared. If it's being reassigned it will give "Uncaught TypeError: Assignment to constant variable. ".And on trying to redeclare the variable with const will lead to "Uncaught SyntaxError: Identifier 'username' has already been declared "
```

Logical Operation:

Solve this using logical operations. (<, >, &&, ||)

```js
var johnAge = 45;
var markAge = 35;

// Check who is older eithe John or Mark 
johnAge > markAge

// Check who is younger
markAge < johnAge

// Check if their age is equal
markAge === johnAge

// Create a new variable and assign the age of john to new variable.
var age = johnAge;

// Check if john is equal to or greater then mark.
johnAge >= markAge

// Check if john is less then or equal to mark.
johnAge <= markAge 

// Calculate the average age of john and mark and assign to a new variable.
var averageAge = (johnAge + markAge)/2
```

Output of the following and why :

```js
let charactor = "Arya";
charactor = "John";
console.log(typeof charactor);
// "String" because the typeof gives type of the value stored in.
```

Output of the following and why :

```js
let charactor = "Arya";
console.log(typeof charactor);
charactor = 10;
//"String" because the typeof gives type of the value stored in. And the charactor is reassigned after the output is printed. If console.log() was after the last reassignment, then typeof would be "Number"
```

valid or not (why)

```js
null = 10;
console.log(null);
//The above statement null = 10 is invalid, firstly null is a datatype and it is used in as a value to an variable, secondly even if we used a variable declaration like var null =10, even this would fail because null is a reserved keyword and new variables using reserved keywords cannot be declared.
```
