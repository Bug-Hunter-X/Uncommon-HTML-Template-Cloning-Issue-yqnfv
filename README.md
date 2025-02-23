# Uncommon HTML Template Cloning Issue

This repository demonstrates an uncommon bug related to cloning template content in HTML using JavaScript.  The issue arises when using `cloneNode(false)` incorrectly with the `&lt;template&gt;` tag.  This leads to an empty element being added to the DOM instead of the expected cloned content.  The solution demonstrates the correct way to clone the template content.

## Bug
The bug lies in the way the template content is cloned.  `cloneNode(false)` only clones the template element itself, not its inner content.  This results in an empty div being added to the `#app` element. 

## Solution
The solution corrects the cloning process by using `cloneNode(true)`. This ensures the entire content within the template is cloned, resolving the issue.