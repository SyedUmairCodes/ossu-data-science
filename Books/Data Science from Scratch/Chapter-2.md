# Basics of Python
> [!CAUTION]
> There’s a lot of information that I didn’t wrote down since I already knew about the basics of Python.

Python is a high-level general purpose programming language that is used in multiple different use-cases and especially for data science and machine learning due to its amazing libraries and frameworks.

Other programming languages use curly braces to delimit blocks of code, Python uses indentation for this. This makes Python code much cleaner but results in unnecessary indentation errors if you're not indenting right.

When something goes wrong in your Python program it results in an error and causes the program to crash. This behavior can be changed by using a except block that tells you the exact error that happened and why it did.

## Virtual Environments

The recommended way to start a new Python project is by creating a virtual environment that allows you to install all of your required frameworks and libraries in a contained environment and you also don't have to mess with the system and global packages.

## Modules

Python comes with the standard library and other libraries and frameworks can be installed depending on the project. These modules won't be available to you by default and in order to use them you'll have to import them into the file you want to access them in.

```python
import re
new_regex = regex.compile("[0-9]+", regex.I)
```

## Testing

Python has multiple different frameworks for testing your code to make sure it performs the way you want it to. A simpler way is to use assert statements or types that are built-into Python.