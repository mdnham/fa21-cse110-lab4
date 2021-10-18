1. 3

    Since `i` was declared with `var`, it is function-scoped, and so it does exist throughout the function block. As the variable that controls the for-loop, we can see that the for-loop keeps going until `i` becomes greater than or equal to the length of prices. And since `i` begins at 0 and increments by 1, the for-loop stops when `i = 3` as `i < prices.length` is no longer true because prices.length is also 3.
2. 150
    Again, since `discountedPrice` is declared with `var`, it is function-scoped; hence it exists throughout the function block. And like `i`, it is reassigned a value for every loop, but since line 13 is executed after the for-loop is finished, the value of `discountedPrice` is dependent on the final loop, which would be when `i = 2`. And so, given that `prices[2] = 300` and `discount = 0.5`, we have that `discountedPrice = 150` from the execution of line 7. Thus, the execution of line 13 prints 150.
3. 150

    Similar to #2, `finalPrice` is declared with `var` and reassigned a value for every loop, so it is also dependent on the final loop. And given that we know that `discountedPrice = 150`, `finalPrice = 150` as well by the execution of line 8; hence, it prints out 150.
4. [50, 100, 150]

    Given the parameters `prices` and `discount`, the function calculates the reduced value of each entry of the array `prices` based of the value of `discount`. In our case, since `discount = 0.5`, every entry of `prices` will be cut in half; hence the function returns [50, 100, 150].
5. This will return an error since `i` was declared with `let`, and so it only existed within the for-loop. Hence, line 12 is calling for a variable that does not exist.
6. Like #5, this will return an error since `discountedPrice` only exists within every loop of the for-loop as it was declared with `let`, so line 13 is calling for a variable that does not exist.
7. 150

    Unlike #5 and #6, `finalPrice` was declared outside of the for-loop, and so it exists throughout the function block. Similar to #3, `finalPrice` is still reassigned a value for every loop, and so line 14 is dependent on the final loop, where `i = 2`. Since the for-loop works exactly the same as the `var` variant, `finalPrice = 150`, so line 14 prints out 150.
8. [50, 100, 150]

    Similar to #7, `discounted` was declared outside of the for-loop, so it exists throughout the function block. And like #4, since we still have the same parameters and the calculation portion of the code works exactly like the `var` variant, the entries of `prices` are still cut in half; hence this function also returns [50, 100, 150].
9. Again like #5, `i` was declared with `let` so it only exists within the for-loop. Thus, this will return an error since line 11 is calling for a variable that does not exist.
10. 3

    `length` is declared outside of the for-loop, and so it exists throughout the function block. From line 4, we know that length is equal to the length of `prices`, and so, `length = 3`. Thus, executing line 12 prints out 3.
11. [50, 100, 150]

    There are no issues with this code, and so this function, like #4 and #8, will calculate for the discounted values of the entries of `prices`, which in this case is also half of the entries. Hence, the function returns [50, 100, 150].
12. 
    A: `student.name`

    B: `student['Grad Year']`

    C: `student.greeting()`

    D: `student['Favorite Teacher'].name`

    E: `student.courseLoad[0]`

13. 
    A. '32'
    
    Since one of the operands is a string, the addition symbol is treated as string concatenation. Hence, 2 is converted into a string, and so '3' + '2' = '32'.

    B. 1

    Since the only string operation is concatenation (+), this operation has to be subtraction (of numbers), thus '3' is converted into a number. And so, 3 - 2 = 1.

    C. 3

    Since neither operand is a string, this operation is normal addition (between numbers). And so, null is converted into a number in which it is equivalent to 0. Hence, 3 + 0 = 3.

    D. '3null'

    Like A, since we have a string as one of the operands, this is treated as string concatenation, and so null is converted as a string. Hence, '3' + 'null' = '3null'.

    E. 4

    Like C, since there is no string operand, this is just normal addition. And so, true is converted into a number, specifically it is equivalent to 1. Hence, 1 + 3 = 4.

    F. 0

    Again, there is no string operand, and so this is just normal addition. Both false and null are converted into numbers, where both of them are equivalent to 0. Hence, 0 + 0 = 0.

    G. '3undefined'

    Like A and D, since there is a string operand, this becomes string concatenation, and so undefined is converted into a string. Hence, '3' + 'undefined' = '3undefined'.

    H. NaN

    This is subtraction between numbers in which both '3' and undefined are converted into numbers. However, undefined is equivalent to NaN as a number, and so 3 - NaN is just NaN.

14. 
    A. true

    For comparisons, different data types are converted to numbers, and so '2' is converted into a number before the comparison happens. Hence, we get true since 2 is greater than 1.

    B. false

    Since the operands are both strings, they are compared as strings rather than numbers. And so, since '1' comes before '2', '12' is actually less than '2', thus this results in false.

    C. true

    '==' checks for equality, but it only checks if the values are equal. In this case, since we have different data types, '2' first gets converted as a number before the comparison. And since 2 is equal to 2, this outputs true.

    D. false

    As for '===', it is stricter than '==', specifically it does not allow for type conversions. And so, it specifically compares if '2' is the same as 2, but they are not due to being different data types. Hence, we get false.

    E. false

    Like C, true first gets converted to a number, specifically 1, before it is compared. And since 1 is not equal to 2, this outputs false.

    F. true

    The Boolean object is initialized as true if the parameter isn't undefined or null (0, '', false). Hence, Boolean(2) has a value of true, thus it is exactly the same as true. Hence, this strict equality statement outputs true.

15. Both operators check for equality, but '===' is stricter than '=='. '==' compares after any necessary type conversions, thus it is focused more on equalities of values ignoring differences in data types. However, '===' does not, so it checks strict equality: value and data type.

17. (Markdown means 17.)

    With our parameters, modifyArray calls doSomething on every entry of the parameter array, [1, 2, 3], in which doSomething returns double of the input. And so, modifyArray will return an array with values that are double of the original entries: [2, 4, 6].

19. (Markdown means 19.)

    1

    4

    3

    2