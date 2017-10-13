---
title       : Homework 7
description : CMSCI 120 Homework


--- type:NormalExercise lang:python xp:100 skills:1 key:fd2d31317f
## Let's Practice Iterations

Iterations provide our final building block.  Iterations enable us to repeat existing code until a desired condition has been met.  This means iterations and conditionals are very closely connected.

There are 2 types of iterations in computer science, determinate and indeterminate.  Determinate repeats instructions a set number of times, a value that is known when the loop starts.  Indeterminate loop continues until a condition has been met, but we do not know when that will occur.

Let's start with a determinate loop, the *for* loop.


*** =instructions
- Modify the Python commands to put the value *5* in *range* function
- This will execute the commands inside the iteration 5 times
- *range* generates an iterable structure like a *tuple* that contains the values 0, 1, 2, 3, 4

*** =hint
- Put *5* as argument to *range()*

*** =pre_exercise_code
```{python}

```

*** =sample_code
```{python}
# Modify range statement with value 5

for i in range(____):
    print("How many times does this print?")

```

*** =solution
```{python}
# Modify range statement with value 5

for i in range(5):
    print("How many times does this print?")

```
