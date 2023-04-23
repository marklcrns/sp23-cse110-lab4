# Part 2

1. Since the variable `i` is declared inside a function with `var` variable
   type, it is function scoped. Therefore, the variable `i` is accessible
   outside of the `for` loop. The `for` loop will run 3 times, and each time it
   runs, it will increment the value of `i` by 1. Therefore, the value of `i`
   will be 3 after the `for` loop is done running. The `console.log` statement
   will print `3` to the console.
2. Line 13 will print `150` to the console. Since the variable `discountedPrice`
   is declared using `var`, it is function scoped. Therefore, regardless of
   where the `console.log` statement is, it will be able to access the value of
   `discountedPrice`. The value of `discountedPrice` is set to `150` inside the
   `for` loop, so the `console.log` statement will print `150` to the console.
    - `150` is printed because `300` was the last value in the `prices` list
      passed into the function. Also, the discount is `0.5` which is 50% off the
      `300` price. Therefore, `300 * 0.5` is `150`.
3. Line 14 will print `150` to the console. Since the variable `finalPrice` is
   declared using `var`, it is function scoped. Therefore, regardless of where
   the `console.log` statement is, it will be able to access the value of
   `finalPrice`. The value of `finalPrice` is set to `150` inside the `for`
   loop, so the `console.log` statement will print `150` to the console.
    - `150` is printed simply because the `finalPrice` variable is always get
      reassiend to the value of `discountedPrice` which is `150`. The "math"
      behind the calculation of `finalPrice` is trivial since the
      `discountedPrice` is multiplied and divided by `100`, there is no
      difference between `discountedPrice` and `finalPrice` at the end of the
      `for` loop.
4.  The function will return `[ 50, 100, 150 ]` which contains the discounted
    prices of the `prices` list based on the `discount` passed into the
    function. The function returns `discounted` which is an array of the same
    length as the `prices` list. The `discounted` array is populated by the
    `discountedPrice` variable which is calculated by multiplying each of the
    elements in `prices` by the `discount` (actually it is multiplied by
    `1-discount` but there is no difference since the discount is `0.5`).

