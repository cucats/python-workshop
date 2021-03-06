# Preparation for CUCaTS coding workshop

<!-- MarkdownTOC autolink=true depth=6 bracket=round -->

- [Installing Python](#installing-python)
    - [Windows](#windows)
    - [Mac](#mac)
    - [Linux](#linux)
- [Installing the package installer (Optional)](#installing-the-package-installer-optional)
    - [Windows](#windows-1)
    - [Mac and Linux](#mac-and-linux)
    - [Using pip (Optional)](#using-pip-optional)

<!-- /MarkdownTOC -->


## Installing Python

[Python](https://www.python.org) is both a programming language and a piece of software. There are two popular versions of Python: Python 2 and Python 3. We are going to be using Python 3, which is more modern.

It will save time if you can install Python 3 on your laptop before the workshop - instructions on how to do so follow.

### Windows

* Download the [Windows x86-64 MSI installer](https://www.python.org/ftp/python/3.4.2/python-3.4.2.amd64.msi) for 64 bit Windows or [Windows x86 MSI installer](https://www.python.org/ftp/python/3.4.2/python-3.4.2.amd64.msi) for 32 bit Windows. If in doubt, choose 32 bit.
    * The choice between 64 and 32 bit only matters if you want to install libraries in the future, as you will need to install the same version as your Python version.
* Run it and follow instructions.
* Choose `add python.exe to path` so that you can run it from the command line with `python`

![Remember to add python.exe to path for easier access](img/window_installer.png)

* To test if your installation is successful, you can press `windows + R`, type `cmd` and press enter to launch the command prompt (a black box into which you can type commands). Then type `python` and press enter. The Python console should start - you should see something like:
```
Python 3.4.2 (default, Dec 27 2014, 13:16:08) 
[Something] on Windows
Type "help", "copyright", "credits" or "license" for more information.
>>>
```
You can then close the window.

* If you see Python 2.7, then start with `py -3` instead.

### Mac

* For OS X 10.6 and above, Download and run [this](https://www.python.org/ftp/python/3.4.2/python-3.4.2-macosx10.6.pkg).
* Open your terminal by pressing `cmd + space` and entering `terminal`. Type `python3`. (Don't include the full stop.)

### Linux

* Open a terminal and install Python 3 using your package manager. For example, `sudo apt-get install python3` or `sudo yum install python3`.

## Installing the package installer (Optional)

This is not necessary for the workshop. But if you want to use Python in the future, this might come in handy.

Python comes with many useful libraries which you can install easily with a package manager. Here we will provide instructions for installing [pip](https://pip.pypa.io/en/latest/installing.html). 

### Windows
* The Python 3 installer installs pip by default. You can check that pip is installed by entering `pip --version` or `py -3 -m pip --version` in your command prompt. If the first command gives you an error but the second one works, you might want to update pip by entering `py -3 -m pip install --upgrade pip`. Then `pip --version` should work.
* If pip is not installed, you can install it like so:
    * Download the [installer script](https://bootstrap.pypa.io/get-pip.py) and save it somewhere (e.g. your desktop). 
    * Browse to the location where you saved the installer. Then hold down `shift` and right click on an empty space in your file explorer, and select `Open command window here`.
    * Type `py get-pip.py` and press enter.

### Mac and Linux
* Check if you have pip installed: open your terminal and type `pip` or `python3 -m pip`. If you don't get an error, then pip is already installed.
* If you don't have pip, you can run the following command which is a script to download the installer and installing it.
    - `curl -OL https://bootstrap.pypa.io/get-pip.py && python3 get-pip.py`
    - If it complains about permission denied, run `sudo python3 get-pip.py`

### Using pip (Optional)

You can install packages by typing `pip install <package-name>`. For example, if we wanted plotting functionalities, we could install [matplotlib](http://matplotlib.org/) by typing `pip install matplotlib`.
