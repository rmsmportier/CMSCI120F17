---
title       : Homework 3
description : CMSCI 120 Homework


--- type:NormalExercise lang:python xp:100 skills:1 key:fd2d31317f
## Combining Expressions and Building Blocks (1)

We can use the combination of expressions and the output building block to print designs to our screen.  Follow the instructions below.

*** =instructions
- Replace the ____ with "\*" in each open expression.

*** =hint
- Be sure to use "" around * to indicate that this is string data type

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Print the first line of design
print(____ * 19)

# Print the second line of design
print(____ + ' ' * 17 + ____)

# Print the third line of design
print(____ + ' ' * 17 + ____)

# Print the fourth line of design
print(____ * 19)

```

*** =solution
```{python}
# Print the first line of design
print("*" * 19)

# Print the second line of design
print("*" + ' ' * 17 + "*")

# Print the third line of design
print("*" + ' ' * 17 + "*")

# Print the fourth line of design
print("*" * 19)

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_function("print", index=1,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the first call to print.")
            
test_function("print", index=2,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the second call to print.")
            
test_function("print", index=3,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the third call to print.")
            
test_function("print", index=4,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the fourth call to print.")
            
success_msg('Excellent work!!  Let\'s try another.')

```


--- type:NormalExercise lang:python xp:100 skills:1 key:5da1240b9e
## Combining Expressions and Building Blocks (2)

We can create flexibility in our program by using variables to store some of the values we previously typed.  

Let's store the character to one variable, and the number of times to repeat to another.  

You may not follow everything that is occurring with the print statements, but I encourage you to review each one of them.  Focus on how changing what is assigned to the variable changes the outcome.  

See if you can understand the choice that was made in the second and third print statements for how many times to repeat the single space.

*** =instructions
- Assign the value '\*' to variable *a*; be sure to include the '' that indicate string type
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
print(a * b)

# Print the second line of design
print(a + ' ' * (b-2) + a)

# Print the third line of design
print(a + ' ' * (b-2) + a)

# Print the fourth line of design
print(a * b)

```

*** =solution
```{python}
# Assign character to variable a
a = "*"

# Assign number of times to repeat to variable b
b = 19

# Print the first line of design
print(a * b)

# Print the second line of design
print(a + ' ' * (b-2) + a)

# Print the third line of design
print(a + ' ' * (b-2) + a)

# Print the fourth line of design
print(a * b)

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
            incorrect_msg = "Check the string you specified for the second call to print.")
            
test_function("print", index=3,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the third call to print.")
            
test_function("print", index=4,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the fourth call to print.")
            
success_msg('Excellent work!!  You are doing well.')

```


--- type:NormalExercise lang:python xp:100 skills:1 key:252d420681
## Variables Create Flexibility

We can now easily modify our earlier program to print a different character, and a different number of times to the screen.  This time I have created and run code that produced the design shown.  

Modify the values in *a* and *b* to create the same design.  

I will save you the effort, and tell you that there are 37 $ in the first row of design.

*** =instructions
- Modify the value in variable *a*
- Modify the value in variable *b*

*** =hint
- Use assignment operator as we have done previously, and string indicator for the character to assign

*** =pre_exercise_code
```{python}
# Assign value to variable a
a = "$"

# Assign value to variable b
b = 37

# Print the first line of design
print(a * b)

# Print the second line of design
print(a + ' ' * (b-2) + a)

# Print the third line of design
print(a + ' ' * (b-2) + a)

# Print the fourth line of design
print(a * b)

```

*** =sample_code
```{python}
# Assign value to variable a
a ____ ____

# Assign value to variable b
b ____ ____

# Print the first line of design
print(a * b)

# Print the second line of design
print(a + ' ' * (b-2) + a)

# Print the third line of design
print(a + ' ' * (b-2) + a)

# Print the fourth line of design
print(a * b)

```

*** =solution
```{python}
# Assign value to variable a
a = "$"

# Assign value to variable b
b = 37

# Print the first line of design
print(a * b)

# Print the second line of design
print(a + ' ' * (b-2) + a)

# Print the third line of design
print(a + ' ' * (b-2) + a)

# Print the fourth line of design
print(a * b)

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
            incorrect_msg = "Check the string you specified for the second call to print.")
            
test_function("print", index=3,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the third call to print.")
            
test_function("print", index=4,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the first call to print.")

success_msg('Nice job!!  You are now programming in Python with 2 of 6 building blocks')

```

--- type:NormalExercise lang:python xp:100 skills:1 key:7522f73f67
## Variables Create Flexibility (2)

Let's modify our program even further.   

The new design we want to create is displayed, with 42 occurrences of # on first line.  

Let's reduce the identical second and third print statements down to one print statement.  

What character could we put in place of ____ in our new print statement that will ensure we get identical output but on different lines? 

What value would we need to assign to *end* argument to make everything work correctly?

*** =instructions
- Assign the value to variable *a*
- Assign the value to variable *b*

*** =hint
- Use assignment operator as we have done previously, and string indicator for the character to assign
- This time there are 42 occurrences of # on first line

*** =pre_exercise_code
```{python}
# Assign value to variable a
a = "#"

# Assign value to variable b
b = 42

# Print the first line of design
print(a * b)

# Print the second and third lines of design.  Specify the character needed at end of each line, and the value for end=
print((a + ' ' * (b-2) + a + "\n") * 2, end = "")

# Print the fourth line of design
print(a * b)

```

*** =sample_code
```{python}
# Assign value to variable a
a ____ ____

# Assign value to variable b
b ____ ____

# Print the first line of design
print(a * b)

# Print the second and third lines of design.  Specify the character needed at end of each line, and the value for end=
print((a + ' ' * (b-2) + a + ____) * 2, end = ____)

# Print the fourth line of design
print(a * b)

```

*** =solution
```{python}
# Assign value to variable a
a = "#"

# Assign value to variable b
b = 42

# Print the first line of design
print(a * b)

# Print the second and third lines of design.  Specify the character needed at end of each line, and the value for end=
print((a + ' ' * (b-2) + a + "\n") * 2, end = "")

# Print the fourth line of design
print(a * b)

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
            incorrect_msg = "Check the string you specified for the second call to print.  Think about the character that forces Python to new line, and the character that ensures print does not automatically go to new line at end.")
            
test_function("print", index=3,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the third call to print.")

success_msg('Nice work; keep it going')

```

--- type:NormalExercise lang:python xp:100 skills:1 key:3276474c49
## Variables Create Flexibility (3)

Let's modify our program even further.   

Now we are going to support a variable number of rows.  

We first print the line with our character; in this case there are 57 values in the first row.  

We then repeat some number of times the row with the character only at the beginning and end, and spaces in between.  

You will need to determine the total number of rows.  Set variable *c* to this number.  

In the print statement for number of internal lines, you will adjust *c* to represent number of rows needed internal to design.  The total number of rows will include the first and last printed, so determine how many rows are needed inside the box.

*** =instructions
- Assign the value to variable *a*
- Assign the value to variable *b*
- Assign the value to variable *c*

*** =hint
- Use assignment operator as we have done previously, and string indicator for the character to assign

*** =pre_exercise_code
```{python}
# Assign value to variable a
a = "&"

# Assign value to variable b
b = 57

# Assign value to variable c
c = 8

# Print the first line of design
print(a * b)

# Print the these lines the number of times in c minus the 2 rows printed at start and finish.
print((a + ' ' * (b-2) + a + "\n") * (c - 2), end = "")

# Print the fourth line of design
print(a * b)

```

*** =sample_code
```{python}
# Assign value to variable a
a ____ ____

# Assign value to variable b
b ____ ____

# Assign value to variable c
c ____ ____

# Print the first line of design
print(a * b)

# Print these lines the number of times needed to create c rows, including the first and last line.
print((a + ' ' * (b-2) + a + "\n") * (____ - ____), end = "")

# Print the fourth line of design
print(a * b)

```

*** =solution
```{python}
# Assign value to variable a
a = "&"

# Assign value to variable b
b = 57

# Assign value to variable c
c = 8

# Print the first line of design
print(a * b)

# Print these lines the number of times needed to create c rows, including the first and last line.
print((a + ' ' * (b-2) + a + "\n") * (c - 2), end = "")

# Print the fourth line of design
print(a * b)

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

test_object("c",
            undefined_msg = "Do not remove assignment statement for variable *c*.",
            incorrect_msg = "Check the value you assigned to variable *c*.")

test_function("print", index=1,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the first call to print.")

test_function("print", index=2,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the second call to print.  Think about the character that forces Python to new line, and the character that ensures print does not automatically go to new line at end.")
            
test_function("print", index=3,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the third call to print.")

success_msg('Excellent work!!  You should be seeing the tremendous value in using variables with expressions and functions like *print*.  We have learned only a little syntax, yet you are creating some highly flexible programs.')

```

--- type:NormalExercise lang:python xp:100 skills:1 key:32b15d0301
## Variables Create Flexibility (4)

Let's go even further with what we are doing.   

This time, let's create 2 new variables that will contain our 2 different designs we are printing.  Let's call these variables *border* and *internal*.

The design we are creating is the same as the previous exercise.  This time, we want the print statements to use our new variables.

The first and last print statements should use *border* while the print statement for the internal should use variable *internal*.

*** =instructions
- Assign the value to variable *a*
- Assign the value to variable *b*
- Assign the value to variable *c*
- Assign the product of *a* and *b* to variable *border*
- Assign the concatenated result of *a*, " " repeated (b-2) times, *a*, and newline character to create variable *internal*

*** =hint
- Use assignment operator as we have done previously, and string indicator for the character to assign
- Count the number of rows and columns
- Make sure you are using correct character
- Look back at previous exercises for help

*** =pre_exercise_code
```{python}
# Assign value to variable a
a = "&"

# Assign value to variable b
b = 57

# Assign value to variable c
c = 8

# Print the first line of design
print(a * b)

# Print these lines the number of times in c minus an adjusted number of rows.
print((a + ' ' * (b-2) + a + "\n") * (c - 2), end = "")

# Print the fourth line of design
print(a * b)

```

*** =sample_code
```{python}
# Assign value to variable a
a ____ ____

# Assign value to variable b
b ____ ____

# Assign value to variable c
c ____ ____

# Assign value to variable border
border ____ ____ * ____

# Assign value to variable internal
internal ____ a ____ ' ' ____ (b-2) ____ a ____ "\n"

# Print the first line of design
print(____)

# Print the these lines the number of times in c minus the 2 rows printed at start and finish.
print(____ * (c - 2), end = "")

# Print the fourth line of design
print(____)

```

*** =solution
```{python}
# Assign value to variable a
a = "&"

# Assign value to variable b
b = 57

# Assign value to variable c
c = 8

# Assign value to variable border
border = a * b

# Assign value to variable internal
internal = a + ' ' * (b-2) + a + "\n"

# Print the first line of design
print(border)

# Print the these lines the number of times in c minus the 2 rows printed at start and finish.
print(internal * (c - 2), end = "")

# Print the fourth line of design
print(border)

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

test_object("c",
            undefined_msg = "Do not remove assignment statement for variable *c*.",
            incorrect_msg = "Check the value you assigned to variable *c*.")

test_object("border",
            undefined_msg = "Do not remove assignment statement for variable *border*.",
            incorrect_msg = "Check the value you assigned to variable *border*.")

test_object("internal",
            undefined_msg = "Do not remove assignment statement for variable *internal*.",
            incorrect_msg = "Check the value you assigned to variable *internal*.")

test_function("print", index=1,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the first call to print.")

test_function("print", index=2,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the second call to print.  Think about the character that forces Python to new line, and the character that ensures print does not automatically go to new line at end.")
            
test_function("print", index=3,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the third call to print.")

success_msg('Excellent work!!  You are now programming in Python, and have mastered 2 of the 6 building blocks including expressions and the *print* function.')

```


