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
8. How differnt frameworks deal with coersion.







