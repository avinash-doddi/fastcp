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
        - Cbrt
        - Product
        - Sieve
        - IsPrime
    + Collections of search
        - Find
        - LowerBound
        - UpperBound
    + Collections of trees
        - Create
        - Inorder
        - Preorder
        - Postorder
        - Levelorder

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
>>> subsequences = arrays.Subseq([1,2,3,4,5])

importing a single sub-package from fastcp

>>> from fastcp import bitMan
>>> toggled_number = bitMan.Toggle(123)
```

### Examples

```python

>>> from fastcp import arrays

>>> arrays.Freq([1,1,2,2,2,3])
{1:2, 2:3, 3:1}

>>> from fastcp import strings

>>> strings.Substr("python")
['python', 'ython', 'thon', 'hon', 'on', 'n']

>>> strings.Subseq("Pypi")
['Pypi', 'Pyp', 'Pyi', 'Py', 'Ppi', 'Pp', 'Pi', 'P', 'ypi', 'yp', 'yi', 'y', 'pi', 'p', 'i', '']

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
