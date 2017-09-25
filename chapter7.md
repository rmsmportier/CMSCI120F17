---
title       : Homework 6
description : CMSCI 120 Homework


--- type:NormalExercise lang:python xp:100 skills:1 key:fd2d31317f
## Let's Practice Conditionals

Conditionals provide our fifth building block; leaving only iterations to cover.  Conditionals enable us to vary logic applied to expressions by evaluating "conditions" that determine whether the logic should apply.

With conditionals comes a new data type in Python, *Boolean*.  *Boolean* variables can take only 2 possible values, *True* or *False*.  

The simplest form of conditional is the *if* statement.  *if* is a block statement similar to function definitions.  This means we will use ":" to indicate *more to come*, and indent logic to execute under the *if*.  The Python statements within the *if* statement will only be executed when the stated condition is *True*.  

Variables *scale* and *degrees* have been created in your Python shell.  Our goal is to convert temperatures from Celsius to Fahrenheit, or Fahrenheit to Celsius based on the value currently stored in *scale* which indicates the units associated with value currently in *degrees*.

In order to do this, our "condition" will use *==* to evaluate equality between the value in *scale* and a literal string.

Let's start with conversion from Celsius to Fahrenheit.


*** =instructions
- Modify the Python commands to evaluate *scale* for equality with the literal string *"Celsius"*.
- Conversion from Celsius to Fahrenheit is accomplished with 9/5 * degree + 32.  Modify the calculation inside the *if* block to convert the value in variable *degrees*.
- Assign the result to *odegrees* variable

*** =hint
- Are you using *==* for condition statement?
- Are you comparing the variable *scale* to *"Celsius"*?
- Check your calculation for conversion, and remember PEMDAS

*** =pre_exercise_code
```{python}

scale = "Celsius"
degrees = 100

```

*** =sample_code
```{python}
# Modify if statement to evaluate value in scale

if ____ ____ ____ :
    ____ = ____ * ____ / ____ + ____

```

*** =solution
```{python}
# Modify if statement to evaluate value in scale

if scale == "Celsius" :
    odegrees = degrees * 5 / 9 + 32

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_object("odegrees",
            undefined_msg = "Did you create variable *odegrees*?",
            incorrect_msg = "Check the syntax used to assign value to *odegrees*, and the calculation expression values.")

success_msg("Good work.  Let's try a few more examples.")

```

--- type:NormalExercise lang:python xp:100 skills:1 key:f04153389a
## Let's Practice *else*

When we combine *else* with *if*, we create a condition block that is only executed when the *if* condition is *False*.

We need to use the : to indicate *more to come*, and we need to indent statements within the *else* block statement. 

With *if* and *else* together, only 1 block will be executed.  *if* when the stated condition is *True*, and *else* when it is *False*.

We are going to add the conversion logic needed to convert from Fahrenheit to Celsius.

*** =instructions
- Modify the Python commands to evaluate *scale* for equality with the literal string *"Celsius"*.
- Conversion from Celsius to Fahrenheit is accomplished with 9/5 * degree + 32.  Modify the calculation inside the *if* block to convert the value in variable *degrees*.
- Inside the *else* block, use the formula to convert from Fahrenheit to Celsius.  This formula requires that we subtract 32 from *degrees*, and then multiply by 5/9.  For this calculation, be sure to include () around the subtraction so that calculation is completed first.
- Assign the result to *odegrees* variable.

*** =hint
- Are you using *==* for condition statement with *if*?
- Are you comparing the variable *scale* to *"Celsius"*?
- Check your calculation for conversion in *if* block (Celsius to Fahrenheit), and remember PEMDAS.
- Check your calculation for conversion in *else* block (Fahrenheit to Celsius), and remember PEMDAS.

*** =pre_exercise_code
```{python}

scale = "Celsius"
degrees = 100

```

*** =sample_code
```{python}
# Modify if statement to evaluate value in scale

if ____ ____ ____ :
    ____ = ____ * ____ / ____ + ____
else:
    ____ = __ ____ - ____ __ * ____ / ____

```

*** =solution
```{python}
# Modify if statement to evaluate value in scale

if scale == "Celsius" :
    odegrees = degrees * 9 / 5 + 32
else:
    odegrees = (degrees - 32) * 5/9

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_object("odegrees",
            undefined_msg = "Did you create variable *odegrees*?",
            incorrect_msg = "Check the syntax used to assign value to *odegrees*, and the calculation expression values.")

success_msg("Excellent.  Let's keep going.")

```

--- type:NormalExercise lang:python xp:100 skills:1 key:459fc97d29
## Add *elif* to complete structure

Suppose the condition we state with *if* has multiple possibilities.  For example, suppose we have a variable that can contain the values 2, 3, 4, or 5.

When the value is 2, we want to take one action.  When the value is 3, another;     4, another;   etc.

*elif* provides a way to do this.  When the condition specified for *if* is *False*, we can then evaluate a different condition.  *elif* stands for *else if*.  Python evaluates *elif* condition when *if* is *False*.

Combining *if*, *elif*, and *else* creates a chain in which only block statements for one condition will be executed.  The chain contains one *if* at the start, at most one *else* at the end, and any number of *elif* in between.

*elif* will only be evaluated when a previous condition is *False* whether *if* or *elif*.  Once a *True* condition is encountered, nothing further is evaluated.  *else* is the catch all at the bottom in the event that no *True* condition was found anywhere in the chain.

*We are going to play a small Magic 8 ball game.  Based on the value in variable "num", the Magic 8 ball will provide a response of "Yes", "No", or "Maybe".  If the value of "num" is 0, Magic 8 ball responds "No".  If the value is 1, the response is "Yes".  If the value is any other value, the response will be "Maybe".*

*** =instructions
- Modify the Python commands to evaluate *num* for equality with 0.
- Modify the block statement for *if* to set variable *magic* to "No".
- Introduce *elif* along with condition to evaluate *num* for equality with 1.
- Modify the block statement for *elif* to set variable *magic* to "Maybe".
- Introduce *else* statement to handle any other value for *num*.  You will not need to add a condition as this will only be executed if neither of the previous checks resulted in True.
- Modify the block statement for *else* to set variable *magic* to "Yes".

*** =hint
- Are you using *==* for comparing equality with *if* and *elif*?
- Make sure you are not attaching condition to *else*; it will only execute when previous are not *True*.
- Are you comparing the variable *num* to the correct values for *if* and *elif*?
- Check your string assignments to variable *magic*.
- Print the value in *magic*.

*** =pre_exercise_code
```{python}

num = 2

```

*** =sample_code
```{python}
# Modify if statement to get response for your value

if ____ ____ ____ :
    ____ = ____
elif ____ ____ ____ :
    ____ = ____
else:
    ____ = ____
    
# Print value of magic
____(____)

```

*** =solution
```{python}
# Modify if statement to get response for your value

if num == 0 :
    magic = "No"
elif num == 1 :
    magic = "Yes"
else:
    magic = "Maybe"
    
print(magic)

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_object("magic",
            undefined_msg = "Did you create variable *magic*?",
            incorrect_msg = "Check the instructions and make sure you are assigning correct value to *magic* based on evaluated value of *num*.")

test_student_typed("if\s*num\s*={2}\s*0\s*:",not_typed_msg="Check syntax for equal to 0")

test_student_typed("elif\s*num\s*={2}\s*1\s*:",not_typed_msg="Check syntax for equal to 1")

test_student_typed("else:",not_typed_msg="Check syntax for condition if either of previous are not *True*")

success_msg("Good work.  You re getting the hang of this.")

```

--- type:NormalExercise lang:python xp:100 skills:1 key:c63077e73b
## Comparison Operators

In addition to equality, comparison operators exist for

- less than *<*
- greater than *>*
- less than or equal to *<=*
- greater than or equal to *>=*
- not equal to *!=*

For the instructions below, select the appropriate comparison operator to use. A variable *num* has been created that can be evaluated for each conditional statement.  Evaluate the value in the order indicated in instructions.  Only one result should be *True*.

*** =instructions
- If the value for *num* is less than 0, assign "Invalid number" to *msg*
- If the value for *num* is less than 10, assign "Not this time" to *msg*
- If the value for *num* is less than 20, assign "We are getting there" to *msg*
- If the value for *num* is less than 40, assign "Almost there" to *msg*
- If the value for *num* is less than 60, assign "Got it!" to *msg*
- If the value for *num* is greater than or equal to 60, assign "Invalid number" to *msg*

*** =hint
- For each condition, consider the available comparison operators, and select the appropriate one
- Remember, in a chain, there is only one *if* and at most one *else*.  Use *else* to handle the fallout from all previous conditions.
- Make sure you created *msg* with appropriate string values
- Print the value in *msg*

*** =pre_exercise_code
```{python}

num = 27

```

*** =sample_code
```{python}

# Is the value for *num* less than 0?

____ num ____ 0:
    ____ = "____"

# Is the value for *num* less than 10?

____ num ____ 10:
    ____ = "____"
    
# Is the value for *num* less than 20?

____ num ____ 20:
    ____ = "____"
    
# Is the value for *num* less than 40?

____ num ____ 40:
    ____ = "____"

# Is the value for *num* less than 60?

____ num ____ 60:
    ____ = "____"
    
# Is the value for *num* greater than or equal to 60?

____:
    ____ = "____"
    
# Print msg
print(____)

```

*** =solution
```{python}
# Is the value for *num* less than 0?

if num < 0:
    msg = "Invalid number"

# Is the value for *num* less than 10?

elif num < 10:
    msg = "Not this time"
    
# Is the value for *num* less than 20?

elif num < 20:
    msg = "We are getting there"
    
# Is the value for *num* less than 40?

elif num < 40:
    msg = "Almost there"

# Is the value for *num* less than 60?

elif num < 60:
    msg = "Got it!"
    
# Is the value for *num* greater than or equal to 60?

else:
    msg = "Invalid number"

print(msg)

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_object("msg",
            undefined_msg = "Did you create *msg* for each possible condition?",
            incorrect_msg = "Check the condition statements against the original instuctions.  Incorrect value for *msg*.  Only one conditional should be executed.")

test_student_typed("if\s*num\s*\\<\s*0:\s*",not_typed_msg="Check syntax for less than 0")

test_student_typed("elif\s*num\s*\\<\s*10:\s*",not_typed_msg="Check syntax for less than 10")

test_student_typed("if\s*num\s*\\<\s*20:\s*",not_typed_msg="Check syntax for less than 20")

test_student_typed("if\s*num\s*\\<\s*40:\s*",not_typed_msg="Check syntax for less than 40")

test_student_typed("if\s*num\s*\\<\s*60:\s*",not_typed_msg="Check syntax for less than 60")

success_msg("Excellent.  One last piece for conditionals, and you will have this mastered.")

```

--- type:NormalExercise lang:python xp:100 skills:1 key:81339413ce
## Logical Operators

We can now connect several logical expressions together using *and*, *or*, and *not*

For the instructions below, select the appropriate logical operator to use. A variable *num1* has been created that can be evaluated for each conditional statement.  An additional variable *num2* has been created that can be evaluated along with *num1*, according to the instructions below.  Only one result should be *True*.

*** =instructions
- If the value for *num1* is less than or equal to 0, and value for *num2* is greater than 0, calculate *val* as product of *num1* and *num2*
- If the value for *num1* is greater than 0, and value for *num2* is less than or equal to 0, calculate *val* as sum of *num1* and *num2*
- If the value for *num1* is greater than 0, and value for *num2* is greater than 0, calculate *val* as *num1* divided by *num2*
- Otherwise, set *val* to "No operation provided".

*** =hint
- For each condition, consider the available logical operators, and select the appropriate one
- Remember, in a chain, there is only one *if* and at most one *else*.  Use *else* to handle the fallout from all previous conditions.
- Make sure you created *val* with appropriate arithmetic operations for variables *num1* and *num2*
- Print the value in *val*

*** =pre_exercise_code
```{python}

num1 = 27
num2 = -4

```

*** =sample_code
```{python}

# Is the value for num1 less than or equal to 0 and num2 greater than 0?

____ num1 ____ 0 ____ num2 ____ 0:
    ____ = ____ ____ ____

# Is the value for num1 greater than 0 and num2 less than or equal to 0?

____ num1 ____ 0 ____ num2 ____ 0:
    ____ = ____ ____ ____
    
# Is the value for num1 greater than 0 and num2 greater than 0?

____ num1 ____ 0 ____ num2 ____ 0:
    ____ = ____ ____ ____
    
# What do we do if none of the above are True?

____:
    ____ = ____


# Print val
print(____)

```

*** =solution
```{python}
# Is the value for num1 less than or equal to 0 and num2 greater than 0?

if num1 <= 0 and num2 > 0:
    val = num1 * num2

# Is the value for num1 greater than 0 and num2 less than or equal to 0?

elif num1 > 0 and num2 <= 0:
    val = num1 + num2
    
# Is the value for num1 greater than 0 and num2 greater than 0?

elif num1 > 0 and num2 > 0:
    val = num1 / num2
    
# What do we do if none of the above are True?

else:
    val = "No operation provided"


# Print val
print(val)

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_object("val",
            undefined_msg = "Did you create *val* for each possible condition?",
            incorrect_msg = "Check the condition statements against the original instuctions.  Incorrect value for *val*.  Only one conditional should be executed.")

test_student_typed("if\s*num1\s*\\<=\s*0\s*and\s*num2\s*\\>\s*0:\s*",not_typed_msg="Check syntax for num1 less than or equal to 0 and num2 greater than 0")

test_student_typed("elif\s*num1\s*\\>\s*0\s*and\s*num2\s*\\<=\s*0:\s*",not_typed_msg="Check syntax for num1 greater than 0 and num2 less than or equal to 0")

test_student_typed("elif\s*num1\s*\\>\s*0\s*and\s*num2\s*\\>\s*0:\s*",not_typed_msg="Check syntax for num1 greater than 0 and num2 greater than 0")

test_student_typed("else:",not_typed_msg="Check syntax for what to do if none are True")



success_msg("Excellent work!!!  One building block left, and you can program anything.")

```

