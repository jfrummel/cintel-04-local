# cintel-04-local
Python Project Virtual Environment
Run the following commands in the terminal to set up a project virtual environment and install the necessary packages. Run them from the root project folder (e.g. pyshiny-penguins-dashboard-express). Use PowerShell on Windows or the terminal on macOS and Linux.

Create a Project Virtual Environment (generally one-time setup)
Create a project virtual environment in the .venv folder of the project root directory.

py -m venv .venv
Creating a project virtual environment is generally a one-time setup. Once the folder exists, we can activate it to work on the project.

If VS Code pops up and says: We noticed a new environment has been created. Do you want to select it for the workspace folder? select Yes.

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
