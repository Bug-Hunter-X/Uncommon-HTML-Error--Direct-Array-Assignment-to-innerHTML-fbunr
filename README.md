# Uncommon HTML Error: Direct Array Assignment to innerHTML

This repository demonstrates an uncommon error in HTML related to the `innerHTML` property.  The error arises from attempting to directly assign a JavaScript array to the `innerHTML` property of an element.  This action will not throw an error, but will silently fail. The array will not render in the HTML.

## Bug Description

The bug is demonstrated in `bug.html`.  It incorrectly attempts to set the `innerHTML` of a div element to a JavaScript array. The expected behavior is to display the array's content as strings, but instead the content is not displayed because innerHTML expects a string as a value.

## Solution

The solution (`bugSolution.html`) demonstrates how to correctly assign the array to `innerHTML` by first converting it to a string.

## How to reproduce the bug

1. Clone this repo.
2. Open `bug.html` in a web browser.
3. Observe that the div with id "myDiv" remains empty, demonstrating the incorrect assignment of the array to innerHTML.

## How to fix the bug

1. Open `bugSolution.html`
2. Observe that the div with the id "myDiv" now correctly displays the array elements converted to string using the join method.