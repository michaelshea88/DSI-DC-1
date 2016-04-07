---
title: Programming Fundamentals and Python 1

---

# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Programming Fundamentals and Python 1

Week 1 | Lesson 1.3


### LEARNING OBJECTIVES
*After this lesson, you will be able to:*
- Define what a programming language is
- Differentiate between frontend and backend languages
- Define integers, strings, tuples, lists, and dictionaries
- Demonstrate arithmetic operations and string operations
- Demonstrate variable assignment

### STUDENT PRE-WORK
*Before this lesson, you should already be able to:*
- Describe/define Python data types

## Programming Languages (10 mins)
<details>
<summary>
Turn and Talk: What is a programming language?
</summary>
```bash
Programming languages are how we communicate a sequence of instructions to a computer. Each language has a precise form (syntax) and precise meaning (semantics). We are not able to do this with human languages because they are not suited to understanding complex algorithms.
```
</details>

### Front-end Languages

Languages that have to do with what the user sees and interacts with. These are also called client side languages. For example, when
you go to ebay, you're interacting with the front-end.

http://www.ebay.com/

<details>
<summary>
HTML
</summary>
```bash
Structure
```
</details>

<details>
<summary>
CSS
</summary>
```bash
Style
```
</details>

<details>
<summary>
Javascript
</summary>
```bash
Behavior
```
</details>

### Back-end Languages

Back-end programming typically consists of a server, an application and a database. Back to the ebay example, when you register as a seller,
the application is storing your information in a database that was created on a server. A server is basically another computer reachable by the user(client) computer, but it's remote and it's mainly used to process and store data.

Examples of back-end languages include R, PHP, Python and Ruby.

In this class, we'll be learning Python.

Why?
- It's free
- Relatively simple to code and understand. Less steep of a learning curve than R, a popular statistical language.
- Has lots of data science libraries, frameworks, modules and toolkits.

## Python Data Types (5 mins)

<details>
<summary>
Integers
</summary>
```bash
Whole numbers from negative infinity to infinity, such as 1, 0, -5, etc.
```
</details>

<details>
<summary>
Float
</summary>
```bash
short for "floating point number," any rational number, usually used with decimals such as 2.8 or 3.14159.
```
</details>

<details>
<summary>
Strings
</summary>
```bash
A set of letters, numbers, or other characters.
"Frank Underwood, I am your father."
```
</details>

<details>
<summary>
Tuples
</summary>
```bash
A list with a fixed number of elements. ie x=(1,2,3) parentheses makes it a tuple.
x = ("Kirk", "Picard", "Spock")"Frank Underwood, I am your father."
```
</details>

<details>
<summary>
Lists
</summary>
```bash
A list without a fixed number of elements. ie x=[1,2,3] note the square brackets, a list
x = ["Lord", "of", "the", "Rings"]
```
</details>

<details>
<summary>
Dictionaries
</summary>
```bash
A type with multiple elements i.e. x = {1: 'a','b': 2,3: 3} where you address the elements with, e.g., a text.
x = {'key1':'value1', 'key2':'value2'}
```
</details>

[Python Basic data types](https://en.wikiversity.org/wiki/Python/Basic_data_types)


<a name="demo"></a>
## Demo Integers (5 min)

#### Integers
Integers are numeric values and can be stored, manipulated, and expressed inside variables without quotes.

In the Python shell type:
```bash
23
```
<details>
<summary>
and it returns:
</summary>
```bash
23
```
</details>

In the Python shell type:
```bash
-44
```
<details>
<summary>
and it returns:
</summary>
```bash
-44
```
</details>

You can also perform basic math using integers as well. In Python notebook type:
```bash
45-19
```
<details>
<summary>
and it returns:
</summary>
```bash
26
```
</details>

## Demo: Strings (5 min)

#### Strings
Strings are a type. They are the basic unit of text in Python and all the other types except integers may contain strings.

In the Python shell type:
```bash
"I love Darth Vader"
```
<details>
<summary>
and it returns:
</summary>
```bash
'I love Darth Vader'
```
</details>

You can also make a variable refer to a string. Note that a variable name can really be anything.
It should be semantic though.

In the Python shell type:

```bash
hello= "it's me"
```
Now type:
```bash
hello
```
<details>
<summary>
and it returns:
</summary>
```bash
"it's me"
```
</details>

Now type:
```bash
print(hello)
```
<details>
<summary>
and it returns:
</summary>
```bash
Luke, I am your father
```
</details>

The print command prints the value that 'x' stands for on the screen. It removes the quotations. Whenever you type something into a type that isn't an integer, syntax (the commands that you give python, such as print), or variable (such as x just was) you need to put it into quotations. You can use 'single' or "double" quotations.


## Demo: Tuples (5 min)
#### Tuples
A tuple is an unchangeable sequence of values.
When you typed ('I love Python') you only included one element.
In the Python shell type:
```bash
x = ("Kirk", "Picard", "Spock")
```
When you do this you create a tuple with three elements. You can access these elements individually by typing the variable and the then inside brackets directly to the right of the variable type the number of the element to which you are referring.

Now type:
```bash
print(x[1])
```
<details>
<summary>
and it returns:
</summary>
```bash
Picard
```
</details>


You may think that it is odd that it returned element 2 instead of element 1. The reason that it did this is because Python starts numbering at 0. element 1 = 0, element 2= 1, element 3= 2. You can also call on the elements in reverse order.

Now type:
```bash
print(x[-1])
```
<details>
<summary>
and it returns:
</summary>
```bash
Spock
```
</details>


## Demo: Lists (5 min)
#### Lists
A list is a changeable sequence of data. A list is contained by square brackets i.e. [1,2,3]
In the Python shell type:
```bash
x = ["Lord", "of", "the", "Rings"]
x[2] = "Frodo"
print(x)
```

<details>
<summary>
and it returns:
</summary>
```bash
['Lord', 'of', 'Frodo', 'Rings']
```
</details>


The code above changes element number 2 in x.


## Demo: Dictionaries (5 min)
#### Dictionaries
Dictionaries contain a key and a value. { } enclose dictionaries (Note, that you can also construct a set with curly brackets. The first input in a dictionary pair is the 'key'. The second input in a
dictionary pair is the 'value'. The general format looks like this:
key1:value1

In the Python shell type:
```bash
x = {'key1':'value1', 'key2':'value2'}
```

Now type:
```bash
print(x)
```

These may not be in the exact order in which you typed them. The reason for the different order is because dictionaries have no order. You cannot type x[0] and be referring to 'key1':'value1' . What you do to refer to a value is type the key.

In the Python shell type:
```bash
x['key1'] = 'I love Python'
```

Now type:
```bash
print(x)
```

<details>
<summary>
and it returns:
</summary>
```bash
{'key1': 'I love Python', 'key2': 'value1'}
```
</details>


The keys stay the same but the values are changeable. You can also only have one occurrence of a key in a dictionary, but you may have the values all be the same.

Now type:
```bash
x = {'key':'value1', 'key':'value2'}
```

Then type:
```bash
print(x)
```

<details>
<summary>
and it returns:
</summary>
```bash
{'key': 'value2'}
```
</details>


The first key is overwritten by the second.

Now type:
```bash
x = {'key1':'value', 'key2':'value'}
```

Then type:
```bash
print(x)
```

<details>
<summary>
and it returns:
</summary>
```bash
{'key2': 'value', 'key1': 'value'}
```
</details>

This example shows that you can create two separate keys with the same value.

[Integers, Strings, Tuples, Lists, Dictionaries](https://en.wikiversity.org/wiki/Python/Basic_data_types)


<a name="demo"></a>
## Demo: arithmetic operations and string operations (20 mins)

#### Simple Math
Math is very straightforward in Python. + adds, - subtracts, / divides, and believe it or not * multiplies. The main thing to comment on is %.  % performs a division and then returns the remainder. This is called the modulus operation.
In the Python shell type:
```bash
9 % 3
```

<details>
<summary>
and it returns:
</summary>
```bash
0
```
</details>

Now type:
```bash
9 % 2
```
</details>

<details>
<summary>
and it returns:
</summary>
```bash
1
```
</details>

You can also use variables, and elements and values in simple arithmetic.
In the Python shell type:
```bash
x = 1
y = 5
x + y
```

<details>
<summary>
and it returns:
</summary>
```bash
6
```
</details>

Now type:
```bash
x = [1, 2, 3]
x[1] + x[2]
```
<details>
<summary>
and it returns:
</summary>
```bash
5
```
</details>

This is how you use elements from a list to perform arithmetic operations. It should be clarified that x[0] = 1, x[1] = 2, and x[2] = 3. You can also add and multiply strings, tuples, and lists.

In the Python shell type:
```bash
x = {'a':1, 'b':2}
x['a'] + x['b']
```

<details>
<summary>
and it returns:
</summary>
```bash
3
```
</details>

That is how you do arithmetic with values from a dictionary. Don't forget to use quotations around the keys unless you use integers as the keys. Spend a couple of minutes messing around with this stuff, its fun and it'll help you remember it better. You may also add strings, tuples, and lists.

#### Concatenating
To add two strings together - to do this you just type the first string, an addition sign, the second string.
In the Python shell type:
```bash
"X Files" + " is awesome"
```

<details>
<summary>
and it returns:
</summary>
```bash
'X Files is awesome'
```
</details>

You can do the same with variables referring to strings.
In the Python shell type:
```bash
x = "X Files"
y = " is awesome"
x + y
```

<details>
<summary>
and it returns:
</summary>
```bash
'X Files is awesome'
```
</details>

You can do the same with tuples.
In the Python shell type:
```bash
x = ('I', 'Love')
y = ('True Detective Season 1',)
print(x + y)
```

<details>
<summary>
and it returns:
</summary>
```bash
('I', 'Love', 'True Detective Season 1')
```
</details>

It works the same with lists. What you cannot do is combine two different kinds of types.


#### Multiplying types
Multiplying is very easy and straight forward.
In the Python shell type:
```bash
x = 'the americans '
x * 5
```
<details>
<summary>
and it returns:
</summary>
```bash
'the americans the americans the americans the americans the americans '
```
</details>


Now, try it with a tuple.
In the Python shell type:
```bash
x = ('the americans',)
x * 5
```
<details>
<summary>
and it returns:
</summary>
```bash
('the americans',
 'the americans',
 'the americans',
 'the americans',
 'the americans')
```
</details>

What happens when you try this with dictionaries?

In the Python shell type:
```bash
x = {'the americans':1}
x * 5
```
<details>
<summary>
and it returns:
</summary>
```bash
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: unsupported operand type(s) for *: 'dict' and 'int'
```
</details>

You cannot do the same with dictionaries; that would make multiple keys with the same entry name, which isn't valid in Python.

#### Indexing
You have already learned how to index in lesson 2. When you typed x[3] you were indexing. You may also index a string without first making a variable represent it.
In the Python shell type:
```bash
"I Love Nicktoons"[5]
```
<details>
<summary>
and it returns:
</summary>
```bash
'e'
```
</details>

#### Slicing
Slicing is used to access a range of elements the way that indexing accesses one element.
In the Python shell type:
```bash
x = "Spotify and Netflix are awesome"
print(x[12:32])
```
<details>
<summary>
and it returns:
</summary>
```bash
Netflix are awesome
```
</details>

The numbers that you enter after the variable (the [12:32]) are called indices.


[arithmetic operations and string operations](https://en.wikiversity.org/wiki/Python/Basic_data_types)


<a name="ind-practice"></a>
## Independent Practice: Topic (10 minutes)
Pair up, make up your own statements and see if your partner can tell you what will be returned BEFORE running it.


<a name="conclusion"></a>
## Conclusion (5 mins)
Let's check to see if we know what we learned about today:
- Define what a programming language is
- Differentiate between frontend and backend languages
- Define integers, strings, tuples, lists, and dictionaries
- Demonstrate arithmetic operations and string operations
- Demonstrate variable assignment
