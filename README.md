# Sprint Challenge - JavaScript Fundamentals

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This challenge allows you to practice the concepts and techniques learned over the past week and apply them in project. This Sprint explored JavaScript Fundamentals. During this Sprint, you studied array methods, this keyword, prototypes, and class syntax. In your challenge this week, you will demonstrate proficiency by completing a range of JavaScript problems.

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the sprint challenge. 

## Introduction

The index.js file contains all of your challenges. Please review it in full before answering the questions. If you complete the stretch goals please leave them in your file but commented out so that they do not affect the MVP tasks 

In meeting the minimum viable product (MVP) specifications listed below, you should have all tests passing. You can console.log to check your work and ensure you are submitting the correct results 

### Commits

Set up codegrade early and commit your code regularly and meaningfully. 

## Interview Questions
### (please edit this file and write your answer below each question.)
Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read.

1. Explain the differences between `.map`, `.reduce` and `.filter` and describe a use case for each. 

        .map -- .map iterates through all the items in the array and returns a new array, unlike forEach which may edit data in the original array, map can convert data in that copy it makes, this is really useful if you need to add and delete key pairs frequently, because you can do that with no fear of losing the original data record forever. 

        .reduce -- .reduce executes a "reducer" callback function on each element of the array, passing in the return value from the calculation on the preceding element. The reducer callback walks through the array element-by-element, at each step adding the current array value to the result from the previous step. This is really handy for inventory, like adding up sums and totals.

        .filter --  .filter creates a new array with all elements that pass the test implemented by the provided function. It calls a provided callback function once for each element in an array, and constructs a new array of all the values for which the callback returns a value that is true. This is super handy for searching through large databases and pulling out the information you want like for our travel example we did in class, finding all the cities with good wifi, hiking and beaches. 





2. Explain the difference between a callback and a higher order function.

        - a higher order function is a function that takes in a callback function as a parameter or argument. 

3. Explain what a closure is.

        - a closure is when an inner function reaches into it's surrounding state to grab a value. 

4. Describe the four principles of the 'this' keyword.

        1. Window binding -if we haven't given 'this' any context it will return the window, the global object in node or undefined in strict mode.

        2. Implicit binding - Applies to objects with methods. When the function (method) is invoked, look the the left of the dot, that's what 'this' refers to.

        3. Explicit binding - we tell a function what the 'this' keyword should be using .call, .apply or .bind. Call will immediately invoke the function and you pass in your arguments 1 by 1. Apply will immediately invoke the function and you pass in your arguments as an array. Bind you pass in your arguments 1 by 1, but it will not immediately invoke the function, instead it returns a brand new function that can be invoked later.

        4. New binding - When a function is invoked with a new keyword the this keyword inside that function is bound to the new object being constructed. When a function is   invoked as a constructor function using the new keyword, this points to the new object that’s created


5. Why do we need super() in an extended class?

        - we need to 'superimpose' the parameters of the parent constructor onto the child so as to not lose the methods from the parent. 

You are expected to be able to answer questions in these areas. Your responses contribute to your Sprint Challenge grade. 

## Instructions

### Task 1: Set up Project

Using VSCode and Command Line:


1. Fork the repo
2. Go into canvas and connect your reop to codegrade
3. Clone your forked version of the repo
4. DO NOT CREATE A BRANCH. You will be pushing your changes to the main/master today
5. cd into your repo
6. open the terminal in your vs code and type `npm install`
7. next type `npm run test` in your terminal
8. Complete your work making regular commits to main/ master your codegrade score will update each time you make a push.


### Testing & Debugging

Open a second terminal inside of your project by clicking on the split terminal icon
![alt text](assets/split_terminal.png "Split Terminal")

Inside of your second terminal type `npm start` 
![alt text](assets/npm_start.png "type npm start")

You will be running your tests in one terminal and debugging in the other. As you work on your code you should make use of `console.log` to check your progress and debug.
![alt text](assets/tests_debug_terminal_final.png "your terminal should look like this")

### Task 2: Project Requirements (MVP)

You must complete all tasks inside of `index.js` and answer the questions above.

In your solutions, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

## Resources
 
 [Sprint Challenge Study Guide](https://www.notion.so/lambdaschool/Unit-1-Sprint-3-Study-Guide-033a9a00659a4ef98c12eb97e49a6110)

## Submission format

Please submit your project via codegrade by following [these instructions](https://lambdaschool.notion.site/lambdaschool/Lambda-School-Git-Flow-Step-by-step-269f68ae3bf64eb689a8328715a179f9) See part 2, submitting an assignment with codegrade
