# READ9

## Refactoring

## What is functional programming?
Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data


- how do we know if a function is pure or not? Here is a very strict definition of purity:

1. It returns the same result if given the same arguments (it is also referred as deterministic)
2. It does not cause any observable side effects


- If our function reads external files, it’s not a pure function — the file’s contents can change.

- Any function that relies on a random number generator cannot be pure.

- Pure functions benefits is that The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts:

* Given a parameter A → expect the function to return value B
* Given a parameter C → expect the function to return value D


- When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

- Basically, if a function consistently yields the same result for the same input, it is referentially transparent.
pure functions + immutable data = referential transparency