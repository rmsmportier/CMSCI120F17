---
title       : Lab 2
description : CMSCI 120 Lab Assignment

--- type:NormalExercise lang:python xp:100 skills:1 key:b66b5626af
## Fix the Error

Notice the string entered in script on right.  Try running in the iPython shell by highlighting and pressing Ctrl-Enter:

Think about the type of error message you received.

*** =instructions
- Fix the error
- Press Submit Answer

*** =hint
- With syntax errors, look for mismatched "", '', or ()
- With runtime errors, look for mis-spelled words as Python needs exact match

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Correct the syntax error below
prnt("Here we go again!!!"

```

*** =solution
```{python}
# Correct the syntax error below
print("Here we go again!!!")
```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_output_contains("Here we go again!!!", pattern=False, no_output_msg = "Take a look at the instructions and try again")

success_msg("Nice job; another string that needed a missing ) and a mis-spelled print.")

```

--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:7ce347b7bc
## Try Something New

Take a look at the code below.  Try running it in the iPython shell.

*print(4/0)*

What type of error occurs?  Can you explain what caused this error?


*** =instructions
- Syntax error, did not follow Python rules
- Runtime error, followed the rules but something else was wrong when I ran it
- Semantic error, everything worked but not what I was expecting

*** =hint
- With runtime errors, look for bad direction to computer.  See if the instruction you gave is even possible.

*** =pre_exercise_code
```{python}
```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct."
msg_success = "Exactly! This runtime error was caused by telling the computer to divide by zero; something we know is not possible.  In programs, divide by zero can be more subtle than this.  Now you know what the error looks like, and what to look for when it does occur."
test_mc(2, [msg_bad, msg_success, msg_bad])

```

--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:aa3120c0eb
## Try Something New Take 2

Take a look at the code below.  Try running it in the iPython shell.

*print(1,000,000)*

What type of error occurs?  Can you explain what caused this error?


*** =instructions
- Syntax error, did not follow Python rules
- Runtime error, followed the rules but something else was wrong when I ran it
- Semantic error, everything worked but not what I was expecting

*** =hint
- No error message?  So is the code doing what you expected?

*** =pre_exercise_code
```{python}
```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct."
msg_success = "Correct!!  No error messages occurred because we followed the rules, and no impossible direction was given.  Unfortunately, we were not expecting 3 numbers.  We inadvertantly created a *tuple* in Python.  Even without () around the 3 numbers, separating by commas tells Python this is a *tuple*."
test_mc(3, [msg_bad, msg_bad, msg_success])

```

--- type:NormalExercise lang:python xp:100 skills:1 key:791cd66fd0
## Try Something New Take 3

Take a look at the code entered in the script to the right.  Try running it in the iPython shell.

What type of error occurs?  See if you can correct the error in the script.

*** =instructions
- Fix the error in the script
- Press Submit Answer

*** =hint
- With syntax errors, look for matching or missing "" or '' or ()

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Correct the syntax error below
'This is a string"
```

*** =solution
```{python}
# Correct the syntax error below
print("This is a string")
```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_output_contains("This is a string", pattern=False, no_output_msg = "Take a look at the instructions and try again")

test_function("print", index=1,
            not_called_msg = "Did you call print?",
            incorrect_msg = "Make sure a valid string is passed to print function.  Look at hint to help you identify.")

success_msg("Good job! It is important that the quotes at both end of string are the same type of quote.")

```

--- type:NormalExercise lang:python xp:100 skills:1 key:01f417f01e
## Will This Work?

You have been asked to calculate the sum of a long list of numbers: 1, 3, 4, 5, 7, 10, 13, 14, 22, 28, 34

The code in iPython shell was entered to address the requirements.  Try to run the code.

*** =instructions
- Check what was entered, and the result
- Is this result expected?  If not, fix the calculation
- Press Submit Answer
 

*** =hint
- Look at the original instructions
- Check the values indicated and carefully validate against what was entered.


*** =pre_exercise_code
```{python}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer
import pandas as pd
movies = pd.read_csv("http://s3.amazonaws.com/assets.datacamp.com/course/introduction_to_r/movies.csv")

import numpy as np

```

*** =sample_code
```{python}
# Correct the syntax error below
a = 1 + 3 + 4 + 5 + 7 + 10 + 14 + 22 + 28 + 34

# Print value in a
print(a)
```

*** =solution
```{python}
# Correct the syntax error below
a = 1 + 3 + 4 + 5 + 7 + 10 + 13 + 14 + 22 + 28 + 34

# Print value in a
print(a)
```


*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_object("a",
            undefined_msg = "Don't remove the definition of variable *a*.",
            incorrect_msg = "Check your calculation again.")

test_function("print", index=1,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the variable in print function.")

success_msg("Good job! This was a semantic error because we missed entering 13.")

```

--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:69e50c50af
## What Is the Data Type?

What is the data type of the following?

*3.2*


*** =instructions
- int
- float
- str
- Has no type

*** =hint
- Look at the symbols used, and look for indicators of string, integer, or floating point.

*** =pre_exercise_code
```{python}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

```


*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct."
msg_success = "Correct!  This is floating point because there are no quotes, and a decimal point is used with the numbers."
test_mc(2, [msg_bad, msg_success, msg_bad, msg_bad])
```

--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:274db49651
## What Is the Data Type? (2)

What is the data type of the following?

*"3.2"*


*** =instructions
- int
- float
- str
- Has no type

*** =hint
- Look at the symbols used, and look for indicators of string, integer, or floating point.

*** =pre_exercise_code
```{python}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

```


*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct."
msg_success = "Correct!  This is string because of the quotes.  The decimal point and digits do not mean number when quotes are present."
test_mc(3, [msg_bad, msg_bad, msg_success, msg_bad])
```

--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:3f8106f655
## What Is the Data Type? (3)

What is the data type of the following?

*32*


*** =instructions
- int
- float
- str
- Has no type

*** =hint
- Look at the symbols used, and look for indicators of string, integer, or floating point.

*** =pre_exercise_code
```{python}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

```


*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct."
msg_success = "Correct!  This is integer because there are no quotes and no decimal point; only numbers."
test_mc(1, [msg_success, msg_bad, msg_bad, msg_bad])
```


--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:c67f653aa7
## What Is the Data Type? (4)

What is the data type of the following?

*3 \* 2*


*** =instructions
- int
- float
- str
- Has no type

*** =hint
- Look at the symbols used, and look for indicators of string, integer, or floating point.

*** =pre_exercise_code
```{python}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

```


*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct."
msg_success = "Correct!  This is integer because there are no quotes and no decimal point, only numbers."
test_mc(1, [msg_success, msg_bad, msg_bad, msg_bad])
```


--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:46fe918faf
## What Is the Data Type? (5)

What is the data type of the following?

*3 \* .2*


*** =instructions
- int
- float
- str
- Has no type

*** =hint
- Look at the symbols used, and look for indicators of string, integer, or floating point.

*** =pre_exercise_code
```{python}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

```


*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct."
msg_success = "Correct!  This is floating point because there are no quotes, but there is a decimal point.  We have done multiplication with integer and float, and a floating point is created."
test_mc(2, [msg_bad, msg_success, msg_bad, msg_bad])
```

--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:81628bfe04
## What Is the Data Type? (6)

What is the data type of the following?

"3" * 2


*** =instructions
- int
- float
- str
- Has no type

*** =hint
- Look at the symbols used, and look for indicators of string, integer, or floating point.

*** =pre_exercise_code
```{python}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

```


*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct."
msg_success = "Correct!  This is string because of the quotes.  This actually replicates (multiplies) the string 3 twice."
test_mc(3, [msg_bad, msg_bad, msg_success, msg_bad])
```

--- type:NormalExercise lang:python xp:100 skills:1 key:22c8690582
## PEMDAS

Take a look at the code entered in the script to the right.  Try running it in the iPython shell.

Using (), show the groupings as they would be applied for PEMDAS.  Run the result in the shell to validate accuracy.


*** =instructions
- Add () to show each grouping done by PEMDAS order of precedence

*** =hint
- What does each part of PEMDAS represent?
- Why is the order of the letters important?

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Add () around PEMDAS groupings
a = 2 + 3 * 5 + 9

# Print value of a
print(a)
```

*** =solution
```{python}
# Correct the syntax error below
a = ((2 + (3 * 5)) + 9)

# Print value of a
print(a)
```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_student_typed("a\s*=\s*\(\(2\s*\+\s*\(3\s*\*\s*5\)\)\s*\+\s*9\)",not_typed_msg="Check your PEMDAS (); make sure you have covered all operations in correct order.")

test_object("a",
            undefined_msg = "Don't remove the definition of variable *a*.",
            incorrect_msg = "Check your PEMDAS () again.")

success_msg("Good job! For this one, we complete the multiplication, then the first addition, then the second addition.")

```


--- type:NormalExercise lang:python xp:100 skills:1 key:9f70d8f6e1
## PEMDAS (2)

Take a look at the code entered in the script to the right.  Try running it in the iPython shell.

Using (), show the groupings as they would be applied for PEMDAS.  Run the result in the shell to validate accuracy.


*** =instructions
- Add () to show each grouping done by PEMDAS order of precedence

*** =hint
- What does each part of PEMDAS represent?
- Why is the order of the letters important?

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Add () for PEMDAS grouping
a = 2 + 3 * (5 + 9)

# Print value of a
print(a)
```

*** =solution
```{python}
# Correct the syntax error below
a = (2 + (3 * (5 + 9)))

# Print value of a
print(a)
```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_student_typed("a\s*=\s*\(2\s*\+\s*\(3\s*\*\s*\(5\s*\+\s*9\)\)",not_typed_msg="Check your PEMDAS (); make sure you have covered all operations in correct order.")

test_object("a",
            undefined_msg = "Don't remove the definition of variable *a*.",
            incorrect_msg = "Check your PEMDAS () again.")

success_msg("Good job! For this one, we complete the operation in parentheses, then multiplication, then the addition.")

```


--- type:NormalExercise lang:python xp:100 skills:1 key:2b0f436126
## PEMDAS (3)

Take a look at the code entered in the script to the right.  Try running it in the iPython shell.

Using (), show the groupings as they would be applied for PEMDAS.  Run the result in the shell to validate accuracy.


*** =instructions
- Add () to show each grouping done by PEMDAS order of precedence

*** =hint
- What does each part of PEMDAS represent?
- Why is the order of the letters important?

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Add () for PEMDAS grouping
a = 2 // 3 + 5 % 9

# Print value of a
print(a)
```

*** =solution
```{python}
# Correct the syntax error below
a = ((2 // 3) + (5 % 9))

# Print value of a
print(a)
```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_student_typed("a\s*=\s*\(\(2\s*//\s*3\)\s*\+\s*\(5\s*\%\s*9\)\)",not_typed_msg="Check your PEMDAS (); make sure you have covered all operations in correct order.")

test_object("a",
            undefined_msg = "Don't remove the definition of variable *a*.",
            incorrect_msg = "Check your PEMDAS () again.")

success_msg("Good job! For this one, we complete the integer division, then the modulus calculation, then the addition.")

```


--- type:NormalExercise lang:python xp:100 skills:1 key:2506eea444
## Fix the Error (2)

Notice the string entered in script on right.  Try running in the iPython shell by highlighting and pressing Ctrl-Enter:

Think about the type of error message you received.

*** =instructions
- Run the command and look at error output
- Try switching the order of variable name and value

*** =hint
- Check the order of variable and expression in your assignment statement


*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Correct the syntax error below
87 = x

# Print value of x
print(x)

```

*** =solution
```{python}
# Correct the syntax error below
x = 87

# Print value of x
print(x)

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_student_typed("x\s*=\s*87",not_typed_msg="Check your variable assignment statement.")

test_object("x",
            undefined_msg = "You need an assignment statement for variable *x*.",
            incorrect_msg = "Did you correct assignment for variable *x*?")

test_function("print", index=1,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Be sure to print variable *x*.  Look at hint to help you identify.")

success_msg("Nice job; Assignment statements must put variable on the left and expression on the right.")

```


--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:4d375bba62
## Operation Shortcuts

Take a look at the code below.  Try running it in the iPython shell.

*a = b = 5*


*c = b + 2*


*b += 2*

What are the values of *a*, *b*, and *c* once run?


*** =instructions
- *a* is 5, *b* is 5, *c* is 7
- *a* is 5, *b* is 7, *c* is 7
- *a* is 5, *b* is 5, *c* is 5
- *a* is 5, *b* is 5, *c* is 5

*** =hint
- Try using print() for each variable to see current value

*** =pre_exercise_code
```{python}
```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct."
msg_success = "Correct!!  The first assignment statement sets up both *a* and *b*, the second creates *c* with current value of *b* + 2, and the third adds 2 to *b* with short hand version of *b = b + 2*.  Similar shorthand can be used for other arithmetic operations."
test_mc(2, [msg_bad, msg_success, msg_bad, msg_bad])

```

--- type:NormalExercise lang:python xp:100 skills:1 key:d33633f503
## Fix the Error (3)

Notice the string entered in script on right.  Try running in the iPython shell by highlighting and pressing Ctrl-Enter:

Think about the type of error message you received.

*** =instructions
- Fix the error
- Press Submit Answer

*** =hint
- When completing string concatenation, make sure all individual pieces are string type.

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Correct the syntax error below
print("This is an example " + "of string concatenation for " + 4 + " strings")

```

*** =solution
```{python}
# Correct the syntax error below
print("This is an example " + "of string concatenation for " + str(4) + " strings")
```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_output_contains("This is an example of string concatenation for 4 strings", pattern=False, no_output_msg = "Take a look at the instructions and try again")

test_function("print", index=1,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string that you created, and ensure it matches directions.  Look at hint to help you identify.")


success_msg("Nice job; we needed to convert data type for 4 from integer to string in order to use concatenation.")

```

--- type:NormalExercise lang:python xp:100 skills:1 key:2226242978
## Fix the Error (4)

Notice the string entered in script on right.  You are asked to write a program to sum the numbers from 10 to 20, take the average of those numbers, multiply the average by 3.2, add to 1000, and print the integer remainder when divided by 100.  The script on the right was created, but provides the wrong result.  

Think about the requirements and the result.  Fix the error(s).

*** =instructions
- Fix the problem with the script.
- Press Submit Answer

*** =hint
- Check the instructions, consider what the individual steps are that are needed.  
- Check each step one at a time for accuracy related to the calculation.

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Correct the error below
totl = 10 + 12 + 13 + 13 + 14 + 15 + 16 + 18 + 19 + 20
avg = totl/10
n = avg * 3.2 + 10
n = n//100
print(n)
```

*** =solution
```{python}
# Correct the syntax error below
totl = 10 + 11 + 12 + 13 + 14 + 15 + 16 + 17 + 18 + 19 + 20
avg = totl/11
n = avg * 3.2 + 1000
n = n%100
print(n)
```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_object("totl",
            undefined_msg = "Don't remove the definition of variable *totl*.",
            incorrect_msg = "Check your calculation for *totl* again.")
            
test_object("avg",
            undefined_msg = "Don't remove the definition of variable *avg*.",
            incorrect_msg = "Check your calculation for *avg* again.")

test_object("n",
            undefined_msg = "Don't remove the definition of variable *n*.",
            incorrect_msg = "Check your calculation for *n* again.")

test_function("print", index=1,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check your previous calculations to correct value for *n*.  Look at hint to help you identify.")
            
success_msg("Good job! This one involved several semantic errors.  You needed to fix each in order to achieve the right result.")

```
