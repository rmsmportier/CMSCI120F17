---
title       : Lab 2
description : CMSCI 120 Lab Assignment

--- type:NormalExercise lang:python xp:100 skills:1 key:b66b5626af
## Fix the Error

Notice the string entered in script on right.  Try running in the shell below by highlighting and pressing Ctrl-Enter:

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

Take a look at the code entered in the script to the right.  Try running it in the shell below.

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
print(a)
```

*** =solution
```{python}
# Correct the syntax error below
a = 1 + 3 + 4 + 5 + 7 + 10 + 13 + 14 + 22 + 28 + 34
print(a)
```


*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_object("a",
            undefined_msg = "Don't remove the definition of variable *a*.",
            incorrect_msg = "Check your calculation again.")

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
