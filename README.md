# Introduction to Python Programming

**Dr J Rogel-Salazar**

### LEARNING OBJECTIVES

*After this session, you will be able to:*

- Discuss the history of Python and its use across different industries.
- Define how Python compares to other programming languages.
- Describe the benefits of a Python workflow when working with data.
- Demonstrate basic Python programming fundamentals to solve real world problems.
- Create a custom learning plan to help you continue to build fundamental python skills after this workshop.

### STUDENT PRE-WORK

*Before this lesson, you should already be able to:*

- Bring a laptop with [Anaconda](https://www.continuum.io/downloads) using [Python 3.x](https://www.python.org/downloads/) installed. Note: Make sure to choose the *Python 3.x* version for your operating system. 
- If you are using a PC, also install [git-bash terminal](https://git-for-windows.github.io).
- *Optional*: Install a text editor like [Sublime Text 3](http://www.sublimetext.com) or [Atom](https://atom.io) on your computer. If you are using Anaconda, **Spyder** is included in the distribution.

### SESSION AGENDA

| Number | TYPE                                   | TOPIC                                            |
| :----: | -------------------------------------- | ------------------------------------------------ |
|   1    | [Opening](#opening)                    | Greetings                                        |
|   2    | [Introduction](#intro1)                | Why Python? What Can Python Do For Me?           |
|   3    | [Workflow](#workflow)                  | Implementing Python into your Workflow           |
|   4    | [Guided Practice](#guided-practice1)   | Installing & Configuring Common Python Libraries |
|   5    | [Independent Practice](#ind-practice1) | Applying Python Pseudocode to Sample Data        |
|   6    | BREAK                                  |                                                  |
|   7    | [Introduction](#intro2)                | Python Programming Fundamentals                  |
|   8    | [Programming](#progs)                  | Writing Programs in Python                       |
|   9    | [Guided Practice](#guided-practice2)   | Dive into Data with Python                       |
|   10   | [Independent Practice](#ind-practice2) | More Python Practice                             |
|   11   | [Conclusion](#conclusion)              | Review + Recap                                   |
|   12   | [Takeaways](#takeaway)                 | Learning Plan + Q&A                              |

---

<a name="opening"></a>

## Opening

#### Introduce Yourselves

Before we dive in, a bit about you!


#### Our Expectations

- You're ready to take charge of your learning experience.
- You've installed Anaconda & Python 3.x
- You're interested in learning about Python!

#### Our Objectives

What we’ll cover:

* Why Python & What can Python do for me?
* Implementing Python into your workflow
* Python Libraries
* Programming (pseudocode and Python)
* Dive into data with Python

Why this topic matters:

* Programming is a sought-after skill 
* Python has been gaining popularity (why will se why!)  
  Why this topic rocks:

* Python opens up a door to a variety of opportunities, from data science to research in cosmology 

***

<a name="intro1"></a>

## Introduction: Why Python? What Can Python Do For Me? 

**What is Python?**

- Created by Guido Van Rossum in 1991
- Emphasises **productivity** and code **readability**
  * The language is easy to pick up and learn
  * This gentle learning curve brings makes it easier for many to contribute to production level code
  * Readable code means that almost anyone can pick up a piece of code and understand what it is doing
- Interpreted, object-oriented, high-level programming language with dynamic semantics
  * **Interpreted**: Code implementations execute instructions without having to *compile* them into machine-language instruction. In contrast, compiled code is executed by the computer's CPU (hardware)
    * Interpreted code may run less quickly, but can be executed on multiple platforms without modification
  * **Object-oriented** (OO): Instead of concentrating on isolated "actions", object-orientation enables us to focus on "objects" that contain data (attributes). Objects have specific procedures, known as methods (code) that can access and modify the attributes of the object.
    * OO makes it easier to reuse code in other programs
  * **High-level programming**: Related to the code readability mentioned earlier
    * The use of language similar to natural language makes it easy to use and automate
  * **Dynamic semantics**: Once data has been specified, the machine must be instructed to perform operations on the data. Dynamic semantics (also known as execution semantics)  defines how and when the various constructs of a language should produce a program behaviour, providing flexibility at run-time.

**Why Python?**

* Python is extremely fun to develop in.
* Everything can be done with Python.
* If something can't be done, you can create an extension for it.
* Everything can not only be done, but it can be done fast. For example a program that takes you weeks in C++ might take you a day in Python.
* Great for prototyping, and even for usage in a commercial setting.
* Because it is a modern, elegant, highest level OO language.
* Because it is highly expressive, i.e., you will earn higher productivity.
* Because it comes with "batteries included" i.e. libraries for whatever you want.
* Because it is well documented and has a well-established and growing community.

***

<a name="workflow"></a>

##  Implementing Python into Your Workflow

**Where is Python used?**


* Everywhere! Both in industry and Academia
* Art Middleware – Tools and Plugins
* Research
* Web Development and Web Applications
* Game Development
* Windows Applications
* You name it!

### Examples:

* Industry
  - [Drug discovery](https://www.python.org/about/success/astra/)
  - [Financial services](https://www.python.org/about/success/resolver/)
  - [Films and special effects](https://www.python.org/about/success/ilm/)
* Academia
  - [Gravitational waves](https://software.intel.com/en-us/blogs/2016/02/14/python-brings-us-the-ligo-gravity-wave-sound)
  - [Scientific visualisation](https://www.python.org/about/success/mayavi/)
  - [Biomolecule simulation](https://www.python.org/about/success/mmtk/)

Examples to be presented can be drawn from your own experience with the language. If you need inspiration, there are plenty of examples in [this page](https://www.python.org/about/success/)

**Python v other languages**

[Comparing Python to Other Languages](https://www.python.org/doc/essays/comparisons/)

Python is often compared to other interpreted languages such as Java, JavaScript, Perl, Tcl, or Smalltalk. Comparisons to C++, Common Lisp and Scheme can also be enlightening.

#### EXAMPLE

Let us what a Python program looks like, starting with the typical "Hello World!" program: In essence we are writing code to print the message "Hello World!" in the screen.

- **Python**

```python
print("hello world")
```

- **C++**

```c++
#include<iostream>
using namespace std;

int main()
{
	cout << "Hello World!";
	return 0;
}

```

The Python version of this program is very simple: one line of code that will `print` the string `'Hello World!`.  It is easy to read and understand.

The C++ version does exactly the same, but it requires us to write more information. For example we need to define a `main` function, we have to be careful with the use of punctuation (notice the semicolons at the end of some of the lines) and `cout` is not very understandable in plain terms.

Let us see the same program in Java:

- **Java**

```java
public class HelloWorld
{
    public static void main (String[] args)
    {
        System.out.println("Hello, world!");
    }
}
```

Notice that in the Java version we define the code inside the context of class.

In Object Oriented Programming a *class* is a template definition of the methods and variables in a particular kind of object. In other words, an object is a specific instance of a class: it contains actual values instead of variables.

#### Python interactive shell v scripts

In the example shown above, we are assuming that we are using an interactive shell, i.e. we are writing code that is executed immediately by the Python interpreter and we are able to "interact" with the results of the commands we pass. We can do this via:

- python shell: Look and feel similar to a terminal shell. This can be launched with:

```
> python
```

- ipython shell: Look and feel is more interesting than a plain terminal, providing syntax colouring and shortcuts to interact with our code. This can be launched with:

```
> ipython
```

- jupyter notebook: Uses a web interface that let's us use formatting along side our code and we highly recommend using it. This can be launched with:

```
> jupyter notebook
```

Alternatively, there may be instances where we do not need to interact with our Python code. Instead we may want to execute a program, in bach mode for instance, and simply get the results at the end of the execution.

In those cases we need to create a Python script. We can use any plain text editor of our choice and save the code in a file with extension `.py`.

Plain text, as you might have guessed, is rather plain. It supports standard ASCII characters, including numbers, symbols, and spaces, but does not support any type of text formatting. Therefore you cannot apply bold, italic, or underlined styles, and you cannot use different fonts or font sizes in a plain text document.

Some common plain text editors include Atom, NotePad (Win), TextEdit (Mac), Nano (Linux, Mac), NotePad++ (Win) or TextWrangler (Mac).

An alternative to using plain text editors is the use of an integrated development environment (IDE), which  provides comprehensive facilities to computer programmers for software development. A good IDE consists of a source code editor, build automation tools and a debugger as well as intelligent code completion.

Common Python IDEs:

- [PyCharm](https://www.jetbrains.com/pycharm/)
- Eclipse with [PyDev](http://www.pydev.org)
- [Atom](https://atom.io)
- Anaconda distributions (Mac, Win, Linux) come with an IDE called `Spyder`.

A barebones script for the "Hello World!" program (saved to a file called `hi.py`) looks like this:

```python
print("Hello world!")
```

To run the script by passing it as a command to the Python interpreter we need to write:

```python
> python hi.py
```

Please note that all of the code that is at indentation level 0 gets executed. Functions and classes that are defined but not on at the 0-th level indentation are not executed.

Unlike other languages, there's no `main()` function that gets run automatically - the `main()` function is implicitly all the code at the top level.

In this case, the top-level code is an if block.  `__name__` is a built-in variable which evaluates to the name of the current module. We can test whether our script is being run directly or being imported by something else by testing

```python
if __name__ == "__main__":
    ...
```

A more sophisticated version of the "Hello World!" script is therefore:

```python
def main():
	print("hello world")

if __name__ == '__main__':
    main()
```

### Packages

Libraries of code written to solve particular set of problems

In Python there are many related packages relevant to data science: pandas, Scikit-learn, NumPy, etc

These are installed with PIP, Conda, etc. For example we can use:

`pip install <package-name>`

We saw how this was used in the demo section (see above) to install `plotly`

Other packages that are widely used:

* pandas
  * Ever used Excel? How do yo fancy working with data structured in a similar way, but without the irritation of formatting, long formulae and better graphics. Well, use *pandas*
* SciPy/NumPy
  * Does your application require the use of advanced mathematical functions or numerical operations with arrays, vectors or matrices? Try *SciPy* (scientific python) and *NumPy* (numerical python)
* Scikit-Learn
  * Are you interested in using python in a data science workflow and exploit the use of machine learning in your applications? Look no further than *Scikit-learn*
* matplotlib
  * Are you tired of the boring-looking charts produced with Excel? Are you bored of looking for the write menu to move a label in your plot? Take a look at the visuals offered by *matplotlib* 	
* statsmodels: statistical tests
  * Is your boss asking about significance testing and confidence intervals? Are you interested in descriptive statistics, statistical tests, plotting functions, and result statistics? Well *statsmodels* offers you that and more.
* Beautiful Soup
  * All the data you require is available freely on the web but there is no download button and *You* need to scrape the website? You can  extract data from HTML using *Beautiful soup*

### Importing a module

```python
import math
x = math.cos(2 * math.pi)
print(x)

from math import *

log(10)

log(10,2)
```

### Types, Variables, assignment

```python
# variable assignments
x = 1.0
my_variable = 12.2
type(x)

y = 1
type(y)

b1 = True
type(b1)

s = "String"
type(s)
```

```python
import types
print(dir(types))

1+2, 1-2, 1*2, 1/2

1.0+2.0, 1.0-2.0, 1.0*2.0, 1.0/2.0

# Comment

# Comparison: >, <, <=, <=, ==
2 > 1

# Testing for equality
2 == 2
```

**Lists**

```python
l = [1,2,3,4]
print(type(l))
print(l)
print(l)
print(l[1:3])
print(l[::2])

# Python starts counting from 0
print(l[0])
```

**Tuples**

```python
point = (10, 20)
print(point, type(point))

x, y = point
print("x =", x)
print("y =", y)
```

**Dictionaries**

```python
params = {"parameter1" : 1.0, "parameter2" : 2.0,
"parameter3" : 3.0,}
print(type(params))
print(params)
```

***

<a name="ind-practice1"></a>

## Independent Practice: Applying Python Pseudo-code to Sample Data

Pseudocode is a language very close to English that allows us to represent a program concisely. The only thing you need is a statement to show where you are starting and where you are ending a program.

> Instructor Note: Run through the following example with the students. Then ask them to tackle problems similar to the ones proposed below.

Calculate and print the average of three numbers: 5, 10, and 15.

```
Start
	num1 = 5
	num2 = 10
	num3 = 15
	sum = num1 + num2 + num3
	average = sum/3.0
	print average
End
```

### Proposed problems:

1. Create a complete programme that will calculate the area circle with radius r.
2. Calculate and print the square of a number. If the number is larger than 10 also calculate the cube.
3. List the letters in the sentence "Python is awesome"

<a name="intro2"></a>
## Introduction: Python Programming Fundamentals

Understanding core programming concepts and why they are used is just as important as knowing how to write code. 

Before we start, let us review some basic concepts of any programming language:

- **Variables**: A variable is a storage location and an associated symbolic name which contains some known or unknown quantity or information, a value. Variables can be of different `types`
  - `r = 3` 

- **Control Structures**: A control structure is a block of programming that analyses variables and chooses a direction in which to go based on given parameters. The term flow control details the direction the program takes (which way program control “flows”). Hence it is the basic decision-making process in computing; flow control determines how a computer will respond when given certain conditions and parameters. Some typical structures include
  - If statement
  - For loop
  - Functions 

- **Data Structures**: Data structure is a particular way of storing and organising data in a computer so that it can be used efficiently. Some examples include:
  - Lists
  - Tuples
  - Arrays
  - Matrices
  - Dataframes

- **Syntax**: the syntax of a programming language is the set of rules that define the combinations of symbols that are considered to be correctly structured programs in that language

The interrelationship of these elements make it possible for us to write programs to implement algorithms and solve problems


### Control Flow

* The term flow control details the direction the program takes (which way program control “flows”). 

* It determines how a computer will respond when given certain conditions and parameters.

#### **If**

An `if` statement is a conditional structure that, if proved true, performs a function or displays information. 

Think of this as a decision that moves the flow of your program depending on the answer to a TRUE-FALSE question. 

```
IF a person is older than 18
THEN they can drive
ELSE they cannot drive

```
We can express the pseudo-code above into Python as follows:

```python
if age_person > 18:
	return "They can drive"
else:
	return "They cannot drive"	
```

Let us see another example:

```python
A = 10
B = 100
if A>B:
	print("A is larger than B")
elif A==B:
	print("A is equal to B")
else:
	print("A is smaller than B")
```

#### **For loop**

A loop statement in programming performs a predefined set of instructions or tasks while or until a predetermined condition is met. 

Think of this as a repetitive action that has to be performed until further notice. 

```
FOR each user of a service in a list
   PRINT greet them
```

In the pseudo-code above, the condition we are asked to greet each user in a list. We stop the repetition when we reach the end of the list. 

We can express this loop in Python as follows:

```python
users = ["Jeff", "Jay", "Theresa"]

for user in users:
    print("Hello %s" % user)
```

**Tip**: When creating a for loop, make sure it's condition will always be met to help prevent an endless loop.

Let us see another example. Can you explain what the program is doing?

```python
for x in [1,2,3]:
    print(x)

for key, value in params.items():
    print(key + " = " + str(value))
```

##### List comprehension

List comprehension is an elegant way to define and create list in Python. It uses a for loop inside the definition of the list itself.

Let us take a look at one, and see if you can figure out what is happening:

```python
l1 = [x**2 for x in range(0,5)]
```

#### **Functions**

A function is a group of instructions, also known as a named procedure, used by programming languages to return a single result or a set of results. 

Functions are a convenient way to divide our code into useful blocks, providing us with order, making the code more readable and reusable.

Functions are a key way to define interfaces so programmers can share their code.

Here is how you define a function in python

```python
def function_name(input1, input2...): 
    1st block of instructions 
    2nd block of instructions
    ...
```

Let us define a function that returns the square of the input value:

```python
def square(x):
	"""
	Return the square of x.
	"""
	return x ** 2
```

We can call this function as follows:

```python
var1 = 7

var2 = square(var1)

print(var2)
```

***

<a name="progs"></a>

## Programming: Writing Programs in Python (15 mins)

Python is an *interpreted* language, which means you can run the program as soon as you make changes to the file. This makes iterating, revising, and troubleshooting programs is much quicker than many other languages.

You can now translate into Python the pseudo-code created in [the Independent Practice ](#ind-practice1) above.

***

<a name="guided-practice2"></a>

## Guided Practice: Dive into Data with Python (20 mins)

Let us create a new Jupyter notebook for this practice. We will work in pairs.

1. Save the file called [Python101_Part2_GuidedPractice.ipynb](./code/Python101_Part2_GuidedPractice.ipynb) in a known location in your file system
2. Start Jupyter and navigate to the location where you saved the file
3. Open the file 
4. Voilà, you can start the Guided Practice

***

<a name="ind-practice2"></a>

## Independent Practice: More Python Practice (20 mins)

### DISCUSION

Given your interests and knowledge, which are you more interested in learning about:

- practical applications of python, or
- python fundamentals?

> 
>
> OPTION 1
>
> You can use the [Iris Dataset notebook included in the materials](./code/Python101_Part2_IndPractice.ipynb) to follow up the introduction to pandas in the previous section. Note that the notebook makes reference to the [Iris Dataset included here](./code/data/iris.csv).
>

***

<a name="conclusion"></a>

## Conclusion: Review + Recap Topics

### Class discussion

In the session you have covered the following topics:

* Discuss the history of Python and its use across different industries.
* Compare Python with programming languages.
* The benefits of a Python workflow
* Python programming fundamentals.
* Use Python code to solve real world data problems.

***

<a name="takeaway"></a>

## Takeways: Learning Plan + Q&A 

#### What Should You Do Next?



We suggest some resources such as books, podcasts, GA courses, etc.

* For beginner programmers:
  * go through [Learn Python the hard way](http://learnpythonthehardway.org)
  * read up on and familiarise yourself with the language by going through the tutorials [A Beginner's Python Tutorial](https://en.wikibooks.org/wiki/A_Beginner's_Python_Tutorial)

* For programmers new to python
  *  Read the information in [Moving to Python From Other Languages](https://wiki.python.org/moin/MovingToPythonFromOtherLanguages)
  *  [Python for java developers](https://antrix.net/static/pages/python-for-java/online/)
  *  [Python for MATLAB users](http://bastibe.de/2013-01-20-a-python-primer-for-matlab-users.html)

* For more seasoned programmers:
  * Challenge yourself by tackling the [Python Challenge](http://www.pythonchallenge.com) 


> 

***

## ADDITIONAL RESOURCES

- [Python success stories](https://www.python.org/about/success/)
- [Learn Python the hard way](http://learnpythonthehardway.org)
- [Beginners' Guide to Python](https://wiki.python.org/moin/BeginnersGuide)
-  [10 Minutes to Pandas](http://pandas.pydata.org/pandas-docs/stable/10min.html)

