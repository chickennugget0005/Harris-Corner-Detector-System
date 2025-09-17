# Create a virtual Environment to run any of these programs
# You need to download pakages OpenCV, numpy as np, p& yzed.sl as


#Error when tried to install python package because it can corrupt the system python installation used at system level. Ubuntu 22.04+

This environment is externally managed ╰─> To install Python packages system-wide, try apt install python3-xyz, where xyz is the package you are trying to install.

# Tried using pipx to install package globally without it affecting the system as a whole.
# installation 
$ sudo apt install pipx

# was a success but when installed still didnt work with code.
$ pip install opencv

# The final resort that I had to use was making a venv (virtual environment) so that the package could be installed locally in the venv.

# How to start virtual environment:

# whenever you are making the virtual environment for the first time:
# select the 3.13.7 or whatever there is on the bottom right of the Visual Studio Code screen
# Then click on create a virtual environment, that should create a .venv folder in the workspace (folder in which you are working in)
# This should be it for creating the venv

# whenever you are working on some code click (Ctrl + `) to open a terminal
# then you have to source the venv:
$ source venv/bin/activate

# This should show a (venv) before the command line. 

# Now you can install whatever you want and it shouldnt interfere with the global environment. 


# to exit the venv:
$ deactivate 
# or just close the terminal

# Remember!! Always source venv/bin/activate from your project folder!

# if you see yellow lines under the thing again
# type: to check the installed packages 
$ python -m pip list 

# To see the python version you are working with:
$ which python

# Ensure that the selected interpreter is venv one!
