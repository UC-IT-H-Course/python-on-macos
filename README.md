<div align="center">

# Python on macos

This is a general guide for installing and using python on macos

<div>

# Installing

I strongly recommend installing through brew because it is easier to update. First install brew by running the following command in your terminal:

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Then install python through brew:

```sh
brew install python
```

# Troubleshooting macos issues

## `ModuleNotFoundError: No module named '_tkinter'`

For the following error:

```
File "/Users/school/Documents/uc/ui.py", line 1, in <module>
    from tkinter import *
  File "/usr/local/Cellar/python@3.9/3.9.6/Frameworks/Python.framework/Versions/3.9/lib/python3.9/tkinter/__init__.py", line 37, in <module>
    import _tkinter # If this fails your Python may not be configured for Tk
ModuleNotFoundError: No module named '_tkinter'
```

Can be resolved:

```sh
brew install python-tk
```
