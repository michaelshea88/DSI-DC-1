---
title: Intro to Python 2
duration: "1:5"
creator:
    name: Lucy Williams
    city: DC
---

# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Intro to Python 2
Week 1 | Lesson 1.3

### LEARNING OBJECTIVES
*After this lesson, you will be able to:*
- Create lists and operate on them
- Create dictionaries and operate on them

### STUDENT PRE-WORK
*Before this lesson, you should already be able to:*
- Define/describe/explain a list and a dictionary

### LESSON GUIDE
| TIMING  | TYPE  | TOPIC  |
|:-:|---|---|
| 10 min  | [Introduction](#introduction)   | Lists and dictionaries  |
| 30 min  | [Demo / Codealong / Guided Practice](#demo)  | Lists  |
| 5 min  | [Independent Practice](#ind-practice)  | Lists  |
| 30 min  | [Demo / Codealong / Guided Practice](#demo)  | Dictionaries  |
| 5 min  | [Independent Practice](#ind-practice)  | Dictionaries  |
| 10 min  | [Conclusion](#conclusion)  |  |


<a name="introduction"></a>
## Introduction: Lists and dictionaries (10 mins)
Lists are what they seem - a list of values. Each one of them is numbered, starting from zero - the first one is numbered zero, the second 1, the third 2, etc. You can remove values from the list, and add new values to the end. Example: Your many friends' names.

Dictionaries are similar to what their name suggests - a dictionary. In a dictionary, you have an 'index' of words, and for each of them a definition. In python, the word is called a 'key', and the definition a 'value'. The values in a dictionary aren't numbered - they aren't in any specific order, either - the key does the same thing. You can add, remove, and modify the values in dictionaries. Example: telephone book.

[Lists and Dictionaries](http://sthurlow.com/python/lesson06/)


<a name="demo"></a>
## Demo / Codealong / Guided Practice: Lists (30 mins)

Lists are extremely similar to tuples. Lists are modifiable (mutable), so their values can be changed. Most of the time we use lists, not tuples, because we want to easily change the values of things if we need to.

Lists are defined very similarly to tuples. Say you have FIVE friends, called Curly, Moe, Larry, Tweedle Dee and Tweedle Dumb. Let's create a list.
In Jupyter notebook type:
```bash
friends = ['Curly', 'Moe', 'Larry', 'Tweedle Dee', 'Tweedle Dumb']
```

then type:
```bash
friends
```

and it returns:
```bash
['Curly', 'Moe', 'Larry', 'Tweedle Dee', 'Tweedle Dumb']
```

Let's print the 3rd friend in your list.
In Jupyter notebook type:
```bash
print friends[2]
```

and it returns:
```bash
Larry
```

Let's add to the list.
In Jupyter notebook type:
```bash
friends.append('Samwise Gamgee')
```

then type:
```bash
friends
```

and it returns:
```bash
['Curly', 'Moe', 'Larry', 'Tweedle Dee', 'Tweedle Dumb', 'Samwise Gamgee']
```
Samwise Gamgee has been added to the end of your friends list.

Let's remove your 4th friend.
In Jupyter notebook type:
```bash
del friends[3]
```

then type:
```bash
friends
```

and it returns:
```bash
['Curly', 'Moe', 'Larry', 'Tweedle Dumb', 'Samwise Gamgee']
```
Tweedle Dee has been removed.


[Lists](http://sthurlow.com/python/lesson06/)

**Check**: Why are lists used more often then tuples?
Why did we use 'del friends[3]' to remove the 4th friend and not 'del friends[4]'?


<a name="ind-practice"></a>
## Independent Practice: Topic (5 minutes)
Suggestions:
Create your own list
Return only one element in the list
Add/delete something to the list


<a name="demo"></a>
## Demo / Codealong / Guided Practice: Dicitonaries (30 mins)

Now you have a list of your friends, but let's say you want to call them. A list won't
do, you need to associate your friends with their phone numbers. You need a telephone
book. For this we need a dictionary. We know that dictionaries have keys and values.
In other words, your friends' names would be the keys and their phone numbers
would be the values.

When you initially create a dictionary, it is very much like making a tuple or list.
Tuples have ( and ) things, lists have [ and ] things. Guess what! dictionaries
have { and } things - curly braces.

In Jupyter notebook type:
```bash
# Make the phone book:
phonebook = {'Curly':123456, 'Moe':789012, 'Larry':345678, 'Tweedle Dee':901234, 'Tweedle Dumb':567890}
```

then type:
```bash
phonebook
```

and it returns:
```bash
{'Curly': 123456,
 'Larry': 345678,
 'Moe': 789012,
 'Tweedle Dee': 901234,
 'Tweedle Dumb': 567890}
```

Let's add a new friend to the phonebook.
In Jupyter notebook type:
```bash
phonebook['Humpty Dumpty'] = 234567
```

then type:
```bash
phonebook
```

and it returns:
```bash
{'Curly': 123456,
 'Humpty Dumpty': 234567,
 'Larry': 345678,
 'Moe': 789012,
 'Tweedle Dee': 901234,
 'Tweedle Dumb': 567890}
```

Let's delete a friend to the phonebook.
In Jupyter notebook type:
```bash
del phonebook['Curly']
```

then type:
```bash
phonebook
```

and it returns:
```bash
{'Humpty Dumpty': 234567,
 'Larry': 345678,
 'Moe': 789012,
 'Tweedle Dee': 901234,
 'Tweedle Dumb': 567890}
```

Let's create a new dictionary with nothing in it to start with:
In Jupyter notebook type:
```bash
ages = {}
```

Now, let's add some names and ages to the dictionary.
```bash
ages['Humpty Dumpty'] = 23
ages['Larry'] = 19
ages['Moe'] = 78
ages['Tweedle Dee'] = 45
```

[Dictionaries](http://sthurlow.com/python/lesson06/)

**Check**:
() are used for tuples, lists, or dictionaries?
[] are used for tuples, lists, or dictionaries?
{} are used for tuples, lists, or dictionaries?


<a name="ind-practice"></a>
## Independent Practice: Topic (5 minutes)
Suggestions:
Create your own dictionary
Return only one element in the dictionary
Add/delete something to the dictionary

<a name="conclusion"></a>
## Conclusion (10 mins)
- Partner up and explain what a list and a dictionary are to your partners
- What are the differences between a list and a dictionary?
- What are the two things you need for a dictionary?

## Bonus Challenges
Once you've mastered the basics, further your understanding of Python by attempting "[Alternate Code Challenges 2](code/starter-code/Alternate%20Code%20Challenges%20-%20Week%201%20Lesson%201.2.ipynb)".
