# CSS calc() Errors: Negative Values and Unit Incompatibilities

This repository demonstrates common errors encountered when using the `calc()` function in CSS, specifically focusing on issues with negative values and unit compatibility.

## Bug Description
The CSS `calc()` function can produce unexpected results when dealing with negative values or when combining different units in a calculation without proper consideration for unit compatibility. Negative values can lead to elements not rendering as expected, while incorrect unit combinations result in unexpected calculations.  This can manifest as elements collapsing, incorrect sizing, or other visual anomalies.

## How to Reproduce
1. Clone this repository.
2. Open `bug.css` to see the buggy code.
3. Open `bugSolution.css` to see the corrected code.  Experiment with adjusting values to observe the difference.

## Solution
Ensure the calculations within `calc()` result in positive values for dimensions such as `width` and `height`. Double-check unit compatibility and order of operations within complex calculations. For instance, consistently using the same unit across calculations helps avoid unexpected results. If negative values are unavoidable, ensure they're properly handled by your application's logic and fallback mechanisms. 