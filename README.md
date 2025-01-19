# Lua Function Bug: Nil Argument Handling with +

This repository demonstrates a subtle bug in a Lua function that involves the handling of `nil` arguments when using the `+` operator. The function `foo` is expected to add two numbers, but it behaves unexpectedly when one or both arguments are `nil`.

## Bug Description
The function incorrectly returns `nil` instead of either throwing an error or providing a more meaningful response when encountering `nil` arguments. This is counter-intuitive, especially when one might expect an error or a default value.

## How to Reproduce
1. Clone this repository.
2. Run `bug.lua`.
3. Observe the unexpected output when calling `foo` with `nil` arguments.

## Solution
The `bugSolution.lua` file provides a corrected version of the function, addressing the issue by explicitly checking for `nil` values and handling them appropriately.