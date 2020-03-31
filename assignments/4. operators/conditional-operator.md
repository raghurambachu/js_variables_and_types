## If Statement
1.  🎖Make a simple calculator with these functions. Using prompt, type conversion, if else statement. Use prompt to take the input from user i.e two numbers and an operation (Add, Sub, Mul, Div).

  ⛑ Rule
    * [ ] While substracting and dividing keep in mind the number one should be greater then number two. If not show alert saying `Number Two is larger then Number one`.
  ⚡️ Operations
    * [ ] Add
    * [ ] Sub
    * [ ] Mul
    * [ ] Div

let operation = prompt("Enter the operation you want to perform ?");
if (
  operation === "Add" ||
  operation === "Sub" ||
  operation === "Mul" ||
  operation === "Div"
) {
  let input1 = +prompt("Enter the First Number");
  let input2 = +prompt("Enter the Second Number");
  let result;
  if ((operation === "Sub" || operation === "Div") && input1 < input2) {
    alert(
      "For Subtraction and Division the First Number should be larger than the Second Number"
    );
  } else {
    if (operation === "Add") {
      result = input1 + input2;
    } else if (operation === "Sub") {
      result = input1 - input2;
    } else if (operation === "Mul") {
      result = input1 * input2;
    } else {
      result = input1 / input2;
    }
    console.log(result);
  }
} else {
  alert(
    operation +
      "cannot be performed by the calculator. Please Enter valid operations ie 'Add', 'Sub','Mul','Div'"
  );
}

2. 🎖Write a if else statement which checks if the status is single `console.log` the message `John is single` or else `John is married`
```js
var firstName = 'John';
var status = 'single';
// Your code goes here
```
var firstName = "John";
var status = "married";
if(status === "single"){
  console.log(firstName + " is single")
}else{
  console.log(firstName + " is married")
}


3. 🎖Write a JavaScript program that takes two `integers` from user (using prompt) and alerts the larger number.
```js
// your code goes here
```
let number1 = +prompt("Enter the first integer");
let number2 = +prompt("Enter the second integer");
if(isNaN(number1) || isNaN(number2)){
  alert("Please enter valid integers.")
}else{
  let larger;
  if(number1 > number2){
    larger = number1;
  }else if(number2 > number1){
    larger = number2
  }else{
    larger ="Inputted integers are equal. Neither of them is larger."
  }
  alert(larger);
}


4. 🎖Write a JavaScript conditional statement to find the sign (+, -) of product of three numbers. Take those three numbers from user using `prompt`. Display an alert box with the specified sign.

```js
// Your code goes here
```
// +++ +
// ++- -
// +-+ -
// +-- +
// -++ -
// -+- +
// --+ +
// --- -

let inputNum1 = +prompt("Enter the first number","");
let inputNum2 = +prompt("Enter the second number","");
let inputNum3 = +prompt("Enter the third number","");
if (
  (inputNum1 > 0 && inputNum2 > 0 && inputNum3 > 0) ||
  (inputNum1 > 0 && inputNum2 < 0 && inputNum3 < 0) ||
  (inputNum1 < 0 && inputNum2 > 0 && inputNum3 < 0) ||
  (inputNum1 < 0 && inputNum2 < 0 && inputNum3 > 0)
) {
  alert("The sign of the resultant multiplication would be" + " + positive");
} else {
  alert("The sign of the resultant multiplication would be" + " - negative");
}



## Switch Statement

1. 🎖Using switch statement do the following

Take a number value from user and alert the message if it matches the conditions.
* [ ] ONE, if `number` is equal to 1.
* [ ] TWO, if `number` is equal to 2.
* [ ] THREE, if `number` is equal to 3.
* [ ] FOUR, if `number` is equal to 4.
* [ ] FIVE, if `number` is equal to 5.
* [ ] SIX, if `number` is equal to 6.
* [ ] SEVEN, if `number` is equal to 7.
* [ ] EIGHT, if `number` is equal to 8.
* [ ] NINE, if `number` is equal to 9.
* [ ] PLEASE TRY AGAIN, if  is none of the above.
```js
// Your code goes here
```

let userInput = +prompt("Put some number in between 1 to 9");
let numberAlert;
switch(userInput){
  case 1:
    numberAlert = "ONE";
    break;
  case 2:
    numberAlert = "TWO";
    break;
  case 3:
    numberAlert = "THREE";
    break;
  case 4:
    numberAlert = "FOUR";
    break;
  case 5:
    numberAlert = "FIVE";
    break;
  case 6:
    numberAlert = "SIX";
    break;
  case 7:
    numberAlert = "SEVEN";
    break;
  case 8:
    numberAlert = "EIGHT";
    break;
  case 9:
    numberAlert = "NINE";
    break;
  default:
    numberAlert = "PLEASE TRY AGAIN";
}
alert(numberAlert);


2. 🎖Using switch statement do the following

Take the value of `marks` (0-100) from user using `prompt` and `alert` the message (Your Grade is AA) as giver below.
* [ ] `AA` if `marks` is greater than 90.
* [ ] `AB` if `marks` is greater than 80 and less than or equal to 90
* [ ] `BB` if `marks` is greater than 70 and less than or equal to 80
* [ ] `BC` if `marks` is greater than 60 and less than or equal to 70
* [ ] `CC` if `marks` is greater than 50 and less than or equal to 60
* [ ] `CD` if `marks` is greater than 40 and less than or equal to 50
* [ ] `DD` if `marks` is greater than 30 and less than or equal to 40
* [ ] `FF` if `marks` is less than or equal to 30
```js
// Your code goes here
```
let marks = +prompt("Enter the marks between 0 and 100");
let grade;
if(marks < 0 || marks > 100){
  alert("Please enter valid marks in between 0 and 100");
}else{
  switch(true){
    case (marks <= 30):
      grade = "FF";
      break;
    case (marks <= 40):
      grade = "DD";
      break;
    case (marks <= 50):
      grade = "CD";
      break;
    case (marks <= 60):
      grade = "CC";
      break;
    case (marks <= 70):
      grade = "BC";
      break;
    case (marks <= 80):
      grade = "BB";
      break;
    case (marks <= 90):
      grade = "AB";
      break;
    case (marks <= 100):
      grade = "AA";
      break;
  }
  alert("Congratulations your grade is " + grade)
}