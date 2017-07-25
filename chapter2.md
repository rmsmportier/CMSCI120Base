---
title       : Lab 2
description : CMSCI 120 Lab Assignment

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