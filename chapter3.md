---
title       : Homework 2
description : CMSCI 120 Homework


--- type:NormalExercise lang:python xp:100 skills:1 key:b66b5626af
## First Program

When learning any new programming language, one of the first programs is what is called "Hello World!".  All programming languages rely on 6 common building blocks to create programs whether simple or complex.  We are going to use 1 of those 6 primary building blocks to create output to the screen.

Complete instructions in the script.py to the right.

*** =instructions
- Complete the *print* statement with the phrase 'Hello World!'
- Press Submit Answer

*** =hint
- Replace Hello World! for the blanks in the print statement
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

test_output_contains("Hello World!", pattern=False, no_output_msg = "Take a look at the instructions and try again")

success_msg('Nice job!!  Although a very simple program, that one line is a functional program.  Any time you want to communicate output from the computer, you would use a building block designed for output.  In Python, this is the *print()* function.  Anything we place inside the "" will print to the screen.')

```


--- type:NormalExercise lang:python xp:100 skills:1 key:a4fcdfba6a
## Practice Your Data Type Understanding

Let's use the *print()* function to practice understanding of data type.

For each variable in the scrpt.py, inside the subsequent *print()* indicate the data type you believe it is.

Then use the *type()* function to validate your result.

*** =instructions
- Look at what has been assigned to variable *a* with =.  What data type is variable *a*?  Your choices are *float*, *int*, *str*.
- Complete the *print* statement with the data type
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

test_output_contains("I believe a is int", pattern=False, no_output_msg = "Take a look at the instructions and try again")

test_object("a",
            undefined_msg = "Do not remove assignment statement for variable *a*.",
            incorrect_msg = "Do not remove assignment statement for variable *a*.")

test_function("print", index=1,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the data type you indicated in print statement.  Look at hint to help you identify.")
            

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
- Complete the *print* statement with the data type
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

test_output_contains("I believe a is float", pattern=False, no_output_msg = "Take a look at the instructions and try again")

test_object("a",
            undefined_msg = "Do not remove assignment statement for variable *a*.",
            incorrect_msg = "Do not remove assignment statement for variable *a*.")

test_function("print", index=1,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the data type you indicated in print statement.  Look at hint to help you identify.")
            

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
- Complete the *print* statement with the data type
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

test_output_contains("I believe a is str", pattern=False, no_output_msg = "Take a look at the instructions and try again")

test_object("a",
            undefined_msg = "Do not remove assignment statement for variable *a*.",
            incorrect_msg = "Do not remove assignment statement for variable *a*.")

test_function("print", index=1,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the data type you indicated in print statement.  Look at hint to help you identify.")
            

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
- Subtract the value in *a* from the value in *b*
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

# Subtract the value in a from the value in b
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

# Subtract the value in a from the value in b
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
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the operator you used to *add* the two values.")
            
test_function("print", index=2,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the operator you used to *subtract* the two values.")

test_function("print", index=3,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the operator you used to *multiply* the two values.")

test_function("print", index=4,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the operator you used to find remainder when dividing the two values.  The operator is called a modulus.")

success_msg('Excellent work!!  Let\'s keep going.')

```


--- type:NormalExercise lang:python xp:100 skills:1 key:c6599fdcf9
## Combining Expressions and Building Blocks

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


--- type:NormalExercise lang:python xp:100 skills:1 key:fd2d31317f
## Combining Expressions and Building Blocks (2)

We can use the combination of expressions and the output building block to print designs to our screen.  Follow the instructions below.

*** =instructions
- Replace the ____ with "\*" in each open expression below.

*** =hint
- Be sure to use "" around * to indicate that this is str data type

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Print the first line of design
print(____*19)

# Print the second line of design
print(____+' '*17+____)

# Print the third line of design
print(____+' '*17+____)

# Print the fourth line of design
print(____*19)

```

*** =solution
```{python}
# Print the first line of design
print("*"*19)

# Print the second line of design
print("*"+' '*17+"*")

# Print the third line of design
print("*"+' '*17+"*")

# Print the fourth line of design
print("*"*19)

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_function("print", index=1,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the first call to print.")
            
test_function("print", index=2,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the first call to print.")
            
test_function("print", index=3,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the first call to print.")
            
test_function("print", index=4,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the first call to print.")
            
success_msg('Excellent work!!  Let\'s try another.')

```


--- type:NormalExercise lang:python xp:100 skills:1 key:5da1240b9e
## Combining Expressions and Building Blocks (3)

We can create flexibility in our program by using variables to store some of the values we previously typed.  Let's store the character to one variable, and the number of times to repeat to another.  You may not follow everything that is occurring with the print statements, but focus on how changing what is assigned to the variable changes the outcome.

*** =instructions
- Assign the value '\*' to variable *a*; be sure to include the '' that indicate str type
- Assign the value 19 to variable *b*

*** =hint
- Use assignment operator as we have done previously, and string indicator for the character to assign

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Assign character to variable a
a ____ ____

# Assign number of times to repeat to variable b
b ____ ____

# Print the first line of design
print(a*b)

# Print the second line of design
print(a+' '*(b-2)+a)

# Print the third line of design
print(a+' '*(b-2)+a)

# Print the fourth line of design
print(a*b)

```

*** =solution
```{python}
# Assign character to variable a
a = "*"

# Assign number of times to repeat to variable b
b = 19

# Print the first line of design
print(a*b)

# Print the second line of design
print(a+' '*(b-2)+a)

# Print the third line of design
print(a+' '*(b-2)+a)

# Print the fourth line of design
print(a*b)

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
            incorrect_msg = "Check the string you specified for the first call to print.")
            
test_function("print", index=2,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the first call to print.")
            
test_function("print", index=3,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the first call to print.")
            
test_function("print", index=4,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the first call to print.")
            
success_msg('Excellent work!!  You are doing well.')

```


--- type:NormalExercise lang:python xp:100 skills:1 key:252d420681
## Variables Create Flexibility

We can now easily modify our earlier program to print a different character, and a different number of times to the screen.  This time replace the value with variable *a* with '$', and the number of times with 37 for variable *b*.

*** =instructions
- Assign the value '$' to variable *a*; be sure to include the '' that indicate str type
- Assign the value 37 to variable *b*

*** =hint
- Use assignment operator as we have done previously, and string indicator for the character to assign

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Assign character to variable a
a ____ ____

# Assign number of times to repeat to variable b
b ____ ____

# Print the first line of design
print(a*b)

# Print the second line of design
print(a+' '*(b-2)+a)

# Print the third line of design
print(a+' '*(b-2)+a)

# Print the fourth line of design
print(a*b)

```

*** =solution
```{python}
# Assign character to variable a
a = "$"

# Assign number of times to repeat to variable b
b = 37

# Print the first line of design
print(a*b)

# Print the second line of design
print(a+' '*(b-2)+a)

# Print the third line of design
print(a+' '*(b-2)+a)

# Print the fourth line of design
print(a*b)

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
            incorrect_msg = "Check the string you specified for the first call to print.")
            
test_function("print", index=2,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the first call to print.")
            
test_function("print", index=3,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the first call to print.")
            
test_function("print", index=4,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the first call to print.")
            
success_msg('Excellent work!!  You are now programming in Python, and have mastered 2 of the 6 building blocks.')

```


