# Uncommon HTML Bug: Incorrect Element Removal

This repository demonstrates an uncommon bug in HTML related to removing elements using `innerHTML`.  Many developers mistakenly believe setting `innerHTML` to an empty string removes the element. This is incorrect; it only clears its content.

## The Bug
The `bug.html` file contains a simple HTML structure.  The JavaScript attempts to remove a div element by setting its `innerHTML` to an empty string. This, however, does not fully remove the element; it simply removes its content.  The element persists in the DOM, potentially causing issues later on. 

## The Solution
The `bugSolution.html` file shows the correct method for removing the element entirely. The JavaScript snippet correctly removes the element using the `removeChild` method. 