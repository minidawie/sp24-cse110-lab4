1) What will happen at line 12 and why? If the code causes an error, explain why.
    - 3. This is because i will continually iterate until the break condition is met which is 3
2) What will happen at line 13 and why? If the code causes an error, explain why. 
    - 150. discountedPrice is updated after every loop. On the last loop it is updated to 300 * (1-.5) which is 150.
3) What will happen at line 14 and why? If the code causes an error, explain why.
    - 150. finalPrice is updated after every loop. Math.round will round to the nearest integer. In this case it does nothing because discountedPrice is already an integer so multiplying by an integer results in an integer.
4) What will this function return? Give a brief explanation why. If the code causes an error, explain why.
    - The function will return an array of [50, 100, 150]. Since the operation in discountedPrice results in an integer all 3 times, the operations in finalPrice can be ignored, thus resulting in the values in prices being half their original value.
5) What will happen at line 12 and why?  If the code causes an error, explain why. ^^^ (assume this function is being called like the others: discountPrices([100, 200, 300], 0.5)).
    - error because i is outside of the scope of the console.log
6) What will happen at line 13 and why? If the code causes an error, explain why. 
    - error because discountedPrice is outside of the scope of the console.log
7) What will happen at line 14 and why? If the code causes an error, explain why. 
    - 150. This is because finalPrice is declared as a function wide variable in line 4, so even if it is updated within the for-loop that value can still be accessed outside of the for-loops termination.
8) What will this function return? Give a brief explanation. If the code causes an error, explain why.
    - The function will return an array of [50, 100, 150]. discounted is declared as a function wide array so its values can be accessed outside of the for-loops termination. Since the operation in discountedPrice results in an integer all 3 times, the operations in finalPrice can be ignored, thus resulting in the values in prices being half their original value.
9) What will happen at line 11 and why? If the code causes an error, explain why. 
    - error because i is outside of the scope of the console.log 
10) What will happen at line 12 and why? If the code causes an error, explain why.
    - 3 because length is declared as a function wide variable and prices.length is 3.
11) What will this function return? Give a brief explanation. If the code causes an error, explain why. 
    - The function will return an array of [50, 100, 150]. discounted is declared as a function wide array so its values can be accessed outside of the for-loops termination. Although discountedPrice is declared as a const it is being redeclared every loop so it may seem like we are reassigning the value of a const variable, but we are instead creating a new variable every time. Since the operation in discountedPrice results in an integer all 3 times, the operations in finalPrice can be ignored, thus resulting in the values in prices being half their original value.

12) Given the above Object, write the notation for:
    a. Accessing the value of the name property in the student object
        - student.name
    b. Accessing the value of the Grad Year property in the student object
        - student['Grad Year']
    c. Calling the function for the greeting property in the student object
        - student.greeting()
    d. Accessing the name property of the object in the Favorite Teacher property in student
        - student['Favorite Teacher'].name
    e. Access index zero in the array of the courseLoad property of the student object
        - student.courseLoad[0]

13) Arithmetic
    a. '3' + 2 = 32
        - string concatenation is done with the + operator.
    b. '3' - 2 = 1
        - you cannot perform subtraction on strings so javascript converts '3' into a number and does numerical subtraction
    c. 3 + null = 3
        - when null is numerically converted it becomes 0
    d. '3' + null = 3null
        - the string concatonation of 3 and null is 3null
    e. true + 3 = 4
        - the numerical conversion of true is 1
    f. false + null = 0
        - the numerical conversion of false and null are both 0
    g. '3' + undefined = 3undefined
        - undefined becomes a string through string conversion 
    h. '3' - undefined = NaN
        - the numerical conversion of undefined is NaN

14) Comparison
    a. '2' > 1 = true
        - '2' becomes the number 2 
    b. '2' < '12' = false
        - lexigraphically 2 is not less than 1
    c. 2 == '2' = true
        - with the type conversion these are equivalent
    d. 2 === '2' = false
        - these are not equal without the type conversion
    e. true == 2 = false
        - true is numerically converted to 1, thus 1 is not equivalent to 2
    f. true === Boolean(2) = true
        - any value other than 0, null, undefined, NaN, "" when boolean converted is true therefore these are strictly equivalent

15) Explain the difference between the == and === operators.
    - == is a loose equivalency operator. This means that javascript will make a type conversion to try to compare the two ends. === is a strict equivalency operator. This means javascript will compare the two ends without a type conversion.

16) Given the above Object, write a for...in loop that will iterate through it and print out the value of the property if the property starts with the letter r, or if the value of that property is an odd number.  (This should be in a JS file part2-question16.js)
    - [question 16 code](part2/part2-question16.js)

17) If the function above is called with the following parameters modifyArray([1,2,3], doSomething), what will be the result? Briefly walk through how you arrived at that result. (This should be in your part2.md). Here we are passing in a function as a parameter, however we can also return a function from another function just as easily, you're encouraged to play around with callbacks as they are used heavily in frontend JS development. 
    - The result will be an array of [2, 4, 6]. The doSomething function is being referrenced by callback in the modifyArray function. Each value in the array is being passed to doSomething which will multiply the value by 2 then push that value into newArr.

18) The above program only prints out the time once when executed. Modify this code such that the program prints out the current time every second.  (This should be a JS file - part2-question18.js)
    - [question 18 code](part2/part2-question18.js)

19) What is the output of the above code? (This should be in your part2.md)
    - 1 4 3 2