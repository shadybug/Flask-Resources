1. Create a new folder for your project. You should always use one folder per project.
2. In VS Code, File->Open Folder. Navigate to the project folder you just created, and press "Open".
3. If you haven't already: open the Extensions tab on your left sidebar. Install the Python and HTML CSS Support extensions.
4. Open up a terminal in VS Code (Terminal->New Terminal)
5. Set up your virtual environment. If you've done this correctly, there should be a (.venv) at the beginning of your lines in the terminal. 
### macOS
> python3 -m venv .venv
> 
> source .venv/bin/activate

### Windows
> py -3 -m venv .venv
> 
> .venv\scripts\activate
6. Open the command palette (Ctrl+Shift+P) and select Python: Select Interpreter. Click on the one that says "('.venv': venv)"
7. Load pip (a Python program manager) into your virtual environment.
> python -m pip install --upgrade pip
8. Install Flask into the virtual environment.
> python -m pip install flask
9. If you plan to use a database, install the Python-MySQL connector so that we can communicate with it.
> python -m pip install mysql-connector-python 
10. Make a file called "app.py", and folders called "static" and "templates" as needed. Make sure the names are exact, or Flask won't recognize them!
