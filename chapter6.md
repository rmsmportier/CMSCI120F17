---
title       : Homework 5
description : CMSCI 120 Homework


--- type:NormalExercise lang:python xp:100 skills:1 key:fd2d31317f
## Creating a Function Framework

Functions provide a powerful element related to computer programming, as we can expand our base programming language to create our own functions.  These enable us to use our functions interchangeably with tokens and functions provided within the programming language.

This is highly useful when developing large systems, as multiple programmers can code functions to seamlessly integrate once completed.  Additionally, we can avoid repeating the same code over and over within the larger system.  This ensures when we need to change the program, we only change in one place versus many.

Additional benefits include reduced maintenance costs for the resulting application, faster development time, ability to swap capability easily for updated capability in the future, simplified testing, and the list goes on and on.

We are going to build a new program to achieve the following:
    *Prompt for a debt amount owed by a consumer, and for a US currency denomination from the following possibilities ($1, $5, $10, $20, $50, $100).  Calculate the height of bills required to pay that debt for that denomination knowing that the thickness of every U.S. denomination bill is 0.0043 inches.  Calculate the height in centimeters knowing there are 2.54 centimeters in 1 inch.  Print the result with appropriate text describing what was entered and what was calculated.*

*** =instructions
- Create the function framework needed to deliver our program.  
- Try creating CFD for this program before you begin in order to align each task with the functions we will create.
- Create a function definition called *InputDebt*; add print statement indicating *"Inside InputDebt"*.
- Create a function definition called *InputDen*; add print statement indicating *"Inside InputDen"*.
- Create a function definition called *CalcHeight*; add print statement indicating *"Inside CalcHeight"*.
- Create a function definition called *PrintHeight*; add print statement indicating *"Inside PrintHeight"*.

*** =hint
- Create functions that align with instructions.  Remember the important elements to create function.
- *define* the function.
- *name* the function.
- *indicate* it is a function.
- *indicate more* to come.

*** =pre_exercise_code
```{python}

```

*** =sample_code
```{python}
# Create function InputDebt; print output indicated in instructions
def ____ _ _ :
    print("____")
    
# Create function InputDen; print output indicated in instructions
def ____ () __
    print("____")
    
# Create function CalcHeight; print output indicated in instructions
def ____ _ _ :
    print("____")
    
# Create function PrintHeight; print output indicated in instructions
def ____ _ _ :
    print("____")

```

*** =solution
```{python}
# Create function InputDebt; print output indicated in instructions
def InputDebt () :
    print("Inside InputDebt")
    
# Create function InputDen; print output indicated in instructions
def InputDen () :
    print("Inside InputDen")
    
# Create function CalcHeight; print output indicated in instructions
def CalcHeight () :
    print("Inside CalcHeight")
    
# Create function PrintHeight; print output indicated in instructions
def PrintHeight () :
    print("Inside PrintHeight")

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_student_typed("def\s*InputDebt\s*\\(\s*\\)\s*:",not_typed_msg="Check your function definition for the function InputDebt")

test_student_typed("def\s*InputDen\s*\\(\s*\\)\s*:",not_typed_msg="Check your function definition for the function InputDen")

test_student_typed("def\s*CalcHeight\s*\\(\s*\\)\s*:",not_typed_msg="Check your function definition for the function CalcHeight")

test_student_typed("def\s*PrintHeight\s*\\(\s*\\)\s*:",not_typed_msg="Check your function definition for the function PrintHeight")

test_student_typed("Inside InputDebt",not_typed_msg="Check instructions for string to print in *InputDebt*")

test_student_typed("Inside InputDen",not_typed_msg="Check instructions for string to print in *InputDen*")

test_student_typed("Inside CalcHeight",not_typed_msg="Check instructions for string to print in *CalcHeight*")

test_student_typed("Inside PrintHeight",not_typed_msg="Check instructions for string to print in *PrintHeight*")

success_msg("Good work.  We have an initial function framework.")

```

--- type:NormalExercise lang:python xp:100 skills:1 key:5da1240b9e
## Build Out First Input Function

Let's make the first input function operational.  

Due to DataCamp restrictions, we won't be using *input()* in this function.  Instead, we will return value from a variable inside the function.  

The framework is the same as when we use *input()*; our approach will be different in order to align with DataCamp restrictions.


*** =instructions
- Assign the value "2376495" to variable *d* in *InputDebt*.  The result is the same as if we had prompted with *input()* function to enter a value, and user entered 2376495
- Convert the value in *d* to integer
- Return the value in *d* to the calling program
- Assign the returned value to variable *debt*

*** =hint
- We want value assigned to variable to be string with specified value.
- What function have we used that will convert data type to integer?  Once converted, remember to store the value back in the variable in main memory.
- What Python syntax returns value in a variable?
- Call *InputDebt*, and save returned value to variable *debt*.

*** =pre_exercise_code
```{python}

```

*** =sample_code
```{python}
# Complete details for InputDebt based on instructions
def InputDebt ():
    ____ = ____
    ____ = ____(____)
    ____ ____

____ = InputDebt()

```

*** =solution
```{python}
# Complete details for InputDebt based on instructions
def InputDebt ():
    d = "2376495"
    d = int(d)
    return d
    
debt = InputDebt()


```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_student_typed('d\s*=\s*"2376495"',not_typed_msg="Check your value assigned to *d* inside function.")

test_student_typed("d\s*=\s*int\\(d\\)",not_typed_msg="Check your type casting function for *d* inside function.")

test_function("InputDebt", 
            not_called_msg = "Check the function definition for *InputDebt*.",
            incorrect_msg = "Check requirements for details related to *InputDebt*, and ensure you returned value from the function.")
            
test_object("debt",
            undefined_msg = "Did you create variable *debt*?",
            incorrect_msg = "Check the syntax used to assign value to *debt*, and the value returned from *InputDebt*.")

success_msg("That's it.  Now our first input function is operational.")

```


--- type:NormalExercise lang:python xp:100 skills:1 key:6e1dae5ba8
## Build Out Second Input Function

Let's make the second input function operational.  

Due to DataCamp restrictions, we won't be using *input()* in this function.  Instead, we will return value from a variable inside the function.  

The framework is the same as when we use *input()*; our approach will be different in order to align with DataCamp restrictions.


*** =instructions
- Assign the value "5" to variable *d* in *InputDen*.  The result is the same as if we had prompted with *input()* function to enter a value, and user entered 5
- Convert the value in *d* to integer
- Return the value in *d* to the calling program
- Assign the result to variable *den*

*** =hint
- We want value assigned to variable to be string with specified value.
- What function have we used that will convert data type to integer?  Once converted, remember to store the value back in the variable in main memory.
- What Python syntax returns value in a variable?
- Call *InputDen*, and save returned value to variable *den*.

*** =pre_exercise_code
```{python}

```

*** =sample_code
```{python}
# Complete details for InputDen based on instructions
def InputDen ():
    ____ = ____
    ____ = ____(____)
    ____ ____

____ = InputDen()

```

*** =solution
```{python}
# Complete details for InputDen based on instructions
def InputDen ():
    d = "5"
    d = int(d)
    return d
    
den = InputDen()


```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_student_typed('d\s*=\s*"5"',not_typed_msg="Check your value assigned to *d*.")

test_student_typed("d\s*=\s*int\\(d\\)",not_typed_msg="Check your type casting function for *d*")

test_function("InputDen", 
            not_called_msg = "Check the function definition for *InputDen*.",
            incorrect_msg = "Check requirements for details related to *InputDen*, and ensure you returned value from the function.")
            
test_object("den",
            undefined_msg = "Did you create variable *den*?",
            incorrect_msg = "Check the syntax used to assign value to *den*, and the value returned from *InputDen*.")

success_msg("Keep it going; two input functions are now operational.")


```

--- type:NormalExercise lang:python xp:100 skills:1 key:1ef3035953
## Build Out Calculation Function

Let's make the calculation function operational.  

*** =instructions
- Variables *debt* and *den* previously created still exist in your workspace.
- Modify the function definition for *CalcHeight* to accept these 2 values.  Call the parameters in the function definition *dt* and *dn*.
- Calculate the number of bills needed to pay the debt using indicated denomination.  You cannot have partial bills, so use of floor (integer) division would be helpful.  Assign this value to variable *bills*.
- Convert the number of bills to a height in cm using .0043 inches/bill and 2.54 cm/inch.  Assign this value to variable *h*.
- Return the calculated height to the calling logic.
- Call *CalcHeight* passing the contents of variable *debt* and variable *den*.  Assign the result to variable *height*.

*** =hint
- If we are sending values to function, names to represent this need to be in function definition and in calling logic.
- Parameters are the names used inside function for values passed.
- Arguments are the names used when calling function.
- Floor division is one of these operators, // or %.
- You will use combination of either * or \ operator to convert units.  Think about current units, and how to cancel units to achieve desired result.

*** =pre_exercise_code
```{python}
debt = 2376495
den = 5
```

*** =sample_code
```{python}
# Complete details for CalcHeight based on instructions
def CalcHeight (____,____):
    ____ = dt ____ dn
    ____ = bills ____ .0043 ____ 2.54
    ____ ____

____ = CalcHeight(____, ____)

```

*** =solution
```{python}
# Complete details for CalcHeight based on instructions
def CalcHeight (dt, dn):
    bills = dt // dn
    h = bills * .0043 * 2.54
    return h
    
height = CalcHeight(debt,den)


```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_student_typed('dt,\s*dn',not_typed_msg="Check parameter names for function.")

test_student_typed("bills\s*=\s*dt\s*\/\/\s*dn",not_typed_msg="Check your calculation for *bills*.")

test_student_typed("h\s*=\s*bills\s*\\*\s*\\.0043\s*\\*\s*2\\.54",not_typed_msg="Check your calculation for *h*.")

test_function("CalcHeight", 
            not_called_msg = "Check the function definition for *CalcHeight*.",
            incorrect_msg = "Check requirements for details related to *CalcHeight*, and ensure you returned value from the function.")
            
test_object("height",
            undefined_msg = "Did you create variable *height*?",
            incorrect_msg = "Check the syntax used to assign value to *height*, and the value returned from *CalcHeight*.")

success_msg("Excellent!!!  That was probably the hardest of the functions to make operational.")


```

--- type:NormalExercise lang:python xp:100 skills:1 key:3715de0f86
## Build Out Print Function

Let's make the print function operational.  

*** =instructions
- Variable *height* and *den* previously created still exist in your workspace
- Modify the function definition for *PrintHeight* to accept these values.  Call the parameters in the function definition *ht* and *dn*.
- Complete *print()* inside *PrintHeight* to print desired output. Round the height printed to 2 decimal places
- Call *PrintHeight* passing the contents of variable *height* and variable *den*.  

*** =hint
- If we are sending values to function, names to represent this need to be in function definition and in calling logic
- Parameters are the names used inside function for values passed
- Arguments are the names used when calling function 

*** =pre_exercise_code
```{python}
debt = 2376495
den = 5

def CalcHeight (dt, dn):
    bills = dt // dn
    h = bills * .0043 * 2.54
    return h
    
height = CalcHeight(debt,den)

```

*** =sample_code
```{python}
# Complete details for PrintHeight based on instructions
def PrintHeight (____,____):
    print("Height of $",____," bills to pay debt is ",____(____,____), " centimeters", sep='')

PrintHeight(____,____)
```

*** =solution
```{python}
# Complete details for PrintHeight based on instructions
def PrintHeight (ht,dn):
    print("Height of $",dn," bills to pay debt is ",round(ht,2), " centimeters", sep='')

PrintHeight(height,den)

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_student_typed('"Height\s*of\s*\$",\s*dn,"\sbills to pay debt is ",round\\(ht,2\\)',not_typed_msg="Check values sent to print statement.  Be sure value for denomination prints first, and value for height second rounded to 2 decimal places.")

test_function("PrintHeight", 
            not_called_msg = "Check the function definition for *PrintHeight*.",
            incorrect_msg = "Check requirements for details related to *PrintHeight*, and ensure you passed correct values in correct order.")

success_msg("We are almost there.  We just need to pull it all together.")

```

--- type:NormalExercise lang:python xp:100 skills:1 key:b4ab7abe30
## Complete Program Framework

Let's make our program work end to end.  We need to create *main()* function that calls each of our previous functions, in the correct order.  Results should be assigned to variables in *main*, and appropriately passed to other functions as needed.

*** =instructions
- Function definitions already exist in your workspace.  You will not need to change these except for the value in *InputDebt*.
- Modify function *InputDebt* to set *d* in *InputDebt* to 279383283987.
- Create function definition for *main()* function.
- *main* needs to call *InputDebt*, saving the returned value to *debt*.
- *main* needs to call *InputDen*, saving the returned value to *den*.
- *main* needs to call *CalcHeight*, passing *debt* and *den* as arguments, and saving the returned value to *height*.
- *main* needs to call *PrintHeight*, passing *height* and *den* as arguments.
- Modify program to call *main*.

*** =hint
- If we are sending values to function, names to represent this need to be in function definition and in calling logic.
- Parameters are the names used inside function for values passed.
- Arguments are the names used when calling function.

*** =pre_exercise_code
```{python}
# InputDen has been defined for you; do not modify
def InputDen ():
    d = "5"
    d = int(d)
    return d

# CalcHeight has been defined for you; do not modify    
def CalcHeight (dt, dn):
    bills = dt // dn
    h = bills * .0043 * 2.54
    return h
    
# PrintHeight has been defined for you; do not modify    
def PrintHeight (ht,dn):
    print("Height of $",dn," bills to pay debt is ",round(ht,2), " centimeters", sep='')


```

*** =sample_code
```{python}
# InputDebt has been defined for you; do not modify except to set initial value of d
def InputDebt ():
    d = "____"
    d = int(d)
    return d

# Define function main.  
def ____ () ____
# Assign results of InputDebt to variable debt
    ____ = ____()
# Assign results of InputDen to variable den
    ____ = ____()
# Call CalcHeight, pass values debt and den.  Assign results to variable height
    ____ = ____(debt,den)
# Call PrintHeight, pass values height and den
    PrintHeight(____,____)
    
# Call main to start the program
____()

```

*** =solution
```{python}
# Complete details for PrintHeight based on instructions
def InputDebt ():
    d = "279383283987"
    d = int(d)
    return d

# Define function main.  
def main () :
# Assign results of InputDebt to variable debt
    debt = InputDebt()
# Assign results of InputDen to variable den
    den = InputDen()
# Call CalcHeight, pass values debt and den.  Assign results to variable height
    height = CalcHeight(debt,den)
# Call PrintHeight, pass values height and den
    PrintHeight(height,den)
    
# Call main to start the program
main()


```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_function("main", 
            not_called_msg = "Did you call function *main*?",
            incorrect_msg = "Check order of functions to call")

test_student_typed('d\s*=\s*"279383283987"',not_typed_msg="Check value assigned to variable *d* in *InputDebt*")

success_msg("Outstanding work!!")


```