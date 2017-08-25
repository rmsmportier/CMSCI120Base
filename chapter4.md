---
title       : Homework 3
description : CMSCI 120 Homework


--- type:NormalExercise lang:python xp:100 skills:1 key:fd2d31317f
## Combining Expressions and Building Blocks (2)

We can use the combination of expressions and the output building block to print designs to our screen.  Follow the instructions below.

*** =instructions
- Replace the ____ with "\*" in each open expression.

*** =hint
- Be sure to use "" around * to indicate that this is string data type

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Print the first line of design
print(____ * 19)

# Print the second line of design
print(____ + ' ' * 17 + ____)

# Print the third line of design
print(____ + ' ' * 17 + ____)

# Print the fourth line of design
print(____ * 19)

```

*** =solution
```{python}
# Print the first line of design
print("*" * 19)

# Print the second line of design
print("*" + ' ' * 17 + "*")

# Print the third line of design
print("*" + ' ' * 17 + "*")

# Print the fourth line of design
print("*" * 19)

```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

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
            incorrect_msg = "Check the string you specified for the fourth call to print.")
            
success_msg('Excellent work!!  Let\'s try another.')

```


--- type:NormalExercise lang:python xp:100 skills:1 key:5da1240b9e
## Combining Expressions and Building Blocks (3)

We can create flexibility in our program by using variables to store some of the values we previously typed.  Let's store the character to one variable, and the number of times to repeat to another.  You may not follow everything that is occurring with the print statements, but focus on how changing what is assigned to the variable changes the outcome.  See if you can determine the choice that was made in the print statement for how many times to repeat.

*** =instructions
- Assign the value '\*' to variable *a*; be sure to include the '' that indicate string type
- Assign the value 19 to variable *b*

*** =hint
- Use assignment operator as we have done previously, and string indicator for the character to assign

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Assign character to variable a
a ____ ____

# Assign number of times to repeat to variable b
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
# Assign character to variable a
a = "*"

# Assign number of times to repeat to variable b
b = 19

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
            incorrect_msg = "Check the string you specified for the fourth call to print.")
            
success_msg('Excellent work!!  You are doing well.')

```


--- type:NormalExercise lang:python xp:100 skills:1 key:252d420681
## Variables Create Flexibility

We can now easily modify our earlier program to print a different character, and a different number of times to the screen.  This time replace the value with variable *a* with '$', and the number of times with 37 for variable *b*.

*** =instructions
- Assign the value '$' to variable *a*; be sure to include the '' that indicate string type
- Assign the value 37 to variable *b*

*** =hint
- Use assignment operator as we have done previously, and string indicator for the character to assign

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Assign character to variable a
a ____ ____

# Assign number of times to repeat to variable b
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
# Assign character to variable a
a = "$"

# Assign number of times to repeat to variable b
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

success_msg('Excellent work!!  You are now programming in Python with 2 of 6 building blocks')

```

--- type:NormalExercise lang:python xp:100 skills:1 key:7522f73f67
## Variables Create Flexibility (2)

Let's modify our program even further.   Let's reduce those 2 identical print functions down to one.  What character could we put in place of ____ that would ensure we get identical output on different lines?  What value would we need to assign to end to make this work correctly?

*** =instructions
- Assign the value '#' to variable *a*; be sure to include the '' that indicate string type
- Assign the value 42 to variable *b*

*** =hint
- Use assignment operator as we have done previously, and string indicator for the character to assign

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Assign character to variable a
a ____ ____

# Assign number of times to repeat to variable b
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
# Assign character to variable a
a = "#"

# Assign number of times to repeat to variable b
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

Let's modify our program even further.   Now we are going to support a variable number of rows.  The first and last lines will be fixed.  We will use the value in a variable to determine how many additional lines to print.

*** =instructions
- Assign the value '&' to variable *a*; be sure to include the '' that indicate string type
- Assign the value 57 to variable *b*
- Assign the value 8 to variable *c*

*** =hint
- Use assignment operator as we have done previously, and string indicator for the character to assign

*** =pre_exercise_code
```{python}
```

*** =sample_code
```{python}
# Assign character to variable a
a ____ ____

# Assign number of times to repeat to variable b
b ____ ____

# Assign number of rows to variable c
c ____ ____

# Print the first line of design
print(a * b)

# Print the these lines the number of times in c minus the 2 rows printed at start and finish.
print((a + ' ' * (b-2) + a + "\n") * (____ - ____), end = "")

# Print the fourth line of design
print(a * b)

```

*** =solution
```{python}
# Assign character to variable a
a = "&"

# Assign number of times to repeat to variable b
b = 57

# Assign number of rows to variable c
c = 8

# Print the first line of design
print(a * b)

# Print the these lines the number of times in c minus the 2 rows printed at start and finish.
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

success_msg('Excellent work!!  You are now programming in Python, and have mastered 2 of the 6 building blocks including expressions and the *print* function.')

```







