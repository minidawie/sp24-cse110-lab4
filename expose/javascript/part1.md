1) What is printed by line 9? If the code returns an error, explain why.
    - 20
2) What is printed by line 13? If the code returns an error, explain why. 
    - 20. Even though result is "out of scope" it can still be accessed because it is of type var which has a function wide scope, not a block scope.

3) What is printed by line 9? If the code returns an error, explain why.
    - 20
4) What is printed by line 13? If the code returns an error, explain why.
    - error. This is the output because the let data type only has block scope meaning that it cannot be accessed outside of the block it was declared in. Since the final result console.log is outside of the if-statement that result is declared in, result was not able to be accessed.

5) What is printed by line 9? If the code returns an error, explain why.
    - error. This error is cause because we are trying to reassign the value in a const variable. 
6) What is printed by line 13? If the code returns an error, explain why
    - error. This is the output because the let data type only has block scope meaning that it cannot be accessed outside of the block it was declared in. Since the final result console.log is outside of the if-statement that result is declared in, result was not able to be accessed.