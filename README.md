# Python Contact Book

A simple contact book made using PySimpleGui.

Saves all contacts through a json file stored in `(user home dir)/.config/banjo/py-contact-book`, 
as well as some stats and (maybe in the future) actual configuration values.

## Running
You are able to find the latest release [here.](https://github.com/BanjoTheBot/py_contact_book/releases)

Here you can download the .exe file for usage on Windows, or a generic executable file for Linux. 
After that it should be a simple click and play.

## Compiling
If you would like to run the file through Python directly or make changes to the code, here are the steps to follow.

Once you have the repo cloned, run these commands to create the venv and install all necessary requirements.

On Windows:
```
python -m venv venv
.\venv\Scripts\activate
pip install -r requirements.txt
```

**NOTE: On Linux, you may need to install TKinter, more info [here.](https://stackoverflow.com/questions/25905540/importerror-no-module-named-tkinter)**
Do this **BEFORE** you run these commands.

On Linux and macOS:
```
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

To run from Python, simply run `py-contact-book.py` from your IDE or CLI.

If you want to compile an executable file, we use PyInstaller. Run this command to compile as expected. 
Pyinstaller should have been downloaded when you installed from requirements.txt earlier.
```
pyinstaller py_contact_book.spec
```