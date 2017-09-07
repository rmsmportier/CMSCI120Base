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
            
success_msg('Nice work.  Notice that spaces have lower value than letters, and that capital letters have lower value than lower case letters.  Also notice that for all calls we created a grouping of values by using either () or "" around the full set of values to evaluate.')

```


--- type:NormalExercise lang:python xp:100 skills:1 key:252d420681
## Built In Functions (3)

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


