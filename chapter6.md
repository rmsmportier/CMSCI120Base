---
title       : Homework 5
description : CMSCI 120 Homework


--- type:NormalExercise lang:python xp:100 skills:1 key:fd2d31317f
## Creating a Function Framework

Functions provide a powerful element related to computer programming, as we can expand our base programming language to create our own functions.  These enable us to use our functions interchangeably with tokens and built-in functions provided within the programming language.

This is highly useful when developing large systems, as individual programmers can code functions that seamlessly integrate together once completed.  Additionally, we can avoid repeating the same code over and over within the larger system.  This ensures that when we need to change the program, we only change in one place versus many.

Additional benefits include reduced maintenance costs for the resulting application, faster development time, ability to swap out capability easily for updated capability in the future, simplified testing, and the list goes on and on.

We are going to build a new program to achieve the following:
    *Prompt for a debt amount owed by a consumer, and for a US currency denomination from the following possibilities ($1, $5, $10, $20, $50, $100).  Calculate the height of bills required to pay that debt for that denomination knowing that the thickness of every U.S. denomination bill is 0.0043 inches.  Calculate the height in centimeters knowing there are 2.54 centimeters in 1 inch.  Print the result with appropriate text describing what was entered and what was calculated.*

*** =instructions
- Create the function framework needed to deliver our program.  
- Try creating CFD for this program before you begin in order to align each task with the functions we will create
- Create a function definition called InputDebt; add print statement indicating "Inside InputDebt"
- Create a function definition called InputDen; add print statement indicating "Inside InputDen"
- Create a function definition called CalcHeight; add print statement indicating "Inside CalcHeight"
- Create a function definition called PrintHeight; add print statement indicating "Inside PrintHeight"

*** =hint
- Create functions that align with instructions.  Remember the important elements to create function
- *define* the function
- *name* the function
- *indicate* it is a function
- *indicate more* to come

*** =pre_exercise_code
```{python}

```

*** =sample_code
```{python}
# Create function InputDebt; print output indicated in instructions
def ____ ____ ____ :
    print("____")
    
# Create function InputDen; print output indicated in instructions
def ____ () ____
    print("____")
    
# Create function CalcHeight; print output indicated in instructions
def ____ ____ ____ :
    print("____")
    
# Create function PrintHeight; print output indicated in instructions
def ____ ____ ____ :
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

test_student_typed("def\\sInputDebt\\s\\(\\)\\s:",not_typed_msg="Check your function definition for the function InputDebt")

test_student_typed("def\\sInputDen\\s\\(\\)\\s:",not_typed_msg="Check your function definition for the function InputDen")

test_student_typed("def\\sCalcHeight\\s\\(\\)\\s:",not_typed_msg="Check your function definition for the function CalcHeight")

test_student_typed("def\\sPrintHeight\\s\\(\\)\\s:",not_typed_msg="Check your function definition for the function PrintHeight")

test_function("print", index=1,
            not_called_msg = "Do not remove print function.",
            incorrect_msg = "Check instructions for the string to print")

test_function("print", index=2,
            not_called_msg = "Do not remove print function.",
            incorrect_msg = "Check instructions for the string to print")

test_function("print", index=3,
            not_called_msg = "Do not remove print function.",
            incorrect_msg = "Check instructions for the string to print")

test_function("print", index=4,
            not_called_msg = "Do not remove print function.",
            incorrect_msg = "Check instructions for the string to print")
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

*** =hint
- We want value assigned to variable to be string with specified value
- What function have we used that will convert data type to integer?  Once converted, remember to store the value back in the variable in main memory
- What Python syntax returns value in a variable?
- Call *InputDebt*, and save returned value to variable *debt*

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
# Create function InputDebt; print output indicated in instructions
def InputDebt ():
    d = "2376495"
    d = int(d)
    return d
    
debt = InputDebt()


```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_student_typed('d\\s=\\s"2376495"',not_typed_msg="Check your value assigned to *d* inside function.")

test_student_typed("d\\s\\=\\sint\\(debt\\)",not_typed_msg="Check your type casting function for *d* inside function.")

test_function("InputDebt", 
            not_called_msg = "Check the function definition for *InputDebt*.",
            incorrect_msg = "Check requirements for details related to *InputDebt*, and ensure you returned value from the function.")
            
test_object("debt",
            undefined_msg = "Did you create variable *debt*?",
            incorrect_msg = "Check the syntax used to assign value to *debt*, and the value returned from *InputDebt*.")
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

*** =hint
- We want value assigned to variable to be string with specified value
- What function have we used that will convert data type to integer?  Once converted, remember to store the value back in the variable in main memory
- What Python syntax returns value in a variable?
- Call *InputDen*, and save returned value to variable *den*

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
# Create function InputDen; print output indicated in instructions
def InputDen ():
    d = "5"
    d = int(den)
    return d
    
den = InputDen()


```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_student_typed('d\\s=\\s"5"',not_typed_msg="Check your value assigned to *d*.")

test_student_typed("d\\s\\=\\sint\\(d\\)",not_typed_msg="Check your type casting function for *d*")

test_function("InputDen", 
            not_called_msg = "Check the function definition for *InputDen*.",
            incorrect_msg = "Check requirements for details related to *InputDen*, and ensure you returned value from the function.")
            
test_object("den",
            undefined_msg = "Did you create variable *den*?",
            incorrect_msg = "Check the syntax used to assign value to *den*, and the value returned from *InputDen*.")
```

--- type:NormalExercise lang:python xp:100 skills:1 key:1ef3035953
## Build Out Calculation Function

Let's make the calculation function operational.  

*** =instructions
- Variables *debt* and *den* previously created still exist in your workspace
- Modify the function definition for *CalcHeight* to accept these 2 values.  Call the parameters in the function definition *dt* and *dn*
- Calculate the number of bills needed to pay the debt using indicated denomination.  You cannot have partial bills, so use of floor (integer) division would be helpful.  Assign this value to variable *bills*.
- Convert the number of bills to a height in cm using .0043 inches/bill and 2.54 cm/inch.  Assign this value to variable *h*.
- Return the calculated value to the calling logic
- Call *CalcHeight* passing the contents of variable *debt* and variable *den*.  Assign the result to variable *height*.

*** =hint
- If we are sending values to function, names to represent this need to be in function definition and in calling logic
- Parameters are the names used inside function for values passed
- Arguments are the names used when calling function 
- Floor division is one of these operators, // or %
- You will use combination of either * or \\\ operator to convert units

*** =pre_exercise_code
```{python}
debt = 2376495
den = 5
```

*** =sample_code
```{python}
# Complete details for CalcHeight based on instructions
def CalcHeight (____,____):
    ____ = ____
    ____ = bills * ____ * ____
    ____ ____

____ = CalcHeight()

```

*** =solution
```{python}
# Complete details for CalcHeight based on instructions
def CalcHeight (dt, dn):
    bills = dt//dn
    h = bills * .0043 * 2.54
    return h
    
height = CalcHeight(debt,den)


```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_student_typed('dt,\\sdn',not_typed_msg="Check parameter names for function.")

test_student_typed("bills\\s\\=\\sdt\\s\\/\\/\\sdn",not_typed_msg="Check your calculation for *bills*.")

test_student_typed("h\\s\\=\\sbills\\s\\*\\s\\.0043\\s\\*\\s\\2\\.54",not_typed_msg="Check your calculation for *h*.")

test_function("CalcHeight", 
            not_called_msg = "Check the function definition for *CalcHeight*.",
            incorrect_msg = "Check requirements for details related to *CalcHeight*, and ensure you returned value from the function.")
            
test_object("height",
            undefined_msg = "Did you create variable *height*?",
            incorrect_msg = "Check the syntax used to assign value to *height*, and the value returned from *CalcHeight*.")
```