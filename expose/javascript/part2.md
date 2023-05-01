1. Line 12 will print "3" because the for loop on lines 6-10 will finish executing when `i` is equal to `prices.length`, which is 3. It will successfully print as `i` is declared as a `var`, so it can continue to be used in the scope of the function.
2. Line 13 will print "150" because the final value of `discountedPrice` will be assigned when `i` is 2. Then, the expression assigned to `discountedPrice` will be (300) * (1 - 0.5), which is equal to 150. It is declared as a `var` and thus can successfully print upon reaching the `console.log` on line 13.
3. Line 14 will print "150" because the final value of `finalPrice` will occur when the value of `discountedPrice` is 150 (see above explanation), so the expression that assigns it a value will be `Math.round(150 * 100) / 100`, which evaluates to 150. It will successfully print as `finalPrice` is declared as a `var`.
4. This function will return an array containing the elements [50, 100, 150] in order, because as the `finalPrice` variable is evaluated on line 8, it is pushed to the `discounted` array on line 9. Since the inputs to the function are an array containing [100, 200, 300] and a "discount" of 0.5, it will return an array containing the corresponding elements after being multiplied by the discount and rounded.
5. ReferenceError: i is not defined
   
   This code causes an error as `i` is defined using `let`, and thus cannot be used outside the scope of the for loop. Since line 12 tries to access `i` outside of the for loop, it throws an error.
6. ReferenceError: discountedPrice is not defined
   
   This code also causes an error as `discountedPrice` is defined using `let` within the for loop, and thus upon reaching line 13 the code will throw an error as described above.
7. Line 14 will print "150" because the final value of `finalPrice` will occur when the value of `discountedPrice` is 150 (see explanation in question 2), so the expression that assigns it a value will be `Math.round(150 * 100) / 100`, which evaluates to 150. It will successfully print as `finalPrice` is declared using `let`, and line 14 accesses the variable within the same scope (unlike in the recent questions).
8. This function will return an array containing the elements [50, 100, 150] in order, because as the `finalPrice` variable is evaluated on line 8, it is pushed to the `discounted` array on line 9. Since the inputs to the function are an array containing [100, 200, 300] and a "discount" of 0.5, it will return an array containing the corresponding elements after being multiplied by the discount and rounded. Since `discounted` is returned in the same scope as it is declared, no error will be thrown.
9. ReferenceError: i is not defined
   
   This code causes an error as `i` is defined using `let`, and thus cannot be used outside the scope of the for loop. Since line 11 tries to access `i` outside of the for loop, it throws an error.
10. Line 12 will print 3 because `length` is initialized to be the length of the `prices` array, which has 3 elements in the function call on line 17. No error is thrown as `length` is only defined once as a `const`.
11. This function will return an array containing the elements [50, 100, 150] in order, because the discounted price is calculated to be each element of the input `prices` array multiplied by (1-`discount`). In this case, (1-`discount`) = 0.5. Thus each element will be multiplied by 5. Then, after each discounted price is calculated, it will be added to the output array, which is returned on line 14.
12. A. `student.name`
    
    B. `student['Grad Year']`

    C. `student.greeting()`

    D. `student["Favorite Teacher"].name`

    E. `student.courseLoad[0]`

13. A. `32`, because it treats 3 as a string and then concatenates 2 onto it.
    
    B. `1`, because it automatically converts the string 3 to a number before doing the mathematical operation.

    C. `3`, because it treats null as 0 in this context.

    D. `3null`, because it converts null to a string and concatenates it.

    E. `4`, because it treats true as 1 in this case.

    F. `0`, because it treats both false and null as a 0.

    G. `3undefined`, because it treats undefined as a string and concatenates it.

    H. `NaN`, because it tries to do a mathematical operation with undefined, but cannot, so it defaults to NaN.

14. A. true
    
    B. false, because it uses string comparison with alphabetical ordering.

    C. true, because it treats the string as a number.

    D. false, because it does strict equality, and the two values are different types.

    E. false, because it treats the true as a 1, and 1 does not equal 2 in this context.

    F. true, because after converting the 2 to a boolean value it becomes true and then both values are strictly equal.

15. `==` does automatic conversions to attempt to check basic equality, while `===` tests strict equality, which means it also compares the types of the two values.
16. See part2-question16.js
17. The result will be an array containing the elements [2, 4, 6], because the `modifyArray` function will take in the array as a parameter and call the `doSomething` function on each of the elements of the given array. In this case, the `doSomething` function multiplies a given input by 2, hence the output array being each element of the input array multiplied by 2.
18. See part2-question18.js
19. The output of the code will be:
    ```
    1
    4
    3
    2
    ```
