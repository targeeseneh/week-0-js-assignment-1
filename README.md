# JavaScript Summary Assignment. 
### JavaScript is a high level programming language. It is a language for the browser but can also be run on other srvers like(Node.js). 
#### Why study Javascript.
- It's use in mobile development.
- It's use in desktop application development.
- It's use to build user interface.
  
##### MDN.
MDN is great for debugging and it's the best network for Javascript. 

##### Variables.
What are variables? In Javascript, a variable is like a continear that stores objects and there are three ways of creating a variable and they are Var, let and const. 
With var and let, you can assign and reassign value to a variable but with const you can assign a value but cannot reassign a value. 

##### Data Types.
Data types are types of informations. Some data types are string, numbers, boolean, null, undefine and symblo. 
+ Strings are used with a quotes, either single or double. It can be a number , letter or a word.
  ```javascript
    var school-name = 'KiT';
  ```
+ Numbers are basically ordinary numbers we use.
  ```javascript
    var sum = 10;
  ```
+ Boolean are basically true or false but unlike strings, they dont require quotes.
  ```javascript
   let learning = true;
  ```
+ Null means theres nothing in it.
  ```javascript
   let y = null;
  ```
+ Undefine is initializing a variable without a value.
  ```javascript
   let name;
  ```
##### Concatinating.
It is the act of adding two or more strings together and it's done by adding a plus(+) between the strings.
```javascript
var num1 + num2 
```
##### Arrays. 
What is an array? Arrays are variables that hols multiple values.
```javascript
let fruits = ['pineapple' , 'apple' , 'banana'] 
```
##### Object Literals.
What is an object literals? In JavaScript, an object is a standalone entity, with properties and type. An object must have a key and a value.
```javascript
const personDetail = {
    first name: "Targee",
    last name: "Seneh",
    age : 30,
    gender: "male"
};
``` 
An array of objects means initializing an array that has different objects with it key value pair in it. 

##### Loops.
Loops are used in JavaScript to perform repeated tasks based on a condition. Conditions typically return true or false. A loop will continue running until the defined condition returns false. 
Kinds of loops are:
 + For loop.
  ```javascript
   for (let i = 0; i < cars.length; i++) {
  text += cars[i] + "<br>";
 }
 ```
+ While loop.
```javascript
while (i < 10) {
  text += "The number is " + i;
  i++;
}
```
+ Do while loop.
```javascript
  do {
  text += "The number is " + i;
  i++;
}
```
while (i < 10);
+ For of loop.
```javascript
let language = "JavaScript";
let text = "";
for (let x of language) {
text += x;
}
```
+ For in loop.
```javascript
  const person = {fname:"John", lname:"Doe", age:25};
let text = "";
for (let x in person) {
  text += person[x];
}
```
##### Conditionals.
Conditional statements are used to perform different actions based on different conditions. There are three types of conditional statement in Javascript. They are: if, else and else if. 
###### The if Statement. 
Use the if statement to specify a block of JavaScript code to be executed if a condition is true.
```js
if (hour < 18) {
  greeting = "Good day";
}
```
###### The else Statement.
Use the else statement to specify a block of code to be executed if the condition is false.
```javascript
if (hour < 18) {
  greeting = "Good day";
} else {
  greeting = "Good evening";
}
```

###### The else if Statement.
Use the else if statement to specify a new condition if the first condition is false.
```javascript
if (time < 10) {
  greeting = "Good morning";
} else if (time < 20) {
  greeting = "Good day";
} else {
  greeting = "Good evening";
}
``` 

##### Function.
A JavaScript function is a block of code designed to perform a particular task.
A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses ().
Function names can contain letters, digits, underscores, and dollar signs.
The parentheses may include parameter names separated by commas:
(parameter1, parameter2).
The code to be executed by the function is placed inside curly brackets:{}.
```javascript
function reverseList() {
    var numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
    var reversed = numbers.reverse();
    console.log(reversed);
  }
  reverseList();
``` 
  
  ##### Document Object Model(DOM).
  When a web page is loaded, the browser creates a Document Object Model of the page. With the HTML DOM, JavaScript can access and change all the elements of an HTML document.
  There are few method that can be use to display items from a HTML ocument in the DoM, they are:
  + console.log(document.querySelectorAll)
  + conole.log(documet.getElemetByClassName)
  + conole.log(documet.getElemetByTagName)
  + conole.log(documet.getElemetById)
  + console.log(document.querySelector).
    
##### SetTimeout
The setTimeout() method executes a block of code after the specified time. The method executes the code only once. The commonly used syntax of JavaScript setTimeout is: setTimeout(function, milliseconds); 
```javascript
function startTime() {
  const date = new Date();
  document.getElementById("txt").innerHTML = date.toLocaleTimeString();
  setTimeout(function() {startTime()}, 1000);
}
```