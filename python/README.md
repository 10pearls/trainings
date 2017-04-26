# Python 

[![N|Solid](https://www.python.org/static/community_logos/python-logo-master-v3-TM.png)]()

## Table of Contents
1. [Introduction](#introduction)
1. [Installation Guide](#introduction-guide)
1. [Zen of Python](#zen-of-python)
1. [Comments](#comments)
1. [Variable , Expressions and Statements](#variable-expressions-statements)
1. [Data Structures](#data-structures)
1. [Functions](#functions)
1. [Module](#module)
1. [Namespace and Scoping Rules](#namespace)
1. [Packaging](#packaging)
1. [Classes](#classes)

## Introduction
This guide is a quick introduction to the Python language. 
Python is a general purpose programming language, that’s used by thousands of people to do things from testing microchips at Intel, to powering Instagram, to building video games. 
It’s small, very closely resembles the English language, and has hundreds of existing third-party libraries.

## Installation Guide
For setting up Python3 on your machine in just few baby steps, 
  -  **[Ubuntu][DigitalOcean]** users
  -  **[Windows][DigitalOceanWin]** users 
  -  **[Mac][DigitalOceanMac]** users 

Some poiters as you're performing installation:
  - We'll be working on Python3. However, if desired you can switch to Python2, which will take        minimal change of lines.
  - The guide also covers a basic **Hello World program**.
  - Perks of running your code/app in a **Virtual Environment**:
  
    -   It isolates your app specific settings from the base python packages.
    -   Only install packages that are required; meaning zero pollution.
    -   Will make your life merrier when building Web Applications. Trust me!

Having trouble in setting up Python [refer FAQ's section](FAQ.md)  

## Zen of Python 
Before we buckle down lets look at the philosophy behind Python as illustrated by long time Pythoneer Tim Peter.
[Link][zen]

## Comments
Yes, your code does need comments, else things go haywire
 - [Single Line][comment1]
 - [Muti Line][comment2]

## Variable , Expressions and Statements
Python is both a **strongly typed** and **dynamic** language. In essence, it's our responsibility to test variable types and correct usage. 
Refer this [link][variable] to learn more about declaring variables.

## Data Structure
In python builtin data structures are list, dict, tuples, sets, strings. 
I don't expect you to learn all the methods associated with each structure, however, a basic idea of how to utilize each structure is important.
[Read here][DataStructures]

## Functions
It's here that Python's magic starts. We can set default arguments for our functions, have lambda functions come into play. And yes multiple returns do exist.
Refer below links for an in-depth view.

  - [Functions][Functions]
  - [Repeating Events][RepeatingEvents]
  - [Decorators][Decorators]
  
There are exercises in classroom for this section.

## Module
The quintessence of modular approach is to break code for re-usability. More [here][Module]
 
## Namespace and Scoping Rules
Only 3 namespaces are visible to the developer: local, global, built-in. Refer to [this][Namespace] article for more info.


## Packaging
Simply put, any directory containing init file is a package. [Learn][Packaging] more


## Classes
Finally, now we know enough to tacke [OOP concepts in Python][OOP] 
There are exercises in classroom for this section.
  
## Python Holy Book - PEP 8
Everything in Python follows a pre-defined guidelines and conventions know as **[PEP 8][pep8]**. It's essential that you refer to it moving forward.

## Whats Next? (Optional)
We have pretty much covered the basics of Python programming.

Feeling brave enough? Lets **Tango with Django!!**
 - [Hello World][Hello World] 
 - [Django Docs][Docs] 
 - [DRF][DRF] (Django Restful Framework)



[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

[DigitalOcean]: <https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-local-programming-environment-on-ubuntu-16-04>
[inst1]: <http://stackoverflow.com/questions/3701646/how-to-add-to-the-pythonpath-in-windows-7/4855685#4855685>
[inst2]: <http://stackoverflow.com/questions/3387695/add-to-python-path-mac-os-x/3387737#3387737>
[pep8]: <https://www.python.org/dev/peps/pep-0008/>
[comment1]: <https://www.codecademy.com/en/courses/introduction-to-python-6WeG3/2/1?curriculum_id=4f89dab3d788890003000096>
[comment2]: <https://www.codecademy.com/en/courses/introduction-to-python-6WeG3/2/2?curriculum_id=4f89dab3d788890003000096>
[variable]: <http://www.thomas-cokelaer.info/tutorials/python/variables.html>
[DataStructures]: <http://www.thomas-cokelaer.info/tutorials/python/data_structures.html>
[Functions]: <http://www.thomas-cokelaer.info/tutorials/python/functions.html>
[RepeatingEvents]: <https://mva.microsoft.com/en-us/training-courses/introduction-to-programming-with-python-8360?l=KcYcW0Fz_304984382>
[Module]: <http://www.thomas-cokelaer.info/tutorials/python/module.html>
[Namespace]: <http://www.thomas-cokelaer.info/tutorials/python/namespace.html>
[Packaging]: <http://www.thomas-cokelaer.info/tutorials/python/packaging.html>
[zen]: <https://www.python.org/dev/peps/pep-0020/>
[OOP]: <http://www.thomas-cokelaer.info/tutorials/python/classes.html>
[DigitalOceanWin]: <https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-local-programming-environment-on-windows-10>
[Decorators]: <http://www.thomas-cokelaer.info/tutorials/python/decorators.html>
[Hello World]: <https://github.com/django-ve/helloworld>
[Docs]: <https://docs.djangoproject.com/en/1.11/>
[DRF]: <http://www.django-rest-framework.org/>
[DigitalOceanMac]: <https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-local-programming-environment-on-macos>