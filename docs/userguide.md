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
+ New Library: (v.1.0.6.1)
    + dataStructures

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

``` python

>>> from fastcp import dataStructures as ds 
>>> d = ds.maxHeap()
>>> # creates a maxHeap object (d)
>>> d.put(20)
>>> d.put(50)
>>> d.get()
50 # returns the max value in heap
>>> d.size()
1  # since 50 is removed from heap

>>> s = ds.Stack()
# create a stack data structure
>>> s.push(10)
>>> s.push(20)
>>> s.size()
2
>>> s.pop()
20
>>> s.pop()
10
>>> s.pop()
None

>>> d = ds.minHeap()
>>> # creates a minHeap object (d)
>>> d.put(20)
>>> d.put(50)
>>> d.get()
20 # returns the min value in heap
>>> d.size()
1  # since 20 is removed from heap
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