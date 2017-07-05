# Control Flow

### Basics
 * No ```switch case```

### pass
 * no-op statement
 
### If-elif-else

 ```python
if x == 0:
    print 'zero'
elif x == 1:
    print 'one'
elif x == 2:
    print 'two'
else:
    print 'other'
 ```

### for

* Iterates over items of any sequence (list or string)
* Does not have explicit stop condition or steps like C's for loop

```python
words = ['hello','world','hi']

for word in words:
    print word
 #output:
 hello
 world
 hi
 ```

### range() function

* Generates lists

```python
range(start=0, end, increment)

range(5)
#output:
[0,1,2,3,4]

range(2,5)
#output:
[2,3,4]

range(1,10,2)
#output:
[1,3,5,7,9]

for i in range(5)
    print i
#output:
0 1 2 3 4
```

### for-else

```python
for i in range(5):
    #do something
else:
    #loop exhausted, do something else
```