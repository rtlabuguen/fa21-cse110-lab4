1. Console will output 3. i is declared as 'var', therefore it exists within the scope of the entire function. i is incremented until it is equal to prices.length (3)
2. Console will output 150. the last time discountedPrice is updated is when i=2, which is the third index of discountedPrices, therefore discountedPrice is set to be 
   ```
    var discountedPrice = prices[2] * (1-0.5);
    = 300 * (0.5)
    = 150
    ```
3. Console will output 150. The discountedPrice variable is the same as in question 2, thus the program will round (discountedPrice * 100) to the nearest integer, which would be 15000, then divide by 100, setting finalPrice to 150
4. The function will return the array named "discounted." Since javascript dynamically deals with data types, there will be no error and the function will successfully return the array
5. The program will encounted an error because the variable "i" is not declared in this scope. "i" is declared as *let*, meaning that it exists only within the code block in which it is declared. Therefore, i does not exist in line 12. 
6. The same as question 5, the variable "discountedPrice" is declared with keyword *let*, therefore it only exists within the loop in which it is declared
7. The console will output 150. While the variable "finalPrice" is declared with the *let* keyword, it is inside the *discountedPrices* function block, therefore the variable still exists in line 15, and will print with the value that it is assigned to on line 8.
8. The function will return an array that contains all the discounted prices that were calculated in the *discountedPrices* function. While the variable "discounted" is declared as *let* and within the scope of the function, the function returns this array and it can still be accessed if it is set to a new variable at the function call.
9. The console will encounted an error because i is declared with the keyword *let* thus will only exist within the scope of the for loop in which it is declared 
10. The console will output 3. The variable "length" is declared as using the keyword *const*, therefore it exists only within the block it is declared, which is the function *discountedPrices*. Therefore the variable exists in line 12 with the same value in which it is assigned at line 4, which is the length of the prices array that is passed through.
11. The function will still return an array that contains the discounted prices that were calculated in the for loop of the *discountPrices* function. Even though the variable "discounted" is declared as *const*, it is never re-assigned, i.e.( discounted = prices). Pushing values into this array does not re-assign the variable, therefore it is still a valid operation. 
12. A. student.name
    B. student["Grad Year"]
    C. student.greeting()
    D. student["Favorite Teacher"].name
    E. student.courseLoad[0]
13. A. '32', js converted integer 2 to a string and concatenated it to '3'
    B. 1, js converted string '3' to an integer and performed integer subtraction
    C. 3, null is converted to integer 0 and integer addition is performed
    D. '3null' null is converted to a string 'null' and string concatenation is performed
    E. 4, true is converted to integer 1 and integer addition is performed
    F. 0, false and null are converted to integer 0 and addition is performed
    G. '3undefined', undefined is converted into a string and string concatenation is performed
    H. NaN, js tried to convert 3 to an integer to perform integer subtraction but undefined has no number conversion so answer is not a number
14. A. True, '2' is converted to an integer and integer comparison is performed
    B. false, the first two character are performed and '2' appears lexicographically after '1'
    C. true, string '2' is converted to integer and integer equality is checked
    D. false, the two inputs are of different types
    E. false, true is converted to integer 1
    F. true, the two inputs are of same type and boolean(2) results in true since it is not "empty"
15. == is a non-strict equality check and can perform casting, === is a strict equality check, meaning that the two inputs must be of same data type to ever be considered equal
17. This program first executes line 13, which calls the *modifyArray* function. Passed into this function is the array containing the three values, and the callback function; *doSomething*. Inside the *modifyArray* function, we define a new *const* array called "newArr", then we iterate through every element of the array with a for loop. Inside the for loop, we push an item into the new array that we declared. pushed into this array is the value that is returned when calling the *callback(array[i])*. Therefore, for each element in the array, we call the callback function, which returns double of the value that is passed, then push the return value into the new array, *newArr*. After doing this for every element that is inside the array passed into the *modifyArray* function, we return *newArr*. Therefore, the value that is returned from the function *modifyArray* is [2,4,6]. 
19. This program calls the function *printNums*. In this function, it immediately prints '1' to the console, then prints '2', but after 1 second, then prints 3, but after 0 seconds, then immediately prints 4. Therefore, the progrma will print 1 then 4, because these calls have no delay, then it will print 3 because it has the shortest delay, then will print 2 because it has the longest delay. 

