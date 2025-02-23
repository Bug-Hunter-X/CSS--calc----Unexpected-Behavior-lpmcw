# CSS `calc()` Unexpected Behavior

This repository demonstrates an uncommon bug related to the CSS `calc()` function.  Specifically, it highlights issues with percentage-based calculations and nested `calc()` expressions. The `bug.css` file contains the problematic code, and `bugSolution.css` offers a corrected approach.

## Bug Description
The `calc()` function, while powerful, can be tricky. When combined with percentages, it relies heavily on the parent container's dimensions. If the parent's dimensions are not explicitly set, the calculation might not behave as expected, potentially leading to incorrect element sizing.  Additionally, improperly nested `calc()` expressions can result in parsing errors by the browser.

## Solution
The solution involves ensuring that parent containers have explicitly defined widths (or heights, depending on the context) before using percentages in `calc()`. For nested `calc()` functions, careful construction and adherence to proper syntax is critical to avoid parsing errors.  Always test thoroughly across different browsers.