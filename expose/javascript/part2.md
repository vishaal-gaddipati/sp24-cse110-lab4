1. 3 will be printed. This is because the variable i is declared with the var keyword and thus it has function scope, so regardless of the block it is defined in, it can still be accessed anywhere in the function. After the for loop is done, i has a value of 3 (since prices if of length 3, so i will go from 0 to 1 to 2 then 3 which ends the loop). At line 12 this value of i=3 is printed to the console.
2. 150 will be printed. This is because the last value that is stored in discountedPrice before the for loop terminates is what will still be in discountedPrice when it is printed on line 13. Since it has keyword var, it can still be accessed outside of the for loop block. The value itself is 150 because var discountedPrice = prices[2] * (1 - discount), where prices[2] = 300 and discount = 0.5. This 300 * (1 - 0.5) = 150.
3. 150 will also be printed at line 14. This is because finalPrice has var keyword so it can be accessed anywhere in the function. The value is 150, because we take the last discountedPrice value in the for loop, which is 150 from question 2, and then multiply it by 100, round which has no effect since there is no floating point numbers, and divide by 100, which results in the number still being 150. Then on line 14 this is outputted to the console.
4. [ 50, 100, 150 ] will be returned. This is because the function itself is applying the discount to all values in the provided array. So the parameter array of [100, 200, 300] with the input discount of 0.5 will halve all the prices based on the function code and result in [50, 100, 150] to be returned. The push call on line 9 is adding the discounted prices to the end of a new array.
5. The code returns a ReferenceError because the let keyword implies the variable i has a block scope within the for loop. So by line 12, i is not defined. Thus it cannot be accessed outside of the block which is why there is an error.
6. The code returns a ReferenceError because the let keyword implies the variable discountedPrice has a block scope within the for loop. So by line 13, discountedPrice is not defined. Thus it cannot be accessed outside of the block which is why there is an error.
7. 150 will be printed at line 14. This is because finalPrice has the let keyword but it is defined in the same scope as the console.log() call that uses it as a parameter. Thus it can be accessed by line 14 because they are on the same level in the code. The value is 150, because we take the last discountedPrice value in the for loop, which is 150 from question 2, and then multiply it by 100, round which has no effect since there is no floating point numbers, and divide by 100, which results in the number still being 150. Then on line 14 this is outputted to the console.
8. [ 50, 100, 150 ] will be returned. This is because the function itself is applying the discount to all values in the provided array. So the parameter array of [100, 200, 300] with the input discount of 0.5 will halve all the prices based on the function code and result in [50, 100, 150] to be returned. The push call on line 9 is adding the discounted prices to the end of a new array. And this array can be returned because despite having the keyword let, that let is not in a block and is on the same level as line 16 so the return causes no issue.
9. The code returns a ReferenceError because the let keyword implies the variable i has a block scope within the for loop. So by line 11, i is not defined. Thus it cannot be accessed outside of the block which is why there is an error.
10. 3 will be printed. This is because the variable length is declared with the const keyword and thus it has block scope, which means that it can only be accessed within the block it is defined in, unlike the var keyword. The variable length is defined to be statically set as the length of the input array prices' length. At line 12 this value of length is printed to the console, which is allowed because the call is in the same scope as the const declaration of length.
11. [ 50, 100, 150 ] will be returned. This is because the function itself is applying the discount to all values in the provided array. So the parameter array of [100, 200, 300] with the input discount of 0.5 will halve all the prices based on the function code and result in [50, 100, 150] to be returned. The push call on line 8 is adding the discounted prices to the end of a new array. And this array can be returned because despite having the keyword const, that const is not in a block and is on the same level as line 14 so the return causes no issue. And we are able to push to a const array in JavaScript so this causes no issue since we are not explicitly reassinging discounted at any point.
12. A. student.name; <br/>
    B. student['Grad Year']; <br/>
    C. student.greeting(); <br/>
    D. student['Favorite Teacher'].name; <br/>
    E. student.courseLoad[0];
13. A. '32'. This is the output because the 2 is type converted into a string '2' and concatenated to '3' becoming '32'. The + implies string concatenation and not math addition. <br/>
    B. 1. This is the output because the '3' string is converted into an integer 3 since mathematical operations take place between integers, so 3 - 2 = 1. <br/>
    C. 3. The output is 3 because null is a 0 in numerical operations. <br/>
    D. '3null'. This is the output because null is converted to the string 'null' and concatenated to '3'. <br/>
    E. 4. The output is 4 because true is converted to a 1 in numerical operations and 1 + 3 = 4. <br/>
    F. 0. The output is 0 because both false and null are type converted to 0 in numerical operations which happen since neither are strings thus we don't concatenate. <br/>
    G. '3undefined'. The output is such because undefined is converted to a string and concatenated with the string '3'. <br/>
    H. NaN. The output is NaN because no arithemtic can be done with undefined so it is type converted to NaN.
14. A. true. The output is true because '2' is type converted from string to integer and is greated than 1. <br/>
    B. false. The output is false because lexographically, '2' comes after '1' and thus it is greater. '1' was considered since it is the first character in the string '12'. <br/>
    C. true. The output is true because '2' is converted to an integer and is thus equal to 2. <br/>
    D. false. The output is false because === is a strict equality check with no type conversion and a string and integer are not of the same type thus they can't be compared. <br/>
    E. false. The output is false because true is type converted to integer 1 but that isn't equal to 2. <br/>
    F. true. The output is true because because since 2 is a non empty value it is Boolean converted to true, then the strict equality operator first checks the types, which since both are Boolean is satisfied, then checks if they are equal and true is equivalent to true thus return true.
15. The difference between == and === operators is that == does type conversion before comparison. However, === is a strict equality operator meaning it first checks type equivalence, then checks is the values are the same.

17. (ACTUALLY IS #17) [ 2, 4, 6 ]. This is the output because on each value in array, we call the callback function, which is doSomething(), to multiply each value in array by 2 and push it into an array to return. That is why the output is everything in the original array times 2.

19. (ACTUALLY IS #19) <br/>
    1 <br/>
    4 <br/>
    3 <br/>
    2