# Inconsistent Unit Handling with CSS calc()

This repository demonstrates a common issue encountered when using the `calc()` function in CSS. Specifically, inconsistencies in unit handling across different browsers can lead to unexpected layout results.

## The Problem
The `calc()` function allows for dynamic calculations within CSS, but combining different units (like percentages and pixels) can cause problems due to variations in how browsers interpret and calculate these values. This can result in elements rendering at unexpected sizes or positions.

## Example
See `bug.css` for an example of a layout that exhibits this issue.  The intended layout may not render correctly across all browsers due to the `calc()` calculation involving both percentages and pixels. 

## Solution
The `bugSolution.css` file demonstrates a possible solution, avoiding the problematic mixing of units within the `calc()` function.  Alternatives include using only one unit type in the calculation, or employing a different approach to achieve the desired layout without relying on potentially inconsistent `calc()` expressions.

## How to Reproduce
1. Clone this repository.
2. Open `index.html` (not included but assumed to use the CSS files) in various browsers.
3. Observe how the layout differs, demonstrating the inconsistencies caused by the `calc()` function in `bug.css`. 
4. Compare that with the layout in `bugSolution.css` which uses a more robust approach.