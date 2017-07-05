# Lists

### Basics
 * List is a comma-separated list of values.

 ```python
 primes = [1,3,5,7,11,13,17,19]
 ```

 ### Indexing and Slicing

 ```python
 print primes[0]
 print primes[-1]
 print primes[-8]
 #output
 1
 19
 1

 print primes[1:3]
 print primes[0:]
 print primes[:8]
 print primes[-8:]
 #output:
 [3,5]
 [1,3,5,7,11,13,17,19]
 [1,3,5,7,11,13,17,19]
 [1,3,5,7,11,13,17,19]
 ```

 ### Mutability
  * List is mutable.
```python
zero_to_five = [0,1,2,3,-4,5]
zero_to_five[4] = 4
print zero_to_five
#output:
[0,1,2,3,4,5]

letters = ['a','b','c','d','e']
letters[1:3] = ['B','C']
print letters
#output
['a','B','C','d','e']

letters[:]=[]
print letters
#output
[]
```

### Concatenation/Nesting
```python
letters = []
letters = letters + ['a','b','c']
print letters
#output
['a','b','c']

letters[2]=['c','d']
print letters
#output
['a','b',['c','d']]

print letters[2][0]
#output
c
```