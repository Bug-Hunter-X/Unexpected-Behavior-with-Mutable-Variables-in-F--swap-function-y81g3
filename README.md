# F# Mutable Variable Swap Bug

This repository demonstrates a common, yet subtle, bug in F# related to the behavior of mutable variables when passed to functions.  The `swap` function attempts to swap the values of two mutable variables, but due to F#'s pass-by-reference semantics, the swap operation modifies the original variables unexpectedly.

The `bug.fs` file contains the erroneous code. The `bugSolution.fs` file provides a corrected version that uses tuples to achieve the desired swap behavior without unintended side effects.