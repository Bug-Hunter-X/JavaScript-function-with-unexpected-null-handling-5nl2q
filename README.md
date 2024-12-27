# JavaScript Null Handling Bug

This repository demonstrates a subtle bug in a JavaScript function involving null handling. The `foo` function is designed to add two numbers, but it unexpectedly returns `null` when one of the input is `null`.  The solution demonstrates a more robust approach.

## Bug

The original `foo` function returns `null` only when either `a` or `b` is explicitly `null`. Other falsy values like `0`, `false`, or `''` are not handled gracefully.

## Solution

The solution improves the function to use strict equality (`===`) to check for `null` explicitly, and allows other falsy values to be processed according to the default addition operation. This makes the function more predictable and flexible.