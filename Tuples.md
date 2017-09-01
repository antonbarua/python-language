# Tuples

### Overview

* Tuple is a sequence data type
* Data in a tuple can be heterogeneous, as opposed to list which can only have homogeneous data
* Tuples are immutable, but can contain mutable data

```python
a = 1, 'a', ['hello', 'world']
print a
# (1, 'a', ['hello','world'])

print a[2]
#['hello','world']

a[1] = 'b'
#Error! immutable

#But can modify mutable objects
a[2][0] = 'hola'
print a[2]

#['hola', 'world']
```

### 0 and 1 element tuples

```python
#0-element
a = ()
print a
#'()'

#1-element
a = 1, #<--trailing comma
print a
#(1,)
```

### Packing and unpacking

```python
a = 1,2,'a' #packing

one, two, aa = a #unpacking
```