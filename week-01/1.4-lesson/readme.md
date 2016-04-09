# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Intro to Python 2
Week 1 | Lesson 1.4

### LEARNING OBJECTIVES
*After this lesson, you will be able to:*
- Create lists and operate on them
- Create dictionaries and operate on them

### STUDENT PRE-WORK
*Before this lesson, you should already be able to:*
- Define/describe/explain a list and a dictionary

<a name="introduction"></a>
## Introduction: Lists and dictionaries (10 mins)

In our last lesson, we went over the six Python data types.

<details>
<summary>
What were they?
</summary>
```bash
- Integers
- Floats
- Strings
- Tuples
- Lists
- Dictionaries
```
</details>

Lists and dictionaries are the most fundamental data structures in Python. In this lesson, we'll be learning to create and perform operations on them.

Turn and Talk: Work in pairs and white table the definitions of list and dictionary.

<details>
<summary>
Lists
</summary>
```bash
- A collection of values
- Can be changed; not fixed
- Each value has a number associated with it, starting at 0
- Denoted by square brackets
A list of values. Each one of them is numbered, starting from zero - the first one is numbered zero, the second 1, the third 2, etc. You can remove values from the list, and add new values to the end. Example: The names of your friends.
```
</details>

<details>
<summary>
Dictionaries
</summary>
```bash
In a dictionary, you have an index of words, and for each of them a definition. In Python, the word is called a key, and the definition a value. The values in a dictionary are not numbered - they are not in any specific order, either - the key does the same thing. You can add, remove, and modify the values in dictionaries. Example: telephone book.
```
</details>

[Lists and Dictionaries](http://sthurlow.com/python/lesson06/)


<a name="demo"></a>
## Guided Practice: Lists (30 mins)

Lists are extremely similar to tuples.

<details>
<summary>
Why would we use a list over a tuple?
</summary>
```bash
Lists are modifiable (mutable), so their values can be changed. Most of the time we use lists, not tuples, because we want to easily change the values of things if we need to.
```
</details>

Say you have FIVE friends, called Curly, Moe, Larry, Tweedle Dee and Tweedle Dumb. Let's create a list.

How do we create a list?

<details>
<summary>
In the Python shell type:
</summary>
```bash
friends = ['Curly', 'Moe', 'Larry', 'Tweedle Dee', 'Tweedle Dumb']
```
</details>

then type:
```bash
friends
```

Let's print the 3rd friend in your list.

<details>
<summary>
In the Python shell type:
</summary>
```bash
print friends[2]
```
</details>

<details>
<summary>
and it returns:
</summary>
```bash
Larry
```
</details>

Let's add to the list.

In the Python shell type:
```bash
friends.append('Samwise Gamgee')
```

then type:
```bash
friends
```

<details>
<summary>
and it returns:
</summary>
```bash
['Curly', 'Moe', 'Larry', 'Tweedle Dee', 'Tweedle Dumb', 'Samwise Gamgee']
```
</details>

append() is what we call a built-in list operation for Python. Let's play around with a some more.

Let's remove your 4th friend using del.

<details>
<summary>
In the Python shell type:
</summary>
```bash
del friends[3]
```
</details>

then type:
```bash
friends
```

<details>
<summary>
and it returns:
</summary>
```bash
['Curly', 'Moe', 'Larry', 'Tweedle Dumb', 'Samwise Gamgee']
```
</details>


[Lists](http://sthurlow.com/python/lesson06/)


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
