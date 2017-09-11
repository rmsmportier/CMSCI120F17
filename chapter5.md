---
title       : Homework 4
description : CMSCI 120 Homework


--- type:NormalExercise lang:python xp:100 skills:1 key:fd2d31317f
## Built In Functions

The concept of functions is a powerful part of programming in any programming language.  A function is simply a name to group a defined sequence of instructions.

We are familiar now with concept of "function factory", where we pass a value(s) to the function, and a result is produced.  That value passed could be a prompt that enables us to *input* commands.  It can be displaying values to screen using *print* function.  It can be typecasting, changing the type of a variable using *int*, *float*, and *str*.

This week we are going to explore available Python functions.

To start, we need to see what functions are available when we first start Python.  We refer to these as built-in functions; they are built-in to the initial Python setup.

Run the code on the right to get a listing of all available functions.  You can do this by highlighting both lines, and then pressing Ctrl-Enter.  

*** =instructions
- Generate the listing of available functions by entering highlighting both lines, and pressing Ctrl-Enter at same time.  Once you have looked through the listing, press *Submit Answer*

*** =hint
- You do not need to change anything.  Once you have viewed the listing, you can "Submit Answer"

*** =pre_exercise_code
```{python}

```

*** =sample_code
```{python}
import builtins
dir(builtins)

```

*** =solution
```{python}
import builtins
dir(builtins)

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_function("dir", index=1,
            not_called_msg = "Did you remove or change the call to dir?",
            incorrect_msg = "Make sure you are passing *builtins* to dir function")
            
success_msg("That's it.  *dir* is itself a function that provides a directory or listing of all available functions.  We have to specify what type of listing we want.  *builtins* indicates that we want those functions that are part of base Python.  Notice the beginning of the listing contains names that align with error messages we have seen like NameErrors.  The first part of the list indicates all existing runtime errors in Python.  For now, just remember where we found them.  We will come back to this later.")

```

--- type:NormalExercise lang:python xp:100 skills:1 key:5da1240b9e
## Built In Functions (2)

We can use another function *help* to assist us in understanding what any of these functions will do, and how to use the selected function.  Let's try this with a few built-in functions we have not previously used.

In the shell, enter *help(min)* and *help(max)*.  Look at the description to understand what each does. Then complete the following:

*** =instructions
- Pick one of the 2 functions to find the largest value in the group of numbers provided
- Pick one of the 2 functions to find the smallest value in the group of numbers provided
- Use the *min* function with a string "This is a test, this is only a test" to see the *smallest* value in the string.
- Use the *min* function with a string "This is A test, this is only a test" to see the *smallest* value in new string.
- Use the *max* function with a string "This is A test, this is only a test" to see the *smallest* value in new string.
- Pick one of the 2 functions to determine which has greater value in computer, "A" or "a".

*** =hint
- Replace ____ with appropriate function to accomplish stated goal.  You can use *help()* with function name passed to *help* in order to assist in selecting correct function.

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Find the largest value in grouping of numbers
print(____(3, 4, 5, 9, 1, -4))

# Find the smallest value in grouping of numbers
print(____(9, 2, 20, -4, -20, 7))

# Use min with string to find the smallest value in string
print(min("_____"))

# Use min with string to find the smallest value in string
print(min("_____"))

# Use max with string to find the greatest value in string
print(max("____"))

# Identify which has greater value
print(____(("A","a")))

```

*** =solution
```{python}
# Find the largest value in grouping of numbers
print(max(3, 4, 5, 9, 1, -4))

# Find the smallest value in grouping of numbers
print(min(9, 2, 20, -4, -20, 7))

# Use min with string to find the smallest value in string
print(min("This is a test, this is only a test"))

# Use min with string to find the smallest value in string
print(min("This is A test, this is only a test"))

# Use max with string to find the greatest value in string
print(max("This is A test, this is only a test"))

# Identify which has greater value
print(max(("A","a")))

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_function("print", index=1,
            not_called_msg = "Check the directions for this result, and do not remove print function.",
            incorrect_msg = "How do you identify the largest value?")
            
test_function("print", index=2,
            not_called_msg = "Check the directions for this result, and do not remove print function.",
            incorrect_msg = "How do you identify the smallest value?")
            
test_function("print", index=3,
            not_called_msg = "Check the directions for this result, and do not remove print function.",
            incorrect_msg = "Did you enter the correct string?")
            
test_function("print", index=4,
            not_called_msg = "Check the directions for this result, and do not remove print function.",
            incorrect_msg = "Did you enter the correct string?")
            
test_function("print", index=5,
            not_called_msg = "Check the directions for this result, and do not remove print function.",
            incorrect_msg = "Did you enter the correct string?")
            
test_function("print", index=6,
            not_called_msg = "Check the directions for this result, and do not remove print function.",
            incorrect_msg = "How do you identify the largest value?")

test_student_typed("This is a test, this is only a test",not_typed_msg="Are you using correct string value for the longer strings?")

test_student_typed("This is A test, this is only a test",not_typed_msg="Are you using correct string value for the longer strings?")

success_msg('Nice work.  Notice that spaces have lower value than letters, and that capital letters have lower value than lower case letters.  Also notice that for all calls we created a grouping of values by using either () or "" around the full set of values to evaluate.  When the grouping is done using () along with , we have created a tuple.  When we use "", we have created a string with multiple characters.')

```

--- type:NormalExercise lang:python xp:100 skills:1 key:252d420681
## Built In Functions (3)

We will explore a few built in functions designed to work with numeric values.  The functions we will focus on are *sum*, *abs*, *divmod*, and *round*.  For each, explore what the function does by entering *help(function name)* from the shell.

*** =instructions
- Use the *sum* function to sum the numbers 5, 10, 15, 20, 25, 30.  Remember to surround the group of numbers with () so that we are passing a tuple.
- I previously calculated a value that is stored in variable *result*.  You can look at the value by entering the variable name or by using *print* to print the variable name from the shell.  Pick one of the 4 functions (*sum*, *abs*, *divmod*, *round*) to keep only the value portion of the result, and not the sign in front of the number.
- Use *divmod* function with the numbers 28 and 5.  What 2 numbers are created?
- Use *round* and change arguments to round the result of variable *result* to 3 decimal places.

*** =hint
- Use *help* along with function name in () to understand what each function is doing

*** =pre_exercise_code
```{python}
import math
result = 100-2000 * 5/4 + math.pi

```

*** =sample_code
```{python}
# Use sum to calculate the sum of numbers provided
print(sum(____5, 10, ____, 20, ____, 30____))

# Find value in result variable, and print value with no sign
print(____(result))

# Use divmod with numbers indicated
print(____(____, ____))

# Use round to round value in variable result to 3 decimal places
print(____(result, ____))

```

*** =solution
```{python}
# Use sum to calculate the sum of numbers provided
print(sum((5, 10, 15, 20, 25, 30)))

# Find value in result variable, and print value with no sign
print(abs(result))

# Use divmod with numbers indicated
print(divmod(28, 5))

# Use round to round value in variable result to 3 decimal places
print(round(result, 3))

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_function("print", index=1,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the values you passed to *sum*.  Be sure to include () to create tuple.")
            
test_function("print", index=2,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the function you selected.")
            
test_function("print", index=3,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "What values did you pass to *divmod* function?")
            
test_function("print", index=4,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Are you calling round to the correct number of decimal places?")

success_msg('Nice job!!  Did you notice that *divmod* returned a tuple of values, and that those values are the integer division and modulus combined together?')

```

--- type:NormalExercise lang:python xp:100 skills:1 key:7522f73f67
## Built In Functions (4)

There are also several nice functions we can use with string data.  Let's experiment with just 2 of them.  Every character in the computer is actually calculated as a number before converting to binary code.  These decimal equivalents allow us to do arithmetic with characters.  This is something that proves very helpful related to encryption algorithms.  We will go deeper with this topic in lab this week.

*** =instructions
- Use the *ord* function to identify the numeric value for "A"
- Use the *ord* function to identify the numeric value for "a"
- Take the difference between *ord* result for "a" and *ord* result for "A"
- Use the *chr* function to identify the character with decimal value 104
- Use the *chr* function to identify the character with decimal value 122
- Use combination of *ord* and *chr* to identify the character that is 5 greater than the character "E"

*** =hint
- You can use *help(ord)* and *help(chr)* to determine what each does
- Enter the values requested for each function call

*** =pre_exercise_code
```{python}

```

*** =sample_code
```{python}
# Use ord to determine numeric value for "A"
print(____("____"))

# Use ord to determine numeric value for "a"
print(____("____"))

# How far apart are the values "A" and "a"
print(____(____) - ____(____))

# Use chr to identify character for 104
print(____(____))

# Use chr to identify character for 122
print(____(____))

# Combine ord and chr to find character 5 greater than "E"
print(____(____(____) + ____))

```

*** =solution
```{python}
# Use ord to determine numeric value for "A"
print(ord("A"))

# Use ord to determine numeric value for "a"
print(ord("a"))

# How far apart are the values "A" and "a"
print(ord("a") - ord("A"))

# Use chr to identify character for 104
print(chr(104))

# Use chr to identify character for 122
print(chr(122))

# Combine ord and chr to find character 5 greater than "E"
print(chr(ord("E") + 5))

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_function("print", index=1,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the function and value you specified.")

test_function("print", index=2,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the function and value you specified.")
            
test_function("print", index=3,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the function and value(s) you specified.  You need to do arithmetic, so you need to convert character values to decimal.  Which function would do this?  Make sure you are using the character with greatest value first.")

test_function("print", index=4,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the function and value you specified.")
            
test_function("print", index=5,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the function and value you specified.")
            
test_function("print", index=6,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the order in which you are calling functions, and the value you are adding.  Change the 'E' to decimal, add the value, then convert back to character.")
            
success_msg("Nice work.  Did you notice that the difference between 'a' and 'A' is more than 26 characters?  There are actually special characters in-between.")

```


--- type:NormalExercise lang:python xp:100 skills:1 key:4b8e2eab31
## Add In Functions

Before we can use add in functions, we first need to make the function module available to our current work session in Python.

We do this with the *import* statement, followed by the function module name.  

Let's start with the function module *math*.  

We will explore functions available in this function module.  We can do this with the *dir* function as we did earlier in the homework for builtins.  This will list all available functions.  

We can also use *help* with individual functions to learn usage.  When calling *help*, we will need to preface each function name with the module name in a format like *math.pi*.

*** =instructions
- Enter *import math* in order to use the functions in this module
- Identify all possible functions by using *dir* for this function module
- Look up help for function radians, in the shell
- Based on information obtained, print the number of radians in 246 degrees, round to 4 decimal places

*** =hint
- The instructions provide the exact syntax to use to import function module math
- Use *dir()* and put *math* inside ()
- Use *help()* with *math.radians* inside () from shell to identify syntax

*** =pre_exercise_code
```{python}

```

*** =sample_code
```{python}
# Import math into our Python session
____ ____

# Identify all functions available using dir
____(____)

# Convert 246 degrees to radians, round to 4 decimal places
print(____(____.____(246),____))

```

*** =solution
```{python}
# Import math into our Python session
import math

# Identify all functions available using dir
dir(math)

# Convert 246 degrees to radians
print(round(math.radians(246),4))

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_import("math", same_as=True, not_imported_msg="Did you import the *math* module?", incorrect_as_msg="Import is not importing correct function module")

test_function("dir", index=1,
            not_called_msg = "Did you call dir?",
            incorrect_msg = "Check the function you specified for dir.")

test_function("math.radians", index=1,
            not_called_msg = "Did you call function to convert to radians?",
            incorrect_msg = "Check the argument values passed to radians")

test_function("round", index=1,
            not_called_msg = "Did you round the result?",
            incorrect_msg = "Did you round to correct number of digits?")

success_msg("Good work")

```

--- type:NormalExercise lang:python xp:100 skills:1 key:ab29ce1bd4
## Add In Functions (2)

Let's look at two more math module functions.  We have learned about floor division, also called integer division.  We can use a function from *math* to achieve same result.  This function is useful when we have completed complex arithmetic expression evaluation as // only works when we provide two operands.

What if we want to know the smallest integer greater than the value we calculate?  We could choose to round the decimal value to the nearest integer.  While this would work for display purposes, it would not for subsequent calculations that might rely on the integer value.  We can instead use a function from *math*.

If floor gives us the greatest integer less than, what function should we look to find?

*** =instructions
- Enter *import math* in order to use the functions in this module
- Use // to calculate floor division for 24 and 7, assign the result to *a*
- Use the *floor* function from *math* module to do the same, assign the result to *b*
- Now identify a function in *math* module, and use that function to calculate the smallest integer greater than the result of 24/7.  Assign that result to *c*

*** =hint
- The instructions provide the exact syntax to use to import function module *math*
- Use floor division as we have done in class several times
- Then use the *floor* function from *math*
- What is the opposite of floor?

*** =pre_exercise_code
```{python}

```

*** =sample_code
```{python}
# Import math into our Python session
____ ____

# Calculate floor division result
a = ____ // ____
print(a)

# Use the floor function from math module to calculate floor division
b = ____.____(____/____)
print(b)

# What is the smallest integer greater than result?
c = ____.____(____/____)
print(c)

```

*** =solution
```{python}
# Import math into our Python session
import math

# Calculate floor division result
a = 24 // 7
print(a)

# Use the floor function from math module to calculate floor division
b = math.floor(24/7)
print(b)

# What is the smallest integer greater than result?
c = math.ceil(24/7)
print(c)

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_import("math", same_as=True, not_imported_msg="Did you import the *math* module?", incorrect_as_msg="Import is not importing correct function module")

test_student_typed("24\s*//\s*7",not_typed_msg="Did you define floor division // for correct values when creating variable *a*?")

test_object("a",
            undefined_msg = "Don't remove the definition of variable *a*.",
            incorrect_msg = "Check the operator and values used to calculate variable *a*.")

test_object("b",
            undefined_msg = "Don't remove the definition of variable *b*.",
            incorrect_msg = "Check the operator and values used to calculate variable *b*.  You should be using *math.floor*.")
            
test_student_typed("24\s*/\s*7",not_typed_msg="Are you using correct values for calculating *b* with *math.floor*?")

test_object("c",
            undefined_msg = "Don't remove the definition of variable *c*.",
            incorrect_msg = "Check the function and values used to calculate variable *c*.")
            
test_student_typed("24\s*/\s*7",not_typed_msg="Are you using correct values for calculating *c* with *math.ceil*?")

success_msg("Good work")

```

