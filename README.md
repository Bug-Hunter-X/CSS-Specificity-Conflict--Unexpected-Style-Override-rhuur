# CSS Specificity Conflict Bug

This repository demonstrates a common issue in CSS: specificity conflicts.  The provided CSS contains two rules that target the same HTML element (`<p>`), but with different selectors. Due to specificity rules, one rule overrides the other, leading to unexpected styling results.

## Bug Description

The bug arises from a specificity conflict between two CSS rules.  The rule `div p { color: blue; }` attempts to set the color of paragraph elements within a `div` to blue. However, the rule `p { color: red; }` is more specific and sets the color to red, overriding the previous rule regardless of context.

## Solution

The solution involves understanding CSS specificity and adjusting the selectors to achieve the desired outcome. The solution file provides a fix by using a more specific selector, or by using `!important` (though this is generally discouraged).