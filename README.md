GUI for generating BIDS Stats Model spec json files.

## Installation
It is best to use this tool within a conda environment.  You can use the following commands from within this directory to set up the environment and install the package.
```
conda create -n bids-sm-maker python=3.12.2
conda activate bids-sm-maker
pip install -e .
```
Once the package is installed, as long as you are working in the `bids-sm-maker` environment, you can launch the GUI from any directory using the `make_spec` command.


## Mac users, please check tcl/tk version
It is important that Sonoma users are using a version of Python that has been paired with a version of tcl/tk > 8.6.13.  If an older version of tcl/tk was installed, it is difficult for the GUI to register mouse clicks.

To check which version of tcl/tk was installed, in python run:
```
import tkinter as tk
print("Check that both of these output version numbers > 8.6.13")
print("Tcl Version: {}".format(tk.Tcl().eval('info patchlevel')))
print("Tk Version: {}".format(tk.Tk().eval('info patchlevel')))

```

## Work in progress.  
Current version only prints the json to screen for testing purposes.



