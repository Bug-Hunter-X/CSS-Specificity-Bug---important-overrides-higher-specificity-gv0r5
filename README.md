# CSS Specificity Bug: !important overrides higher specificity

This repository demonstrates a subtle but important bug related to CSS specificity and the `!important` declaration.  The bug highlights a situation where `!important` overrides a more specific selector.

## Description

The bug involves unexpected behavior when combining specificity and the `!important` declaration.  While generally, higher specificity wins, this example shows `!important` takes precedence despite the specificity of another selector.  This is a common source of confusion and difficult-to-debug CSS issues. 

## How to Reproduce

1. Clone this repository.
2. Open `bug.css` to see the problematic code.
3. Open `bugSolution.css` to see one approach for resolving the issue.
4.  Create an HTML file that uses the classes defined in the CSS files to see the output in the browser.

## Solution

The provided `bugSolution.css` illustrates a potential solution.  It demonstrates the avoidance of `!important` declarations, using alternative styling techniques to achieve the desired effect without introducing unpredictable behavior.