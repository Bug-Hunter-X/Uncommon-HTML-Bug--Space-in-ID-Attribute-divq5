# Uncommon HTML Bug: Space in ID Attribute

This repository demonstrates an uncommon bug in HTML related to using spaces in the `id` attribute of an element.  The bug arises from an incorrect use of `document.getElementById()` which fails when the element's `id` contains spaces.

## Bug Description

The `bug.html` file attempts to modify the `innerHTML` of a div element using its ID. However, the ID has a space in it ('my Div'), which is invalid. The `document.getElementById()` method only works correctly when the `id` is a single word.

## Solution

The solution involves removing the space from the ID of the `div` element or using a CSS selector that can handle spaces in attributes if you cannot rename the ID.  The `bugSolution.html` demonstrates the corrected version.