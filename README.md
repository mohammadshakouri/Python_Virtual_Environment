# 🐍 Python Virtual Environment Setup Guide
### This documentation explains how to create and manage a virtual environment for your Python projects.
#### 1. Create a virtual environment
```
python -m venv .venv
```
This command creates a virtual environment in a folder named .venv.
You can replace .venv with any folder name you prefer.

#### 2. Activate the virtual environment
#### 🪟 On Windows:
```
.venv\scripts\activate.bat
```
#### 🐧 On macOS / Linux:
```
source .venv/bin/activate
```
Once activated, your terminal prompt will usually show the environment name at the start (e.g. (.venv)).

#### 3. Check installed packages
```
pip list
```
Shows the list of installed packages inside the virtual environment.

#### 4. Upgrade pip (recommended)
```
python.exe -m pip install --upgrade pip
```
Keeps your pip version up to date.

#### 5. Save dependencies to requirements.txt
```
pip freeze > requirements.txt
```
This creates a list of all installed packages so you can recreate the environment later.

#### 6. Install dependencies from requirements.txt
```
pip install -r requirements.txt
```
Use this when setting up the environment on another machine or after cloning a project.
(Optional if you’re starting fresh.)

#### 7. Deactivate the virtual environment
```
deactivate
```
This exits the virtual environment and returns to your global Python environment.

### ✅ Optional Tips
- To remove the environment: simply delete the .venv folder.
- To check Python version in the venv:
```
python --version
```


