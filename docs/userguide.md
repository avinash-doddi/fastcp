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
