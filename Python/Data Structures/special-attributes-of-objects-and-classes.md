# Special attributes of objects and classes
author: catalin

levels:

  - basic

  - advanced

  - medium

type: normal

category: must-know

links:

  - >-
    [docs.python.org](https://docs.python.org/3.5/library/stdtypes.html#special-attributes){website}

  - >-
    [MRO](http://python-history.blogspot.in/2010/06/method-resolution-order.html){website}

---
## Content

Python *objects*/*classes*/*instances* have several more **read-only** attributes, some of which are not reported by the `dir()` function.

Attributes are a way of getting from one object to another.

Suppose we have the class:
```python
class Enki:
    pi = 3.14
```

Get all **writable** attributes of your `object`:
```python
print(Enki.__dict__)
# {... 'pi': 3.14, '__module__': '__main__ }

```
Get the `class`'s class:
```python
print(Enki.__class__)
# <class 'type'>
```
You can also get a `tuple` of base classes of a class object with `class.__bases__`.

Get the name of your `class`/`type`:
```python
print(Enki.__name__)
# Enki

```

To get the **qualified name**, the `class.__qualname__` attribute is available in Python 3.3.

Get all classes considered when looking for **base classes**, i.e. the MRO (Method Resolution Order):
```python
print(Enki.__mro__)
#(<class '__main__.Enki'>, <class 'object'>)
```

---
## Practice

Get all the writable attributes of your object:

```
print(Enki.???) 
```
*`__dict__` 
*`__dict` 
*`dict` 
*`dict__`

---
## Revision

Get the class’s class:

```
print(Enki.???) 
```
*`__class__`
*`__class` 
*`class__` 
*`class`