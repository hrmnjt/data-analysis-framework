# Data Analysis Framework

## What is this?
A light-weight folder structure serving as starting point for data-analysis 
projects in python to helps maintain consistency and code-quality.
This structure inspired from 
[Cookiecutter Data Science](http://drivendata.github.io/cookiecutter-data-science/) 
project while personalizing a few things here and there.


## What this is not?
 * Ideal - this is highly personalised for my use. Please feel free to fork and 
 alter as per your need
 * Finalized - since I'm evolving as I learn stuff, this repo is too!


## Details of what's inside!

### Folder Tree: 
```
+-- data                        # datasets used in project
|   +-- external                # 3rd party data sources that are imported for specific purpose in the project
|   +-- processed               # finalized data sources that are used in analysis
|   +-- raw                     # immutated raw data sources required for the analysis
+-- docs                        # documentation with structure for project
+-- references                  # data dictionaries, manuals and reference documentation
+-- src                         # source files for project
|   +-- scripts                 # finalized scripts (new)
|   +-- archive                 # old versions (archives)
|   +-- work                    # working/raw scripts (WIP)
+-- requirements.txt
+-- LICENCE
```

### Coding Guideline to follow:

It is generally the most wisest and common behaviour to choose Python PEP as 
coding guidelines. For complete reference check 
[PEP8 guidelines](https://www.python.org/dev/peps/pep-0008/)

#### Code Layout

 - Indentation: 4 spaces per indentation level (Not to comment for Holy War,
  I prefer Spaces than Tabs)
 - Max line length: 79 characters
 - Blank lines: 2 for class initialization and seperation of blocks. One line 
 for method definition within a class
 - Imports - On different lines unless from two methods being imported same 
 package
 - Module level dunder names: placed after docstring but before imports

#### Module organisation

The first line of each file shoud be shebang. This makes it 
possible to run the file as a script invoking the interpreter implicitly

Next should be the docstring with a description.

Import built-in modules first, followed by third-party modules, followed by any 
changes to the path and your own modules

Next should be authorship information.
 - Author - Person who writes the code
 - Credits - All who have helped the project (Bug reporting, improvements, etc.)
 - Maintainer - one who is responsible for the code

```
#!/usr/bin/env python3

""" Description of the project

Lorem Ipsum is simply dummy text of the printing and typesetting industry. 
Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, 
when an unknown printer took a galley of type and scrambled it to make a type 
specimen book.
"""

import os
import sys
import my_package
from package_intl import fun1, fun2

__author__ = "Harmanjeet Singh"
__copyright__ = "Copyright (C) 2007 Free Software Foundation"
__credits__ = ["Harmanjeet Singh",]
__license__ = "GPL"
__version__ = "1.0.1"
__maintainer__ = "Harmanjeet Singh"
__email__ = "reachhharman@gmail.com"
__status__ = "Development"

```

#### General recommendations

 - Avoid trailing whitespace anywhere
 - Comments that contradict the code are worse than no comments
 - Use docstrings for classes, methods and program as much as possible
 
---