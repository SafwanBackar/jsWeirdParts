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
