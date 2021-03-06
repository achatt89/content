# String Formatting
author: tommarshall

levels:

  - beginner

type: normal

inAlgoPool: false

category: must-know

---
## Content

Python uses string formatting in a similar way to the language C to create new and formatted strings. 

The `%` operator formats a set of variables enclosed in a tuple, which is a fixed size list, alongside a format string which holds normal text with special symbols such as `%s` and `%d`, these are known as *argument specifiers`

These are the argument specifiers:
- `%s` is for a String
- `%d` is for Integers
- `%f` is for Floats

For instance, say you have a variable with a string inside it, this is how you print that string:

```python
app = 'Enki'
print 'Learning Python with %s' % app
```
This gives the following output:
```python
# Learning Python with Enki
```

To use two or more argument specifiers you must use a tuple:

```python
app = 'Enki'
streak = 3

print "This is Python workout number %d \
       with %s" % (app, streak)
```

---
## Practice

Complete the code snippet to print the variable ‘str’ to the console:

```
str = ‘practice’
print (‘The best way to learn is to ???’ 
        ??? str)
```
*`%s` 
*`%` 
*`%d` 
*`%f` 
*`+` 
*`/`

---
## Revision

When you want to use two or more argument specifiers, what must you use in order to print them? ???

*A tuple
*A function
*A string