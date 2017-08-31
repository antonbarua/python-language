# Modules

### Overview

* A module is a file containing Python definitions and statements.
* A module's name is available through the ``__name__`` variable.
* A module can be used by a script using the ``import`` statement.
* A module can contain executable statements and function definitions.
* The statements are only executed when the module is first imported via ``import`` statement.

```python
#moduleA.py
print __name__

def print_str(str):
    print str

#script.py
import moduleA

moduleA.print_str('hello')

##output
moduleA
hello
```

### Module symbols
* Each module has its own symbol table.
* Using ``from module import a`` you can import specific names from a module.
* ``from module import *`` imports all names except the ones beginning with an underscore.

### Execute module as a script

```python
if __name__=='__main__':
    #execute some code

# python <module.py>
```

### The dir() function
* ``dir(module)`` lists the names defined in a module
* ``dir()`` lists the names defined in the current module

### Packages

* For grouping a collection of modules

```python
#sample package hierarchy

packageA/
    __init__.py
    packageB/
        __init__.py
        moduleB.py

#usage

import packageA.packageB.moduleB
or
from packageA.packageB import moduleB

moduleB.func()
```