# Essential Libraries For Science

A core part of programming is having a vague understanding of what exists
out there in terms of functionality, tools, libraries, … You do not need to
know how to do a task, but that this task is possible using this or that
library. In this chapter, we provide a somewhat opiniated list of tools and
libraries that you should know about when writing code for science. We will
not teach _how_ to use those libraries, as there are plenty of
available resources for that. Instead, we only provide a short
introduction of what those libraries _do_.

We have divided the list of libraries into 5 categories: (1) core libraries,
ie libraries that you cannot code for science without; (2) libraries and tools
you should not work without; (3) visualizationg and plotting libraries; (4)
things that will help you speed up your code; (5) domain specific libraries.

## Core libraries: numpy, scipy, pandas.

About 95% of scientific Python code starts with the following lines:

```python
import numpy as np
from scipy import XXX
```

- **`numpy`**'s core functionality is to provide an easy-to-use and efficient
  n-dimensional array data structure called `ndarray`. Any numerical analysis
  code in Python heavily relies on the `ndarray` data structure. The main
  difference with Python's list is that arrays are almost always homogeneously
  typed (all elements of the array are of the same type). `numpy` also
  provides fast and easy operations such as sum, element-wise product, matrix
  product, indexing, slicing, broadcasting, … Note that we have a full chapter
  on how to use `numpy` (see {doc}`numpy` for details)!

- **`scipy`** is the core toolbox for scientific and technical computing for
  Python. It contains many submodules, some related to complex data structures
  (for sparse matrices for example) or operations on `ndarray` (linear
  algebra, fourier transforms, IO), others domain specific (signal processing,
  image processing, clustering). View `scipy` as the Swiss army knife of
  scientific computing in Python.

- **`pandas`** is a software library for the manipulation of data frames (an
  object to store tabular data, as you might find in Excel or relational
  databases). This differs from NumPy arrays in being 'column-oriented': the
  values in each column have to be of the same type, but one row can contain
  many different types of objects." Just as NumPy does for arrays,
  `pandas` provides fast and easy operations on dataframes, such as pivoting,
  merging, joining, data filtering, column-wise operations. We also have a
  full chapter on how to use `pandas` (see {doc}`pandas` for details)!

## "Things you cannot (or should not) work without"

- A good text editor or an IDE (See {doc}`editors-and-ides` for details)!

- `ipython` is a command shell for Python. Think `python`, but a hundred times
  better! It has syntax highlighting, auto-completion, and many magic
  functions (`%debug`, `%run`, etc) to ease the process of programming, data
  exploration, and debugging.

- `pdb`, `ipdb`, `pdb++`, and `pudb` are four python debuggers. Knowing how to use a
  Python debugger is a must! If you don't know how to use one, read
  {doc}`debugging`) without further delay!


- Whether you use an IDE or a text editor, configure it with a static linter
  to check your code as you write it. There are different options available. A
  widely used static linter is `flake8`: it combines three tools into one
  (`pyflakes`, `pycodestyle`, and `mccabe`). Another popular one is `pylint`.


## Visualization libraries

- `Matplotlib` is the most widely used visualization library in Python. While
  the API takes a while to get used to, there is nothing better to create high
  quality scientific figures for publication! Literally everything can be
  tweaked, tuned, and modified.

- `seaborn` is a thin layer on top of Matplotlib: you get the flexibility of
  Matplotlib with an easy-to-use interface.

- `bokeh` 

- plotly

- Altair

## Speed ups

- profilers
- cython
- numba
- joblib
- dask

## Domain specific

- statsmodel
- scikit-learn
- tensorflow
- scikit-image
- networkx
- biopython

# Developping packages

- unit tests
- documentation
