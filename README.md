# cintel-04-local
Activate the Project Virtual Environment (when you work on the project)
Once the project virtual environment exists, we activate the virtual environment to work on the project - or when we open a new terminal.

On Windows:

.venv\Scripts\Activate
On macOS and Linux:

source .venv/bin/activate
Verify: Generally when the environment is active, (.venv) will appear in the terminal prompt.

We also need to select this project virtual environment in VS Code. To do this:

Open the VS Code command palette (Ctrl+Shift+P).
Search for "Python: Select Interpreter".
Select the .venv folder in the project root directory.
Install Packages into the Active Project Virtual Environment
When the project virtual environment is active, install packages into the project virtual environment so they are available for use in the Python code.

NOTE:

We install packages into the project virtual environment.
We import packages into Python code (after they have been installed).
First, upgrade pip and setuptools (core packages) for good measure. NOTE: Using the palmerpenguins package requires setuptools. Then, install the project-specific required packages.

With the project virtual environment active in the terminal, run the following commands:

py -m pip install --upgrade pip setuptools
py -m pip install --upgrade -r requirements.txt
Installing packages is generally a one-time setup.

Run the App
With your project virtual environment active in the terminal and the necessary packages installed, run the app with live reloading and automatically open it in the browser:

shiny run --reload --launch-browser penguins/app.py
While the app is running, that terminal is fully occupied. Open a new terminal to run other commands.