1. values added:  20
2. final result:  20
3. values added:  20
4. The code returns a ReferenceError because the let keyword implies the variable has a block scope within the if statement. So by line 13, result is not defined. Thus it cannot be accessed outside of the block which is why there is an error.
5. The code returns a TypeError because the const keyword implies that the variable cannot be reassigned after it is assigned for the first time. However, on line 9 it is reassigned which is why the "Assignment to constant variable." error is displayed.
6. The code would return the exact same error as that printed by question 5 because the code for line 13 would not be reached since the other error happens at line 9 which is before line 13. But if the line were to be reached, it would still throw an error because const has the same scope as the let keyword, so if line 7 were to be remove, then a ReferenceError would have been thrown instead (like question 4).