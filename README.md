# Unexpected Type Coercion in TypeScript

This repository demonstrates a common issue in TypeScript where type coercion can lead to unexpected runtime errors.  While TypeScript's type system catches many errors during compilation, it doesn't always prevent all potentially problematic type conversions.

The `bug.ts` file contains code that adds a number and a string. Although this may be acceptable behavior in some languages, in other cases it can produce unexpected results, and it highlights a gap in TypeScript's type safety.

The `bugSolution.ts` file offers a solution to avoid such issues.

## How to Reproduce

1. Clone this repository.
2. Open `bug.ts` in a TypeScript compiler.
3. Notice that the code compiles without any type errors.
4. Run the compiled JavaScript code and observe the unexpected output. 

## Solution

The solution involves adding stricter type checking and handling.