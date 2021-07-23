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
Answers: each on of these is a higher order array method that will scan or iterate over an existing array to either pull or compute values from it, and returning a new array.
   a: (.map): iterates over an array, pulls elements and possibly performing some action on the value from the existing array, passing the result(s) into a new array. In the callback function, only the array element is required. The index, and array can be given as the second and third parameters (in this order, respectively), but are optional. A use case might be when one wants iterate over or map over a array of numbers, such as [1, 2, 3], twice, would return the array [2, 4, 6]. In this case we have a set of data and are performing the action on the value at each index, and pushing the results of that action into a new array.
   b. (.filter): iterates over an array, using a callback function that essentially sets a true/false condition that is used to push data or values to a new array. As with .map, only the element is required, but the index and array can also be provided. A use case might be to pull from an array of student grades, pulling out all the students whose grades are greater than or equal to 75.
   c. (.reduce): iterates over an array, reducing a set of values down to one value. When using .reduce(), accumulator (acc) and current value are required arguments for it to run. The index and array can be indicated but are optional here as well. The other unique feature here is the initial value, which is essentially the starting point from which the accumulator performs it's task. In the case of using addition, the initial value would typically be 0, and when using ,multiplication, the initial value would be set to 1 because anything multiplied by 0 will always be zero. One example of a case might include adding  or multiplying a set of numbers, but .reduce() is considered quite veratile.

2. Explain the difference between a callback and a higher order function.

Answer: A function that can accept or receive another function into it to execute is a higher-order function, and conversely, or respectively, a callback function is a function that is passed into a higher order function. 

3. Explain what a closure is.

Answer: Closure is based on the principle that an inner function has access to the function outside of itself, including the variables that exist in the outer scope. When an inner function reaches outside its own scope ('outward') that is when the closure occurs. 

4. Describe the four principles of the 'this' keyword.

Answer: 
   a. Implicit Binding: Whenever a preceding dot calls a function, the object before the dot is 'this'.
   b. Explicit Binding: Whenever we use Javascript's .call() or .apply() methods, 'this' is explicitly defined
   c. Window/Global Object Binding: If 'this' is not bound by any of the principles involved in explicit, implicit, or new binding, the 'this' will make reference to the window/global object. This is true except when running in strict mode.
   d. New Binding: When the 'new' keyword is used in the creation of a new object, under the hood Javascript associates this with the creation of the new object. 

5. Why do we need super() in an extended class?

Answer: if 'extend' is used in the creation of a child or sub-class, super() needs to be called from within the sub-classes' constructor function in order to pass any new attributes back up to the constructor of the parent object.  

You are expected to be able to answer questions in these areas. Your responses contribute to your Sprint Challenge grade. 

## Instructions

### Task 1: Set up Project

Using VSCode and Command Line:


1. Fork the repo
2. Clone your forked version of the repo
3. cd into your repo and create a branch with your first and last name
4. open the terminal in your vs code and type `npm install`
5. next type `npm run test` in your terminal
6. Complete your work making regular commits, once you have all your tests passing and you are ready to submit your work please see canvas for instructions on how to submit

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

Please submit your project via codegrade by following [these instructions](https://www.notion.so/lambdaschool/Submitting-an-assignment-via-Code-Grade-A-Step-by-Step-Walkthrough-07bd65f5f8364e709ecb5064735ce374)

