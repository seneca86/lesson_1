# Lesson 1: Introduction to Python

## Why learn Python?

### Introduction to the class
During Programming 0 and I we have learnt R, which is a programming language with a focus on statistics and data science.

In Programming II we will use Python, which has a broader scope (although it is excellent too for data science). Before jumping into the specifics, let's remember what a programming language consists of.

### Elements of a programming language
A programming language is not that different from other patterns or languages that we encounter in daily life, be it a cooking recipe, a knitting pattern, a board game, a videogame, or a foreign language. Most of them consist of:
- a regular _vocabulary_
- _syntax_ rules
- sequences of _operations_
- repetitions of some operations (_loops_)
- reference to other operations (_functions_)
- assumptions about the _context_
- _data_ to be used, created or modified
- _tools_ to work with the data
- an expected _result_

### Introducing Python
Let's see our first Python program to get a glimpse of its look and feel:
```Python
for day in ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']:
    print(f'{day} is a day of the week')
```

This short loop already conveys some of the properties of Python, such as readability and expressiveness.

Another tiny program follows, that lists the so-called "Five Good Emperors" of the Roman Empire and selects one of them:

```python
emperors = [
    'Nerva',
    'Trajan',
    'Hadrian',
    'Antoninus Pius',
    'Marcus Aurelius',
]
print(emperors[3])
```

Note that we have used a Python structure called `list`, which is defined by enclosing square brackets. The word `emperors` is a _variable_ that provides the list with a name so that we can manipulate it.

Also note that the index `3` returns the fourth element of the list, which means that the first element is accessed via the index `0`. This is a Python convention shared with other programming languages, such as Fortran. You may think of the index as an offset rather than as a position.

A pivotal data structure in Python that we will be back to is the _dictionary_. A dictionary is a collection of unique _keys_ and associated _values_. We can build a dictionary that stores e.g. names of books and its corresponding authors:

```python
books = {
    'Anna Karenina': 'Leo Tolstoy',
    'Meditations': 'Marcus Aurelius',
    'The Prince': 'Machiavelli',
    'Paradise Lost': 'John Milton',
    'At the mountains of Madness': 'H.P. Lovecraft',
}
book = 'At the mountains of Madness'
print(f'{book} was written by {books[book]}'
```

A dictionary is defined with curly brackets and a colon that associates each key with each value. We will get back to dictionaries later in the course.

### Python versus other programming languages
There are various ways to verify the raising popularity of Python, such as:
- It is the fastest-growing major programming language, according to the TIOBE index
- It is the most popular introductory computer science courses at the top US Colleges
- It is the official teaching language for high schools in France

More importantly, there are fundamental reasons to explain this popularity:
- Python is reasable, which makes it easier to learn and remember
- Python is a _dynamic_ language or _scripting_ language, which means that it does not force you to declare variable types before using them
- Python is terse, meaning that programs in Python will me in general shorter than their equivalents in a static language
- Python is _free_, in the sense that you do not have to pay to use it and that you can use it for whatever you wish
- Python has 'batteries included' as commonly expressed, meaning that there is plenty of useful software both in its standard library and in third-party code

However, there are situations in which Python may not be the best option. This occurs when a problem is CPU-bound, in which case a low-level such as C++, C#, or Java may work better.

### Python versions

Python has been around since 1991, created by Guido van Rossum as a successor to the ABC programming language. In 2000, Python 2 was released with a few improvements, and in 2008 it was the turn of Python 3.

Each of these major versions include "hard fixes", which are incompatible _backwards_. Conversion from Python 2 to 3 has been relatively painful but successful, and we will be using Python 3 in the course.

### Ways to run Python
Similarly to R, we will run Python with a combination of an _interactive interpreter_, which we will call "the console", and text files that we will execute. These text files will have the termination ".py".

While using Repl.it or other web-based IDEs we will sometimes need to use the "Shell", which is an interface with the underlying operating system (typically Linux). We will not focus on it since it could cover a course on its own, although we will occasionally comment on it. In the Shell, we can type "python" and access a primitive version of the interactive interpreter that we have in the console.

The Console works in a way such as it reads, evaluates, and prints in loops. This type of interface is for that reason called "REPL", and the reason behind the name of repl.it.

