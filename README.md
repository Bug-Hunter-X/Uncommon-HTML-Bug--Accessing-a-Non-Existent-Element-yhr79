# Uncommon HTML Bug: Accessing a Non-Existent Element

This repository demonstrates a common error in HTML and JavaScript interaction: attempting to manipulate a DOM element that doesn't exist.  The bug is subtle and can be difficult to track down if not carefully checked.  The solution showcases best practices to avoid this type of error.

## Bug Description

The provided HTML file attempts to modify the `innerHTML` of an element with the ID 'myDiv2'. However, this element is never created within the HTML structure, resulting in a runtime JavaScript error.  This is a silent error that may not be immediately obvious.

## Solution

The solution implements a check to see if the element exists before attempting to change it.  If it does not exist, it's created first. This safe approach prevents the error from occurring.