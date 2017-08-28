---
title       : Homework 2
description : CMSCI 120 Homework


--- type:NormalExercise lang:python xp:100 skills:1 key:b66b5626af
## First Program

When learning any new programming language, one of the first programs is what is called "Hello World!".  All programming languages rely on 6 common building blocks to create programs whether simple or complex.  We are going to use 1 of those 6 primary building blocks to create output to the screen.

Complete instructions in the script.py to the right.

*** =instructions
- Complete the *print* function with the phrase 'Hello World!'
- Press Submit Answer

*** =hint
- Replace Hello World! for the blanks in the print function
- Be sure to keep the " ", and to include ! at end of the phrase

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Say Hello World!
print("____ ____")

```

*** =solution
```{python}
# Correct the syntax error below
print("Hello World!")
```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_function("print", index=1,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified, and make sure the case/punctuation match to what was requested.")
            
success_msg('Nice job!!  Although a very simple program, that one line is a functional program.  Any time you want to communicate output from the computer, you would use a building block designed for output.  In Python, this is the *print()* function.  Anything we place inside the "" will print to the screen.')

```


--- type:NormalExercise lang:python xp:100 skills:1 key:a4fcdfba6a
## Practice Your Data Type Understanding

Let's use the *print()* function to practice understanding of data type.

For each variable in the scrpt.py, inside the subsequent *print()* indicate the data type you believe it is.

Then use the *type()* function to validate your result.

*** =instructions
- Look at what has been assigned to variable *a* with =.  What data type is variable *a*?  Your choices are *float*, *int*, *str*.
- Complete the *print* function with the data type
- Complete the call to *type()* by placing the variable name *a* inside the parentheses.  This will tell us the true data type.
- Press Submit Answer

*** =hint
- Remember to look for numbers alone with no "" (int), numbers with decimal point (float), or "" to indicate (str)

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Value is assigned to variable a
a = 987

# Complete print() to indicate type you believe variable a to be
print("I believe a is ____")

# Complete call to type() by replacing a inside ().  This will validate data type of a
print(type(____))

```

*** =solution
```{python}
# Value is assigned to variable a
a = 987

# Complete print() to indicate type you believe variable a to be
print("I believe a is int")

# Complete call to type() by replacing a inside ().  This will validate data type of a
print(type(a))

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_object("a",
            undefined_msg = "Do not remove assignment statement for variable *a*.",
            incorrect_msg = "Do not remove assignment statement for variable *a*.")

test_function("print", index=1,
            not_called_msg = "Did you remove the first call to print?",
            incorrect_msg = "Check the data type you indicated in print statement.  Look at hint to help you identify.")

test_function("print", index=2,
            not_called_msg = "Did you remove the second call to print?",
            incorrect_msg = "Check what you passed to second print.  This should be call to type() function and variable")

test_function("type",
            not_called_msg = "Did you remove the call to type?",
            incorrect_msg = "Be sure to use only the variable name inside () in call to type")

success_msg('Correct!!  This simple program enables us to instruct Python on determining the data type of a variable, and printing result to screen.  Knowing the data type is important as we begin to combine expressions as some combinations of data type are not allowed.  Our variable a is an int because there were numbers only and no "".  Let\'s keep going.')

```

--- type:NormalExercise lang:python xp:100 skills:1 key:ce9aa5c69c
## Practice Your Data Type Understanding (2)

Let's use the *print()* function to practice understanding of data type.

For each variable in the script.py, inside the subsequent *print()* indicate the data type you believe it is.

Then use the *type()* function to validate your result.

*** =instructions
- Look at what has been assigned to variable *a* with =.  What data type is variable *a*?  Your choices are *float*, *int*, *str*.
- Complete the *print* function with the data type
- Complete the call to *type()* by placing the variable name *a* inside the parentheses.  This will tell us the true data type.
- Press Submit Answer

*** =hint
- Remember to look for numbers alone with no "" (int), numbers with decimal point (float), or "" to indicate (str)

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Value is assigned to variable a
a = 987.456

# Complete print() to indicate type you believe variable a to be
print("I believe a is ____")

# Complete call to type() by replacing a inside ().  This will validate data type of a
print(type(____))

```

*** =solution
```{python}
# Value is assigned to variable a
a = 987.456

# Complete print() to indicate type you believe variable a to be
print("I believe a is float")

# Complete call to type() by replacing a inside ().  This will validate data type of a
print(type(a))

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_object("a",
            undefined_msg = "Do not remove assignment statement for variable *a*.",
            incorrect_msg = "Do not remove assignment statement for variable *a*.")

test_function("print", index=1,
            not_called_msg = "Did you remove the first call to print?",
            incorrect_msg = "Check the data type you indicated in print statement.  Look at hint to help you identify.")

test_function("print", index=2,
            not_called_msg = "Did you remove the second call to print?",
            incorrect_msg = "Check what you passed to second print.  This should be call to type() function and variable.")

test_function("type",
            not_called_msg = "Did you remove the call to type?",
            incorrect_msg = "Be sure to use only the variable name inside () in call to type")

success_msg('Correct!!  The data type this time was float because we used numbers and decimal point with no "".  Let\'s keep going.')

```

--- type:NormalExercise lang:python xp:100 skills:1 key:0e3cdebcc2
## Practice Your Data Type Understanding (3)

Let's use the *print()* function to practice understanding of data type.

For each variable in the script.py, inside the subsequent *print()* indicate the data type you believe it is.

Then use the *type()* function to validate your result.

*** =instructions
- Look at what has been assigned to variable *a* with =.  What data type is variable *a*?  Your choices are *float*, *int*, *str*.
- Complete the *print* function with the data type
- Complete the call to *type()* by placing the variable name *a* inside the parentheses.  This will tell us the true data type.
- Press Submit Answer

*** =hint
- Remember to look for numbers alone with no "" (int), numbers with decimal point (float), or "" to indicate (str)

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Value is assigned to variable a
a = "987 // 2"

# Complete print() to indicate type you believe variable a to be
print("I believe a is ____")

# Complete call to type() by replacing a inside ().  This will validate data type of a
print(type(____))

```

*** =solution
```{python}
# Value is assigned to variable a
a = "987 // 2"

# Complete print() to indicate type you believe variable a to be
print("I believe a is str")

# Complete call to type() by replacing a inside ().  This will validate data type of a
print(type(a))

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_object("a",
            undefined_msg = "Do not remove assignment statement for variable *a*.",
            incorrect_msg = "Do not remove assignment statement for variable *a*.")

test_function("print", index=1,
            not_called_msg = "Did you remove the first call to print?",
            incorrect_msg = "Check the data type you indicated in print statement.  Look at hint to help you identify.")
            
test_function("print", index=2,
            not_called_msg = "Did you remove the second call to print?",
            incorrect_msg = "Check what you passed to second print.  This should be call to type() function and variable.")

test_function("type",
            not_called_msg = "Did you remove the call to type?",
            incorrect_msg = "Be sure to use only the variable name inside () in call to type")

success_msg('Correct!!  It does not matter how many arithmetic operations we place inside the assignment for *a* when we place them inside "".  These will always indicate the data type is str.')

```


--- type:NormalExercise lang:python xp:100 skills:1 key:54870e9736
## Combining Variables

We can combine values stored in different variables.  Let's start with a calculation program.  

We want to find the sum, difference, product, and remainder between 2 variables *a* and *b*.

Use the correct arithmetic operator to complete the requested operation in the script.py.


*** =instructions
- Add the value in *a* to the value in *b*
- Subtract the value in *b* from the value in *a*
- Multiply the value in *a* by the value in *b*
- Use the modulus operator to find the remainder when we divide the value in *a* by the value in *b*

*** =hint
- Replace each requested operation with the Python operator for that arithmetic result

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Variable a is assigned value
a = 5876

# Variable b is assigned value
b = 432

# Add the value in a to the value in b
print(a ____ b)

# Subtract the value in b from the value in a
print(a ____ b)

# Multiply the value in a by the value in b
print(a ____ b)

# Find the remainder when dividing a by b
print(a ____ b)

```

*** =solution
```{python}
# Variable a is assigned value
a = 5876

# Variable b is assigned value
b = 432

# Add the value in a to the value in b
print(a + b)

# Subtract the value in b from the value in a
print(a - b)

# Multiply the value in a by the value in b
print(a * b)

# Find the remainder when dividing a by b
print(a % b)


```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_object("a",
            undefined_msg = "Do not remove assignment statement for variable *a*.",
            incorrect_msg = "Do not remove assignment statement for variable *a*.")

test_object("b",
            undefined_msg = "Do not remove assignment statement for variable *b*.",
            incorrect_msg = "Do not remove assignment statement for variable *b*.")

test_function("print", index=1,
            not_called_msg = "Did you remove the first call to print?",
            incorrect_msg = "Check the operator you used to *add* the two values.")
            
test_function("print", index=2,
            not_called_msg = "Did you remove the second call to print?",
            incorrect_msg = "Check the operator you used to *subtract* the two values.")

test_function("print", index=3,
            not_called_msg = "Did you remove the third call to print?",
            incorrect_msg = "Check the operator you used to *multiply* the two values.")

test_function("print", index=4,
            not_called_msg = "Did you remove the fourth call to print?",
            incorrect_msg = "Check the operator you used to find remainder when dividing the two values.  The operator is called a modulus.")

success_msg('Excellent work!!  Let\'s keep going.')

```


--- type:NormalExercise lang:python xp:100 skills:1 key:c6599fdcf9
## Combining Expressions to Create Variables

Combining expressions and building blocks is how we create programs.  Let's create a program that takes a value in feet and converts to inches, printing the result to the screen.  For this program, we need 2 building blocks: expressions and output.

*** =instructions
- Assign the value 12 to variable *a*.  This value is in feet.
- Convert the value in variable *a* from feet to inches by replacing conversion factor in the expression.  Assign the result to variable *b*.
- Print the result of the calculation to the screen.

*** =hint
- Remember that assignment statements require an assignment operator to change value in variable.  What is that operator in Python?
- You will need to combine assignment operator and arithmetic operation to assign correct value to b

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Assign the value 12 to a
a ____ ____

# Convert the value in a to inches with appropriate conversion factor, and assign result to b
b ____ a ____ 12

# Print the result to screen
print("Converting",a,"from feet to inches results in",b)

```

*** =solution
```{python}
# Assign the value 12 to a
a = 12

# Convert the value in a to inches with appropriate conversion factor, and assign result to b
b = a * 12

# Print the result to screen
print("Converting",a,"from feet to inches results in",b)


```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_object("a",
            undefined_msg = "Do not remove assignment statement for variable *a*.",
            incorrect_msg = "Check the value you assigned to variable *a*.")

test_object("b",
            undefined_msg = "Do not remove assignment statement for variable *b*.",
            incorrect_msg = "Check the value you assigned to variable *b*.")

test_function("print", index=1,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "You do not need to change the syntax for the call to print.")
            
success_msg('Excellent work!!  Let\'s try one more program.')

```


--- type:NormalExercise lang:python xp:100 skills:1 key:52e57952de
## Combining Variables and Expressions

I have created 2 variables *width* and *height*.  You can use commands you have learned in the iPython shell to evaluate the current value of each of these variables.  Fill in the operator needed to produce the value specified for each of the following.

*** =instructions
- apply operator to the operands *width* and 4; result should be 4
- apply operator to the operands *width* and 4; result should be 68
- apply operator to the operands *height* and 2.5; result should be 4.8
- apply operator to the operands *height* and 12; result should be 0.0
- apply operators to the operands 10, 2, and 8; result should be 26

*** =hint
- Think about the operators we have learned, what the value and type of each operand is, and try to find an operator that produceses requested results.

*** =pre_exercise_code
```{python}
width = 17
height = 12.0
```

*** =sample_code
```{python}
# Produce result of 4
print(width ____ 4)

# Produce result of 68
print(width ____ 4)

# Produce result of 4.8
print(height ____ 2.5)

# Produce result of 0.0
print(height ____ 12)

# Produce result of 26
print(10 ____ 2 ____ 8)

```

*** =solution
```{python}
# Produce result of 4
print(width // 4)

# Produce result of 68
print(width * 4)

# Produce result of 4.8
print(height / 2.5)

# Produce result of 0.0
print(height - 12)

# Produce result of 26
print(10 + 2 * 8)

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_function("print", index=1,
            not_called_msg = "Did you remove the first call to print?",
            incorrect_msg = "Check the operator you specified for the first call to print.")
            
test_function("print", index=2,
            not_called_msg = "Did you remove the second call to print?",
            incorrect_msg = "Check the operator you specified for the second call to print.")
            
test_function("print", index=3,
            not_called_msg = "Did you remove the third call to print?",
            incorrect_msg = "Check the operator you specified for the third call to print.")
            
test_function("print", index=4,
            not_called_msg = "Did you remove the fourth call to print?",
            incorrect_msg = "Check the operator you specified for the fourth call to print.")
            
test_function("print", index=5,
            not_called_msg = "Did you remove the fifth call to print?",
            incorrect_msg = "Check the operator you specified for the fifth call to print.")
            
success_msg("Excellent work!!")

```

--- type:NormalExercise lang:python xp:100 skills:1 key:23117a3b50
## Combining Variables (2)

We can combine values stored in different variables for other data types.  Let's focus on strings, and combine in a variety of way.

Use the correct operator to complete the requested operation in the script.py.


*** =instructions
- We want to attach the values in *a* and *b* together to create a new combined string.  Separate the 2 pieces with a space.  In computer science, this process of attaching strings is called concatenation.
- We want to take the value in *a* and repeat it 5 times.  In computer science, this process is called replication.
- We want to take the value in *a*, repeat it twice, and combine with the value in *b*.  

*** =hint
- Replace each requested operation with the Python operator for that result

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Variable a is assigned value
a = "This is a string"

# Variable b is assigned value
b = "This is another string"

# Concatenate the value in a to the value in b, separate them with a space
print(a ____ " " ____ b)

# Repeat the value in a, 5 times
print(a ____ 5)

# Repeat the value in a twice, and combine with the value in b.  
print(a ____ ____ ____ b)

```

*** =solution
```{python}
# Variable a is assigned value
a = "This is a string"

# Variable b is assigned value
b = "This is another string"

# Add the value in a to the value in b, separate them with a space
print(a + " " + b)

# Repeat the value in a, 5 times
print(a * 5)

# Repeat the value in a twice, and combine with the value in b.  
print(a * 2 + b)

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_object("a",
            undefined_msg = "Do not remove assignment statement for variable *a*.",
            incorrect_msg = "Do not remove assignment statement for variable *a*.")

test_object("b",
            undefined_msg = "Do not remove assignment statement for variable *b*.",
            incorrect_msg = "Do not remove assignment statement for variable *b*.")

test_function("print", index=1,
            not_called_msg = "Did you remove the first call to print?",
            incorrect_msg = "Check the operator you used to concatenate the values.")
            
test_function("print", index=2,
            not_called_msg = "Did you remove the second call to print?",
            incorrect_msg = "Check the operator you used to replicate the value in *a*.")

test_function("print", index=3,
            not_called_msg = "Did you remove the third call to print?",
            incorrect_msg = "Check the operators you used to replicate and concatenate values.  Be sure to indicate the number of times to replicate.")

success_msg('Excellent work!!  Let\'s keep going.')

```


--- type:NormalExercise lang:python xp:100 skills:1 key:dd3c482686
## Combining Expressions and Building Blocks (2)

Combining expressions and building blocks is how we create programs.  Let's create a program that takes the values of 2 string variables, and the value of 2 integer variables.  Create a string that replicates the first string by the first integer value, the second string by the second integer value, and concatenates the results.

*** =instructions
- Assign the value "I think I am getting the hang of this!!" to variable *a*
- Assign the value 5 to variable *b*
- Assign the value "So many strings, so little time." to variable *c*
- Assign the value 2 to variable *d*

*** =hint
- Look back at what you did with previous exercises.  The difference on this one is that we are using only variables.

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Assign the value to variable a
a ____ ____


# Assign the value to variable b
b ____ ____

# Assign the value to variable c
c ____ ____

# Assign the value to variable d
d ____ ____

# Print the requested result to screen
print(a ____ ____ + ____ ____ d)

```

*** =solution
```{python}
a = "I think I am getting the hang of this!!"

# Assign the value to variable b
b = 5

# Assign the value to variable c
c = "So many strings, so little time."

# Assign the value to variable d
d = 2

# Print the requested result to screen
print(a * b + c * d)

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_object("a",
            undefined_msg = "Did you create variable *a*.",
            incorrect_msg = "Check the value you assigned to variable *a*.")

test_object("b",
            undefined_msg = "Did you create variable *b*.",
            incorrect_msg = "Check the value you assigned to variable *b*.")

test_object("c",
            undefined_msg = "Did you create variable *c*.",
            incorrect_msg = "Check the value you assigned to variable *c*.")

test_object("a",
            undefined_msg = "Did you create variable *d*.",
            incorrect_msg = "Check the value you assigned to variable *d*.")

test_function("print", index=1,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Look at instructions and concatenate the pieces as described.")
            
success_msg('Excellent work!!  Let\'s try one more program.')

```

