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
    - `150` is printed simply because the `finalPrice` variable always get
      reassigned to the value of `discountedPrice` which is `150`. The "math"
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
5. Line 12 will cause an error since `i` is defined using `let` which is block
   scoped. Therefore, `i` is inaccessible outside of the `for` loop. The
   `console.log(i)` statement at line 12 is outside of the `for` loop, so it
   cannot access the value of `i` inside the `for` loop. Therefore, an error
   will occur.
6. Line 13 will cause an error because `discountedPrice` is declared inside the
   `for` loop using `let` which is block scoped. Therefore, `discountedPrice` is
   inaccessible outside of the `for` loop. The `console.log(discountedPrice)`
   statement at line 13 is outside of the `for` loop, so it cannot access the
   value of `discountedPrice` inside the `for` loop. Therefore, an error will
    occur.
7. Line 14 will print `150` to the console. Since the variable `finalPrice` is
   declared using `let`, it is block scoped. Therefore, regardless of where the
   `console.log` statement is, it will be able to access the value of
   `finalPrice`. The value of `finalPrice` is set to `150` inside the `for`
   loop, so the `console.log` statement will print `150` to the console.
    - `150` is printed simply because the `finalPrice` variable always get
      reassigned to the value of `discountedPrice` which is `150`. The "math"
      behind the calculation of `finalPrice` is trivial since the
      `discountedPrice` is multiplied and divided by `100`, there is no
      difference between `discountedPrice` and `finalPrice` at the end of the
      `for` loop.
8. The function will return `[ 50, 100, 150 ]` which contains the discounted
    prices of the `prices` list based on the `discount` passed into the
    function. The function returns `discounted` which is an array of the same
    length as the `prices` list. The `discounted` array is populated by the
    `discountedPrice` variable which is calculated by multiplying each of the
    elements in `prices` by the `discount` (actually it is multiplied by
    `1-discount` but there is no difference since the discount is `0.5`).
9. Line 11 will cause an error because `i` is declared using `let` which is
   block scoped. Therefore, `i` is inaccessible outside of the `for` loop. The
   `console.log(i)` statement at line 11 is outside of the `for` loop, so it
   cannot access the value of `i` inside the `for` loop. Therefore, an error
   will occur.
10. Line 12 will print `3` since `length` is defined using `const` which is
    a block scoped variable. Therefore, `length` can be accessed by line 12
    since line 12 is in the same block as the `const` declaration of `length`.
11. The function will return `[ 50, 100, 150 ]` which contains the discounted
    prices of the `prices` list based on the `discount` passed into the
    function. The function returns `discounted` which is an array of the same
    length as the `prices` list. The `discounted` array is populated by the
    `discountedPrice` variable which is calculated by multiplying each of the
    elements in `prices` by the `discount` (actually it is multiplied by
    `1-discount` but there is no difference since the discount is `0.5`).

## Data Types

12. Notations
    - A. `student.name`
    - B. `student["Grad Year"]`
    - C. `student.greeting()`
    - D. `student['Favorite Teacher'].name`
    - E. `student.courseLoad[0]`
13. Arithmetic
    - A. `'32'`. The `+` operator is used to concatenate strings. Therefore,
      `'3' + '2'` is `'32'`.
    - B. `1`. The `-` operator is used to subtract numbers. Therefore, `3 - 1`
      is `2` and `2 + '2'` is `'22'`. Finally, `'22' - '2'` is `20` and `20 + 1`
      is `21`.
    - C. `3`. The `+` operator is used to add numbers. Therefore, `3 + null` is
      `3`.
    - D. `'3null'`. The `+` operator is used to concatenate strings. Therefore,
      `'3' + null` is `'3null'`.
    - E. `4`. The `+` operator is used to add numbers. Therefore, `true + 3` is
      `4`.
    - F. `0`. The `+` operator is used to add numbers. Therefore, `false + null`
      is `0`.
    - G. `3undefined`. The `+` operator is used to concatenate strings.
      Therefore, `'3' + undefined` is `'3undefined'`.
    - H. `NaN`. The `-` operator is used to subtract numbers. Therefore,
      `'3' - undefined` is `NaN`. `NaN` is a special value in JavaScript that
      means "Not a Number".
14. Comparison
    - A. `true`. '2' is converted to a number and `2 > 1` is `true`.
    - B. `false`. Because the `<` operator is used to compare strings. Since
      `'2'` is greater than `'1'`, in ASCII value, `'2'` is greater than `'12'`.
      Therefore, `'2' < '12'` is `false`.
    - C. `true`. `'2'` is converted to a number and `2 == 2` is `true`.
    - D. `false`. `===` is the strict equality operator. It checks if the two
      operands are equal and of the same type. `'2'` is a string and `2` is a
      number. Therefore, `'2' === 2` is `false`.
    - E. `false`. `true` is converted to `1` and `1 == 2` is `false`.
    - F. `true`. `Boolean(2)` is `true` and `true == true` is `true`.
15. The `==` operator is the equality operator. It checks if the two operands
    are equal. The `===` operator is the strict equality operator. It checks if
    the two operands are equal and of the same type. The `==` operator is
    "weaker" than the `===` operator because the `==` operator does not check
    the type of the operands. The `==` operator will convert the operands to
    the same type before comparing them. The `===` operator will not convert
    the operands to the same type before comparing them.

## Loops

16. [part2-question16.js](./part2-question16.js)

## Functions

17. The `modifyArray` function will return `[2, 4, 6]`. The `modifyArray`
    function takes in two parameters, an array and a callback function. The
    `modifyArray` function will iterate through the array and call the callback
    function on each element of the array. The callback function will double
    the value of the element and return the doubled value. The `modifyArray`
    function will store the doubled value in a new array and return the new
    array. Therefore, the `modifyArray` function will return `[2, 4, 6]`.
18. [part2-question18.js](./part2-question18.js)
19. ```
    1
    4
    3
    2
    ```

