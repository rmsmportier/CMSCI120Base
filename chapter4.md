---
title       : Homework 3
description : CMSCI 120 Homework


--- type:NormalExercise lang:python xp:100 skills:1 key:fd2d31317f
## Combining Expressions and Building Blocks (2)

We can use the combination of expressions and the output building block to print designs to our screen.  Follow the instructions below.

*** =instructions
- Replace the ____ with "\*" in each open expression.

*** =hint
- Be sure to use "" around * to indicate that this is str data type

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
            incorrect_msg = "Check the string you specified for the first call to print.")
            
test_function("print", index=3,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the first call to print.")
            
test_function("print", index=4,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the first call to print.")
            
success_msg('Excellent work!!  Let\'s try another.')

```


--- type:NormalExercise lang:python xp:100 skills:1 key:5da1240b9e
## Combining Expressions and Building Blocks (3)

We can create flexibility in our program by using variables to store some of the values we previously typed.  Let's store the character to one variable, and the number of times to repeat to another.  You may not follow everything that is occurring with the print statements, but focus on how changing what is assigned to the variable changes the outcome.

*** =instructions
- Assign the value '\*' to variable *a*; be sure to include the '' that indicate str type
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
            incorrect_msg = "Check the string you specified for the first call to print.")
            
test_function("print", index=3,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the first call to print.")
            
test_function("print", index=4,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the first call to print.")
            
success_msg('Excellent work!!  You are doing well.')

```


--- type:NormalExercise lang:python xp:100 skills:1 key:252d420681
## Variables Create Flexibility

We can now easily modify our earlier program to print a different character, and a different number of times to the screen.  This time replace the value with variable *a* with '$', and the number of times with 37 for variable *b*.

*** =instructions
- Assign the value '$' to variable *a*; be sure to include the '' that indicate str type
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
            incorrect_msg = "Check the string you specified for the first call to print.")
            
test_function("print", index=3,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the first call to print.")
            
test_function("print", index=4,
            not_called_msg = "Did you remove the call to print?",
            incorrect_msg = "Check the string you specified for the first call to print.")
            
success_msg('Excellent work!!  You are now programming in Python, and have mastered 2 of the 6 building blocks.')

```



