### 1.3.4 Python doesn’t have much mobile support

In the past decade the numbers and types of mobile devices have exploded, and
smartphones, tablets, phablets, Chromebooks, and more are everywhere, running on
a variety of operating systems. Python isn’t a strong player in this space. While options exist, running Python on mobile devices isn’t always easy, and using Python to write and distribute commercial apps is problematic.

### 1.3.5 Python doesn’t use multiple processors well

Multiple-core processors are everywhere now, producing significant increases in performance in many situations. However, the standard implementation of Python isn’t designed to use multiple cores, due to a feature called the global interpreter lock (GIL). For more information, look for videos of GIL-related talks and posts by David Beazley, Larry Hastings, and others, or visit the GIL page on the Python wiki at https://wiki.python.org/moin/GlobalInterpreterLock. While there are ways to run concurrent processes by using Python, if you need concurrency out of the box, Python may not be for you.

## 1.4 Why learn Python 3?

Python has been around for a number of years and has evolved over that time. The first edition of this book was based on Python 1.5.2, and Python 2.x has been the dominant version for several years. This book is based on Python 3.6 but has also been tested on the alpha version of Python 3.7.

Python 3, originally whimsically dubbed Python 3000, is notable because it’s the first version of Python in the history of the language **to break backward compatibility.**
What this means is that code written for earlier versions of Python probably won’t run on Python 3 without some changes. In earlier versions of Python, for example, the print statement didn’t require parentheses around its arguments:

```Python
print "hello"
```

In Python 3, print is a function and needs the parentheses:

```Python
print("hello")
```

You may be thinking, “Why change details like this if it’s going to break old code?” Because this kind of change is a big step for any language, the core developers of Python thought about this issue carefully. Although the changes in Python 3 break compatibility with older code, those changes are fairly small and for the better; they make the language more consistent, more readable, and less ambiguous. Python 3 isn’t a dramatic rewrite of the language; it’s a well-thought-out evolution. The core developers also took care to provide a strategy and tools to safely and efficiently migrate old code to Python 3, which will be discussed in a later chapter, and the Six and Future libraries are also available to make the transition easier. 

Why learn Python 3? Because it’s the best Python so far. Also, as projects switch to take advantage of its improvements, it will be the dominant Python version for years to come. The porting of libraries to Python 3 has been steady since its introduction, and by now many of the most popular libraries support Python 3. In fact, according to the Python Readiness page (http://py3readiness.org), 319 of the 360 most popular libraries have already been ported to Python 3. If you need a library that hasn’t been converted yet, or if you’re working on an established code base in Python 2, by all means stick with Python 2.x. But if you’re starting to learn Python or starting a project, go with Python 3; it’s not only better, but also the future.

## Summary

- Python is a modern, high-level language with dynamic typing and simple, consistent syntax and semantics.
- Python is multiplatform, highly modular, and suited for both rapid development and large-scale programming.
- It’s reasonably fast and can be easily extended with C or C++ modules for higher speeds.
- Python has built-in advanced features such as persistent object storage, advanced hash tables, expandable class syntax, and universal comparison functions.
- Python includes a wide range of libraries such as numeric processing, image manipulation, user interfaces, and web scripting.
- It’s supported by a dynamic Python community.
  
