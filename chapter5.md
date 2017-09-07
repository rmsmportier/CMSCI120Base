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
- Generate the listing of available functions by highlighting both lines, and pressing Ctrl-Enter at same time.  Once you have looked through the listing, press *Submit Answer*

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
            
success_msg("That's it.  *dir* is itself a function that provides a directory or listing of all available functions.  We have to specify what type of listing we want.  *builtins* indicates that we want those functions that are part of base Python.  Notice the beginning of the listing contains names that align with error messages we have seen like NameErrors.  The first part of the list indicates all existing runtime errors in Python.  For now, just remember where we found them.  We will come back to this later.')

```


--- type:NormalExercise lang:python xp:100 skills:1 key:5da1240b9e
## Built In Functions (2)

We can use another function *help* to assist us in understanding what any of these functions will do, and how to use the selected function.  Let's try this with a few built-in functions we have not previously used.

In the shell, enter *help(min)* and *help(max)*.  Look at the description to understand what each does. Then complete the following:

*** =instructions
- Pick one of the 2 functions to find the largest value in the group of numbers provided
- Pick one of the 2 functions to find the smallest value in the group of numbers provided
- Use the *min* function with a string "This is a test, this is only a test" to see the *smallest* value in the string.
- Use the *max* function with a string "This is A test, this is only a test" to see the *smallest* value in new string.
- Pick one of the 2 functions which has greater value in computer, "A" or "a".

*** =hint
- Replace ____ with appropriate function to accomplish stated goal.  You can use *help()* with function name passed to *help* in order to assist in selecting correct function.

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Find the smallest value in grouping of numbers
print(____(3, 4, 5, 9, 1, -4))

# Find the largest value in grouping of numbers
print(____(9, 2, 20, -4, -20, 7))

# Use min with string to find the smallest value in string
print(min("_____"))

# Use max with string to find the greatest value in string
print(max("____"))

# Identify which has greater value
print(____(("A","a")))

```

*** =solution
```{python}
# Find the smallest value in grouping of numbers
print(min(3, 4, 5, 9, 1, -4))

# Find the largest value in grouping of numbers
print(max(9, 2, 20, -4, -20, 7))

# Use min with string to find the smallest value in string
print(min("This is a test, this is only a test"))

# Use max with string to find the greatest value in string
print(max("This is A test, this is only a test"))

# Identify which has greater value
print(max(("A","a")))

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_function("print", index=1,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the function you selected for the first call to print.")
            
test_function("print", index=2,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the function you selected for the second call to print.")
            
test_function("print", index=3,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string in the third call to print.")
            
test_function("print", index=4,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string in the fourth call to print.")
            
test_function("print", index=5,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the function you selected for the fifth call to print.")
            
success_msg('Nice work.  Notice that spaces have lower value than letters, and that capital letters have lower value than lower case letters.  Also notice that for all calls we created a grouping of values by using either () or "" around the full set of values to evaluate.  When the grouping is done with () and , we have created a tuple.  When we use "", we have created a string with multiple characters.')

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
            incorrect_msg = "Check the values you entered, and the function name.")
            
test_function("print", index=2,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the function you selected.")
            
test_function("print", index=3,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the values you entered, and the function name.")
            
test_function("print", index=4,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Are you calling round to the correct number of decimal places?")

success_msg('Nice job!!  Did you notice that *divmod* returned a tuple of values, and that those values were the integer division and modulus combined together?')

```

--- type:NormalExercise lang:python xp:100 skills:1 key:7522f73f67
## Built In Functions (4)

There are also several nice functions we can use with string data.  Let's experiment with just 2 of them.  Every character in the computer is actually calculated as a number before converting to binary code.  These decimal equivalents allow us to do arithmetic with characters.  This is something that proves very helpful related to encryption algorithms.  We will spend some time on these in lab 4 this week.

*** =instructions
- Use the *ord* function to identify the numeric value for "A"
- Use the *ord* function to identify the numeric value for "a"
- Take the difference between *ord* result for "a" and *ord* result for "A"
- Use the *chr* function to identify the character with decimal value 104
- Use the *chr* function to identify the character with decimal value 128
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
print(____(____))- ____(____))

# Use chr to identify character for 104
print(____(____))

# Use chr to identify character for 128
print(____(____))

# Combine ord and chr to find character 5 greater than "E"
print(____(____(____) + ____))

```

*** =solution
```{python}
# Use ord to determine numeric value for "A"
print(ord("A"))

# Use ord to determine numeric value for "a"
print(ord("A"))

# How far apart are the values "A" and "a"
print(ord("a"))- ord("A"))

# Use chr to identify character for 104
print(chr(104))

# Use chr to identify character for 128
print(chr(128))

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
            incorrect_msg = "Check the function and value(s) you specified.  You need to do arithmetic, so you need to convert character values to decimal.  Which function would do this?")

test_function("print", index=4,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the function and value you specified.")
            
test_function("print", index=5,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the function and value you specified.")
            
test_function("print", index=6,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the order in which you are calling functions, and the value you are adding.  Change the 'E' to decimal, add the value, then convert back to character.")
            
success_msg('Nice work; let's move on to add-in functions')

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


