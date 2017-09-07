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


