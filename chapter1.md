---
title       : Lab 1
description : CMSCI 120 Lab Assignment

--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:7ce347b7bc
## Let's Say Hello to Python

In the iPython shell, type the following exactly:

*Hello Python!!!  How’s it going?”*

What type of error message did you receive?

*** =instructions
- Syntax error, did not follow Python rules
- Runtime error, followed the rules but something else was wrong when I ran it
- Semantic error, everything worked but not what I was expecting

*** =hint


*** =pre_exercise_code
```{python}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

```


*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct."
msg_success = "Exactly! Something about our instruction was not correct."
test_mc(1, [msg_success, msg_bad, msg_bad])
```

--- type:NormalExercise lang:python xp:100 skills:1 key:b66b5626af
## Fix the Error

We have demonstrated our code was incorrect.  Let's fix the mistake and submit again.

*** =instructions
- Fix the string delimiter in the script
- Add *print* in front of the phrase
- Surround the phrase with ()
- Press Submit Answer

*** =hint
- With syntax errors, look for matching or missing "" or '' or ()
- Make sure you are telling Python you want to print result of expression

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Correct the syntax error below
Hello Python!!!  How’s it going?"

```

*** =solution
```{python}
# Correct the syntax error below
print("Hello Python!!!  How’s it going?")
```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

Ex().test_output_contains("Hello Python!!!  How\’s it going?", pattern=True, no_output_msg = "Take a look at the instructions and try again")

success_msg("Nice job!  When asking Python to print a string, we need to be sure to include appropriate string delimiters and use print with ()")

```

--- type:NormalExercise lang:python xp:100 skills:1 key:a5404db31b
## Let's Try Another

Notice the string entered in script on right.  Try running in the shell below by highlighting and pressing Ctrl-Enter:

Think about the type of error message you received.

*** =instructions
- Fix the string delimiter in the script
- Add *print* in front of the phrase
- Surround the phrase with ()
- Press Submit Answer

*** =hint
- We want this to be a string
- What delimiters are needed for a string?
- Make sure you are telling Python you want to print result of expression

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Correct the syntax error below
Not too bad

```

*** =solution
```{python}
# Correct the syntax error below
print("Not too bad")
```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

Ex().test_output_contains("Not too bad", pattern=False, no_output_msg = "Take a look at the instructions and try again")

success_msg("You are getting the hang of this!  Another string that needed delimiters and print with ().  *Not* is a token Python recognizes, so it was expecting instructions that matched with *Not*.  This is why the cursor was placed under *too*.")

```

--- type:NormalExercise lang:python xp:100 skills:1 key:b8846bb749
## You Are on a Roll

Take a look at the code entered in the script to the right.  Try running it in the shell below.

What type of error occurs?  See if you can correct the error in the script.

*** =instructions
- Fix the runtime error in the script
- Press Submit Answer

*** =hint
- With runtime errors, look for mis-spelled words as Python needs exact match

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Correct the syntax error below
prnt("Now what?")

```

*** =solution
```{python}
# Correct the syntax error below
print("Now what?")
```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

Ex().test_output_contains("Now what?", pattern=False, no_output_msg = "Take a look at the instructions and try again")

success_msg("Nice!  NameError means Python attempted to look up a phrase we provided and was unable to find a match.  When we are giving instructions, this often means our instruction 'token' does not match one Python knows.  This is a runtime error because Python does not match tokens until attempting to run after no syntax errors exist.")

```

--- type:NormalExercise lang:python xp:100 skills:1 key:791cd66fd0
## Keep It Going

Take a look at the code entered in the script to the right.  Try running it in the shell below.

What type of error occurs?  See if you can correct the error in the script.

*** =instructions
- Fix the syntax error in the script
- Press Submit Answer

*** =hint
- With syntax errors, look for matching or missing "" or '' or ()

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Correct the syntax error below
print("Will it work this time?"
```

*** =solution
```{python}
# Correct the syntax error below
print("Will it work this time?")
```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

Ex().test_output_contains("Will it work this time?", pattern=False, no_output_msg = "Take a look at the instructions and try again")

success_msg("Good job!  EOF errors indicate Python went all the way to end of script (End of File) but could not find what it was looking for.  Often this proves to be a missing ) or mismatched pair ().  A similar EOL error indicates Python went to end of line but could not find what it was looking for.  Often this proves to be a missing or mismatched pair of quotes.")

```

--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:2cb40637cf
## Will This Work?

See if you can anticpate what will happen with the following.  

Think about it before you try it in the shell, and see if you can answer without running.

Will we get an error?

*print("Is there any chance we got this right?")*


*** =instructions
- This will cause a syntax error
- This will cause a runtime error
- This will run without error

*** =hint


*** =pre_exercise_code
```{python}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

```


*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct."
msg_success = "Excellent!!  I think you have mastered errors."
test_mc(3, [msg_bad, msg_bad, msg_success])
```

--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:f824a20e87
## Python as a Calculator

Enter the following in the iPython shell on right

*2 + 3*

What is the result of this command;?  What type of arithmetic operation was completed?  Or did we get an error?

*** =instructions
- Multiplication
- Division
- Exponentiation
- Addition
- An error occurred

*** =hint
- Think about what that symbol means in arithmetic

*** =pre_exercise_code
```{python}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

```


*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct."
msg_success = "Correct!"
test_mc(4, [msg_bad, msg_bad, msg_bad, msg_success, msg_bad])
```

--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:460e5b34b3
## More Calculations

Enter the following in the iPython shell on right

*2 \* 3*

What is the result of this command?  What type of arithmetic operation was completed?  Or did we get an error?

*** =instructions
- Multiplication
- Division
- Exponentiation
- Addition
- An error occurred

*** =hint
- Think about what arithmetic symbols look similar to \*

*** =pre_exercise_code
```{python}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

```


*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct."
msg_success = "Correct!"
test_mc(1, [msg_success, msg_bad, msg_bad, msg_bad, msg_bad])
```

--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:f8be13cace
## Symbols Context Is Everything

Enter the following in the iPython shell on right

*+2*

What is the result of this command?  What type of arithmetic operation was completed?  Or did we get an error?

*** =instructions
- Multiplication
- Subtraction
- Positive number
- Division
- An error occurred

*** =hint
- Look to the left of the + sign; nothing there.  What are we changing then?

*** =pre_exercise_code
```{python}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

```


*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct."
msg_success = "Correct!"
test_mc(3, [msg_bad, msg_bad, msg_success, msg_bad, msg_bad])
```

--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:5117039165
## Extended Context

Enter the following in the iPython shell on right

*++++2*

What is the result of this command?  What type of arithmetic operation was completed?  Or did we get an error?

*** =instructions
- Multiplication
- Subtraction
- Division
- Positive number
- An error occurred

*** =hint
- Look to the left of the + sign; nothing there.  What are we changing then?

*** =pre_exercise_code
```{python}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

```


*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct."
msg_success = "Correct!  The number of + does not matter; still a positive number."
test_mc(4, [msg_bad, msg_bad, msg_bad, msg_success, msg_bad])
```

--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:b15f34058b
## Changing the Context

Enter the following in the iPython shell on right

*-2*

What is the result of this command?  What type of arithmetic operation was completed?  Or did we get an error?

*** =instructions
- Multiplication
- Negative number
- Division
- Positive number
- An error occurred

*** =hint
- Look to the left of the - sign; nothing there.  What are we changing then?

*** =pre_exercise_code
```{python}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

```


*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct."
msg_success = "Correct!  The \- takes value to right and makes it negative."
test_mc(2, [msg_bad, msg_success, msg_bad, msg_bad, msg_bad])
```

--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:866da4d600
## Changing the Context (2)

Enter the following in the iPython shell on right

*- - - - - 2*

What is the result of this operation?  Can you explain why this happened?

*** =instructions
- 2
- \-2
- An error occurred

*** =hint
- Count the number of \- signs

*** =pre_exercise_code
```{python}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

```


*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct."
msg_success = "Correct!  The parity of \- matters as it influences whether positive or negative number."
test_mc(2, [msg_bad, msg_success, msg_bad])
```

--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:2d607defbb
## Symbols Context Is Everything (2)

Enter the following in the iPython shell on right

*\- - - - 2*

What is the result of this operation?  Can you explain why this happened?

*** =instructions
- 2
- \-2
- An error occurred

*** =hint
- Count the number of \- signs

*** =pre_exercise_code
```{python}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

```


*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct."
msg_success = "Correct!  The parity of \- matters as it influences whether positive or negative number."
test_mc(1, [msg_success, msg_bad, msg_bad])
```

--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:68b4b0fe9a
## Symbols Context Is Everything (3)

Enter the following in the iPython shell on right

*2 + + + 2*

What is the result of this operation?  Can you explain why this happened?

*** =instructions
- 4
- 8
- An error occurred

*** =hint
- What does + mean?

*** =pre_exercise_code
```{python}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

```


*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct."
msg_success = "Correct!  We added 2 positive numbers."
test_mc(1, [msg_success, msg_bad, msg_bad])
```

--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:5c1f4dfa5a
## Symbols Context Is Everything (4)

Enter the following in the iPython shell on right

*2 - - - 2*

What is the result of this operation?  Can you explain why this happened?

*** =instructions
- -4
- 4
- 0
- An error occurred

*** =hint
- Count the number of \- signs

*** =pre_exercise_code
```{python}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

```


*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct."
msg_success = "Correct!  2 - 2 is 0"
test_mc(3, [msg_bad, msg_bad, msg_success, msg_bad])
```

--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:2bffbe42a1
## Symbols Context Is Everything (5)

Enter the following in the iPython shell on right

*04*

What is the result of this operation?  Can you explain why this happened?

*** =instructions
- -4
- 4
- 0
- An error occurred

*** =hint
- Is there a number 04?

*** =pre_exercise_code
```{python}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

```


*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct."
msg_success = "Correct!  04 is not a number, and Python would need the 0 removed."
test_mc(4, [msg_bad, msg_bad, msg_bad, msg_success])
```

--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:1f1e8f692a
## Symbols Context Is Everything (6)

Enter the following in the iPython shell on right

*3 4*

What is the result of this operation?  Can you explain why this happened?

*** =instructions
- 34
- result of 3+4 or 7
- 2 numbers were created
- An error occurred

*** =hint
- How many distinct numbers in what you typed?
- Do you think this is clear to Python?

*** =pre_exercise_code
```{python}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

```


*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct."
msg_success = "Correct!  Python cannot interpret that space, so a syntax error is created.  We would need to remove the space to create the number 34.  We could also surround (3,4) and create what Python knows as a *tuple*, or multiple numbers."
test_mc(4, [msg_bad, msg_bad, msg_bad, msg_success])
```