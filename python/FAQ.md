### Installation FAQ's:
Frequently Asked Questions (FAQ) about the setting up Python
##### I installed Python but cannot execute it.

If the installation process went smooth, but when you call python you get an error that might mean Python has not been added to your computer path, therefore your computer is not being able to find the python  command. If you are on Windows, please follow [these instructions][inst1].
##### I have Python 2 already. Should I install Python 3 instead?

The course covers Python 3, and it's recommended that you install and use Python 3 as Python 2 will not be supported anymore by 2020. Simply install Python 3 and then you can use it as:
```sh
python3 myprogram.py 
```
Mac and Linux users, if your computer has Python 2 by default, don't uninstall it as it may harm your operating system. Simply install Python 3 and leave Python 2 as it is and use Python 3 as shown above.

##### pip is not working. What should I do?
Try:
```sh
python -m pip install package_name 
```

##### I can install packages with pip, but I cannot import them in Python.
That could mean you have two Python installations in your computer. For example, you are installing packages for your Python 2 and trying to import them in your Python 3. To install packages for Python 3 you will have to do:
```sh
pip3 install package_name 
```
Then you should be able to import it in Python 3. Note that if have only Python 3, you would write pip instead of pip3.

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

[inst1]: <http://stackoverflow.com/questions/3701646/how-to-add-to-the-pythonpath-in-windows-7/4855685#4855685>
[inst2]: <http://stackoverflow.com/questions/3387695/add-to-python-path-mac-os-x/3387737#3387737>
