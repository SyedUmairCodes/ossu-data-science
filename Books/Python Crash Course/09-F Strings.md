Everything between two double or single quotes will be considered as a string in python but if we want to make our string dynamic we can insert a variable into our string so the value of the variable will become a part of our string.

This is done using format strings or `f-strings` for short, f strings allow us to insert variables inside strings.

```python
name = Harry
message = print(f"Hello, {name}")
```

F-strings can be used in multiple places where you need to update a part of a string such as welcoming the user after they login or display the number of active users on a website.