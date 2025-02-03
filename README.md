# CSS Calc() Unexpected Width Calculation with Border

This repository demonstrates a subtle bug related to the CSS `calc()` function and border width.  The issue arises when using `calc()` to determine an element's width while also applying a border.

The bug is that the border is added *outside* the area calculated by `calc()`, leading to unexpected element dimensions and potential layout problems.  This is especially problematic when nesting elements.

The `bug.css` file contains the problematic code, and `bugSolution.css` provides a solution.

## Solution

The solution involves taking the border into account when calculating the width using `calc()`.  See `bugSolution.css` for details.