# Fast Cp
A Python Library that contains various functions to make Competitive Programming easy. 
This Package includes pre-defined functions that are quite useful in Competitive Programming.
+ To View the Package -> [Click Here](https://pypi.org/project/fastcp/)
+ To View Documentation Web Page -> [Click Here](https://avinash-doddi.github.io/fastcp/)

### Purpose of Package
+ The main purpose of this package is to provide various functions that are helpful for Competitive Programming.

### Features
+ Collections of fastcp
    + Collections of arrays
        - Unique
        - Subarr
        - Subseq
        - Freq
        - Length
    + Collections of strings
        - VowelCount
        - Freq
        - Substr
        - Subseq
    + Collections of bitMan
        - Binary
        - Hexa
        - Octal
        - Toggle
        - CountSetBits
        - BinToDecimal
        - OctToDecimal
        - HexToDecimal
    + Collections of math
        - Product
        - Sieve
        - IsPrime
        + Along with all functions in python 3.11.0 [math](https://docs.python.org/3/library/math.html) library
    + Collections of search
        - Find
        - LowerBound
        - UpperBound
    + Collections of sorting
        - Sort
        - SortDict
        - SortDictValues
    + Collections of collections
        - MultMap
        + Along with all functions in python 3.11.0 [collections](https://docs.python.org/3/library/collections.html) library
    + Collections of trees
        - Create
        - Inorder
        - Preorder
        - Postorder
        - Levelorder
        - Search
        - NodeSum

### Getting Started
This package can be found on PyPi. Hence you can install it using pip

### Installation
```bash
pip install fastcp
```

### Usage

importing all sub-packages from fastcp
```python

>>> from fastcp import *
>>> subsequences = Subseq([1,2,3,4,5])

importing a single sub-package from fastcp

>>> from fastcp import bitMan
>>> toggled_number = bitMan.Toggle(123)
```

### Examples

```python

>>> from fastcp import arrays

>>> arrays.Freq([1,1,2,2,2,3])
{1:2, 2:3, 3:1}
```

```python
>>> from fastcp import *

>>> Substr("python")
['python', 'ython', 'thon', 'hon', 'on', 'n']

>>> Subseq("Pypi")
['Pypi', 'Pyp', 'Pyi', 'Py', 'Ppi', 'Pp', 'Pi', 'P', 'ypi', 'yp', 'yi', 'y', 'pi', 'p', 'i', '']
```
+ New Libraries: (v.1.0.2)
    + sorting
    + collections

```python

>>> from fastcp import sorting
>>> # Sort function at O(N) Complexity

>>> dict = {10: 1, 8: 2, 1: 3, 4: 4}

>>> print(sorting.SortDict(dict))
{1: 3, 4: 4, 8: 2, 10: 1}

>>> print(sorting.SortDict(dict, True))
{10: 1, 8: 2, 4: 4, 1: 3}


>>> from fastcp import *

>>> d = MultMap(0)
>>> # creates a Multi-Dictionary with default value as Int (0);
>>> d[0][0]
0

>>> d = MultMap([])
>>> # creates a Multi-Dictionary with default value as List ([]);
>>> d[0][0]
[]
>>> d[0][0].append(20)
>>> d[0][0]
[20]
>>> d = defaultdict(int)
>>> d[0]
0

```

```python
>>> from fastcp import trees
>>> root = trees.Create(10)
>>> root.left = Create(5)
>>> root.right = Create(20)
>>> trees.Inorder(root)
[5, 10, 20]
>>> trees.Preorder(root)
[10, 5, 20]
>>> trees.Postorder(root)
[5, 20, 10]
>>> trees.Levelorder(root)
[[10], [5, 20]]
```

### Author
Avinash Doddi [https://github.com/avinash-doddi]
