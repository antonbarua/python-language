# Strings

### Basics
* There is no separate 'Character' type. A character is a string of size one.

* Strings are immutable.

```python
s = 'String'
s[0] = 'a' # not allowed!
```

* Both single and double quotes can be used to enclose strings.

```python

s = 'String'
s = "String"
```

### Raw Strings
* \ is for escape sequences.

```python
s = 'C:\new\none'
print s
#output:
C:
ew
one 
```

* r is used for "raw" strings.
```python
s = r'C:\new\none'
print s
#output:
# C:\new\none
```

### Unicode

* u is used for Unicode.

```python
str = u'abc'
```
### Concatenation

```python
s = 'Py' 'thon'
print s
#output:
Python

s = 'Py' + 'thon'
print s
#output:
Python

s = 2 * 'Py' + 'thon'
print s
#output:
PyPython
```

### Index/Subscript & Slicing
```python
# Index

word = 'Python'
print word[0]
print word[5]
print word[-1]
print word[-6]
#output:
P
n
n
P

#Easy-to-remember diagram:
 +----+----+----+----+----+----+
 | P  | y  | t  | h  | o  | n  |
 +----+----+----+----+----+----+
 0    1    2    3    4    5    6
-6   -5   -4   -3   -2   -1     

# Slicing

# print word[a:b] --> print from a to b excluding word[b]

print word[0:2]
print word[2:5]
#output:
Py
tho

print word[0:]
print word[:5]
#output
Python
Pytho

print word[:3] + [3:]
#output:
Python
```


