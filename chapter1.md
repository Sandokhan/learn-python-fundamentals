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
Python is completely object oriented, and not "statically typed". You do not need to declare variables before using them, or declare their type. Every variable in Python is an object. tipoa

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


--- type:NormalExercise lang:python xp:100 skills:2 key:6d30662fe5
## Lists


*** =instructions
Lists are very similar to arrays. They can contain any type such as strings, integers or floats. Lists can also be iterated over in a very simple manner.

Lists are defined by signing a `[]` to a variable. An example would be:
```{python}
mylist = []
```

Try to define a list of numbers where numbers are `1, 2, 3, 4, 5`. Keep in mind that items in a list are comma separated.

*** =hint
Create a new variable with name `mylist` and assigning an `[]` (array) to it.
Numbers should be within the square brackets.

*** =pre_exercise_code
```{python}

```

*** =sample_code
```{python}
# Create a list variable
mylist = 
```

*** =solution
```{python}
mylist = [1,2,3,4,5]
```

*** =sct
```{python}
test_object("mylist", undefined_msg = "Make sure mylist variable has been defined", incorrect_msg = "mylist should have an array of numbers starting from 1 to 5")
success_msg("Look at that, the list of awesomness!!!")
```



--- type:MultipleChoiceExercise lang:python xp:50 skills:2 key:14b680a8b0
## Let's verify our new skills!

How do we define a new variable?

*** =instructions
- `new_variable(1)`
- `new_variable = 1`
- `new_variable / 1`

*** =hint
If you cannot remember then try to check the Variables exercise :)

*** =sct
```{python}
test_mc(correct = 2, 
        msgs = ["Arrrgh close enough! Try to revisit the variables exercise!",
                "Oh yes you are on fire!",
                "Hm! Try to revisit the variables exercise!"])
```


--- type:MultipleChoiceExercise lang:python xp:50 skills:2 key:efbe5d8717
## Let's verify your new skills!

How do we define a variable holding an array of Strings?

*** =instructions
- `mylist = [1,2,3]`
- `mylist = ["1", 2, "3"]`
- `mylist = ["a", "1", "c"]`

*** =hint
If you are not sure then go check the lists exercise :)

*** =sct
```{python}
test_mc(correct = 3,
        msgs = ["Huh close enough, try again!",
                "Arrgs now even close, try once more!",
                "Way to go lad!"])
```



--- type:PlainMultipleChoiceExercise lang:python xp:50 skills:2 key:32c0f3f63c
## Do you like Python?


*** =instructions
- Yes
- No

*** =hint
You do like Python!

*** =sct
```{python}
test_mc(correct = 1,
        msgs = ["Way to go! Hip hip hurray!",
                "Ah, seems I didn't really do a good job, did I?"])
```

--- type:NormalExercise lang:python xp:100 skills:2 key:7f9acbf25d
## Working with imported data


*** =instructions
Often you will want to import data from csv files and create a list out of it so you can work with the data and shape it to your likings.
Who knows maybe you will even want to save the changed data to the file.

Behind the scenes we have loaded a sample csv data set and assigned it to a variable named `csvdata`.
Feel free to print the data to see how it looks. (don't be overwhelmed by amount of data we've put in :))

Your task is to print the

*** =hint


*** =pre_exercise_code
```{python}
import pandas as pd
csvdata = pd.read_csv('https://s3.amazonaws.com/assets.datacamp.com/production/course_5485/datasets/FL_insurance_sample.csv', index_col = 0)
```

*** =sample_code
```{python}
# There is some data assigned to a variable csvdata see if you can print it out

```

*** =solution
```{python}
# There is some data assigned to a variable csvdata see if you can print it out
print(csvdata)
```

*** =sct
```{python}
test_function("print")
```
