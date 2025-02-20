# Uncommon HTML Bug: Unexpected innerHTML Behavior
This repository demonstrates a subtle bug in HTML related to setting the `innerHTML` property of an element using a JavaScript object instead of a string.  The code attempts to insert a JavaScript object into the HTML, which leads to unexpected behavior.

## Problem
The provided `bug.html` file contains an example where a JavaScript object is assigned to `innerHTML`. This causes the expected text content to not render in the div with the id `myDiv`.

## Solution
The `bugSolution.html` demonstrates how to fix the problem.  The fix involves converting the JavaScript object into a string representation before assigning it to `innerHTML`.  Methods like `JSON.stringify()` can be used for this purpose, allowing for the proper display of the object's contents as a string.