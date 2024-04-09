GUI for generating BIDS Stats Model spec json files.

Work in progress.  Current version only prints the json to screen for testing purposes.

run using `python main_gui.py`


Mac users:  If you're running Sonoma, you'll need python 3.12 or newer, most importantly it must be running tcl.tk 8.6.13 or higher. \
As far as I know tcl.tk is updated only with python.  If `pyenv install python 3.12.0` is used it should be fine.  If you use conda it will not install 
the updated tcl.tk version.

If you need it, here's how to check your tcl.tk version.  
```#!/usr/bin/python
# coding: utf-8

import sys

try:
    import Tkinter as tk      # Python 2
except ImportError:
    import tkinter as tk      # Python 3

print("Tcl Version: {}".format(tk.Tcl().eval('info patchlevel')))
print("Tk Version: {}".format(tk.Tk().eval('info patchlevel')))
sys.exit()
```
