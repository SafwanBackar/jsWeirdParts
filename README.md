# jsWeirdParts

Notes for udemy course on JS , understanding the weird parts


Chapter 1: 
==========
1. Syntax parser - compile the code for computer
2. Lexial environment - where the code is written (physically, line by line) and what contains it
3. Execution context - Wrapper to help manage the code that is running. Whenever a code is running or executed,an execution context is created and code is running 
   inside an execution context. A global object (its window object in browsers) and a 'this' variable is created by js inside your running code.(Try this in an empty 
   Every execution context is placed in a stack (2 functions are 2 execution context)
   console.(it will be the window object))
   Never set a varible undefined(Eg: var a = undefined) . Let js do it. That way when debugging, you'll know that it wasn't you who set it.
   Invocation - Running a function 
   Global execution context
   
Chapter 2: Types and Operators
=========

1. Js is dynamic typing. It will figure out when we assing or write code.
When we assign 'safwan' to var name, it will know its a string.
2. Primitive and non primitive data types.
3. Primitive type - Single value, pre defined, known memory 
4. Operators perform certain functions
5. Operator precedence - The structure which decides which operator has the higher precedence and call it in order accordingly.
   If we use multiply and additon in a problem, mulitplication has a precendence of 14 where as addition has a precedence of 13 (based on js operator precedence table),    so it multiplies first. 
   Check var a=2,b=3,c=3, then, a=b=c. It will be 3(Answer: associativity(right to left for equal sign))
6. Coersion - Converting a value from one type to another (var a = 'safwan' + 'backar')
   Instead of adding like a number it returns 'safwan backar' as concantenation, this is dynamic typing. JS does this under the hood. (0==false being true, all done by coersion)
7. Check false < 1, it is true. Js does coersion, converts false to number, checks the associativity. Try Number(false), it will be 0. Number(true) will be 1.
8. How differnt frameworks deal with coersion and assinging a method or property.

Chapter 3: Objects and functions
==========

Day 1.
1. Functions are objects. They are objects with some method or property inside that is commanded to be invocable(meaning that it should run that code)
2. Function inside an object is a method.
3.  Object inside an object is property of the parent object.
4. Function expression and function statements
5. Expresssion = A unit of code that results(returns) in a value(1+2 returns 3). When we say statement, it means to do some work.
6. If statement, if(a===3), a===3 is an expression returning boolean, whereas the if statement itself is a statement, it on its doesn't return a value.
7. function greet(){console.log('h')} is a funtion statement and doesn't return anything until its run and is stored in the memory 
8. Anonymous funtion is fn that doesn't have a name. Its maybe stored in a variable
9. var anonymousGreet = function(){console('hi')}. This is fn expression. It returns a value, an object. A fn object.
10. First class funtions (passed as an argument). 

Day 2.
1. Call by reference (aliases refering to the same location in memory)(eg:objects) and call by value.(sitting completely in differnt spot in the memory)(variables)
2. Setting up default parameters.(eg: var name; name = name || 'john doe';)
3. When a spred operator is used as an argument in a funtion, all the data that comes in the spread will be in an array.

Day 3.

1. Automatic semicolon insertion.(Don't let js decide)
2. Immadiately invoked function expression (iife) (4. - 15) 
3. Running an anonymous fn without setting to a variable by wrapping it in (). So the js know that its an expression, it returns something. Also putting () after a fn is declared makes it run instantly.
(
  function(name){console.log('hello')}()
) 

Chapter 4 : OOP
===========
1. Inheritance -  One object gets the props and methods of another object. Classical and prototypal inheritance. JS has prototypal Inheritance
2. All object have a prototype property.  
3. Reflection and extend. Extend - Combine objects?











