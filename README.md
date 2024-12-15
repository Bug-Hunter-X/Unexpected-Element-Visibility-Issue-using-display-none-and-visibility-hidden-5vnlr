# Uncommon HTML Bug: Incorrect use of CSS display and visibility properties

This repository demonstrates an uncommon bug related to the use of CSS `display` and `visibility` properties to control element visibility in HTML.

The bug arises from using both `display: none;` and `visibility: hidden;` on the same element. While both properties can hide an element, they do so in different ways, leading to unexpected visual results when used together.

## Bug Description
The `bug.html` file contains a simple HTML page with a div element that should be hidden when a button is clicked. The initial attempt uses both `display: none` and `visibility: hidden` in the JavaScript function to hide the div which causes unintended behavior.  The space that the div previously occupied is still maintained while the content is hidden.

## Solution
The `bugSolution.html` demonstrates the correct approach using only `display: none;` which removes the element completely from the layout flow. 

## How to Reproduce
1. Clone the repository.
2. Open `bug.html` and `bugSolution.html` in a web browser.
3. Click the button in each HTML file and observe the difference in the div element's behavior.