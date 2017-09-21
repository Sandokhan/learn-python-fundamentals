---
title       : Python fundamentals
description : You will learn python fundamentals

--- type:VideoExercise lang:python xp:50 skills:2 key:116c4daea5
## Welcome to Python fundamentals

*** =projector_key
b22a991dcada93b36e50672341a2a20a


--- type:VideoExercise lang:python xp:50 skills:2 key:890443c0f1 video_link: //player.vimeo.com/video/125848316
## Short Python introduction


--- type:NormalExercise lang:python xp:100 skills:2 key:7d47c9d6aa
## Hello World!


*** =instructions
Python is a very simple language, and has a very straightforward syntax. It encourages programmers to program without boilerplate (prepared) code. The simplest directive in Python is the "print" directive - it simply prints out a line (and also includes a newline, unlike in C).

*** =hint
Use the `print` method to print out `Hello World!`

*** =pre_exercise_code
```{python}

```

*** =sample_code
```{python}
# Print out Hello World!

```

*** =solution
```{python}
# Print the "Hello World!" to the shell
print("Hello World!")
```

*** =sct
```{python}
test_output_contains("Hello World!")
success_msg("Great job! Now onto the next thing!")
```



--- type:NormalExercise lang:python xp:100 skills:2 key:dbf06a98db
## Variables


*** =instructions
Python is completely object oriented, and not "statically typed". You do not need to declare variables before using them, or declare their type. Every variable in Python is an object.

Let's try to define a `myint` variable which should hold number 7 and then use our `print` skills from the previous exercise to print the value out.

*** =hint
Declare `myint` variable and use `=` operator to assign a value to it.


*** =pre_exercise_code
```{python}

```

*** =sample_code
```{python}
# Assigning value to a variable is done by using the `=` equality operator
myint = 

# Print out the value of myint

```

*** =solution
```{python}
myint = 7
print(myint)
```

*** =sct
```{python}
test_object("myint");
test_output_contains("7", pattern = False, no_output_msg = "Was number 7 printed out?")
```
