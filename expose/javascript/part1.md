# Part 1 Answers

1. `values added: 20`
    - The code does not return an error.
2. `final result: 20` 
    - The code does not return an error.
3. `values added: 20`
    - So far, this lines does not return an error.
4. The code returns an error.
    - The code returns an error because the variable `result` is not defined
      since `let` is block scoped. The variable `result` is defined inside the
      `if` block, so it is not accessible outside of the block. Therefore, line
      13, which is outside of the block where `result` is defined, returns an
      error.
5. `values added: 20`
    - So far, this lines does not return an error.
6. The code returns an error.
    - Similar to `let` variable type, `const` are block scoped. Therefore, the
      variable `result` is not accessible outside of the block where it is
      defined. Therefore, line 13, which is outside of the block where `result`
      is defined, returns an error.
