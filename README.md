# mage-ai
  Data pipeline using mage ai data orchestration

## 1.This Project will cover the following Tech stack: 
	1. Visual Studio Code (install it in your local system)
	2. Python 3.11.7(64bit) (install it in your local system and add PATH to your environment)
	3. PostgreSQL (install it in your local system)
	4. Mage -AI for orchestration 
	5. Git 

# 2.Create a git repository in github <mageai>
  
  	• C:\Users\abc\Downloads\mage> 
  **(Select a directory in VS Code)**
  
  	• C:\Users\abc\Downloads\mage\mageai>git clone path

# 3.To Create Environment

### Using VS Code editor
• **Ctrl+Shift+P** (command palette in VS Code)

• Select --> Python: Create Environment

• Venv Creates a '.venv' virtual environment in the current workspace
	
 ## (OR)

### Using Command Prompt in VS Code
• **Ctrl+~** (to open terminal for cmd/bash/powershell)
	
 	• C:\Users\abc\Downloads\mage\mageai>pip install virtualenv 
 
 **(if you have already installed then skip this step)**
	
 	• C:\Users\abc\Downloads\mage\mageai>python -m venv <env_name> 
 
 **(replace <env_name> with your project_name)**

# 4.To Activate Environment variables

### Using Command Prompt
 	
  	• C:\Users\abc\Downloads\mage\mageai>cd .venv\Scripts\activate 
 
 **(to activate environment variable)**

## (OR)

### Using BASH script
	
 	• abc@madhu MINGW64 ~/Downloads/mage/mageai $ source .venv/Scripts/activate

# 5.To install MAGE-AI
	• C:\Users\abc\Downloads\mage\mageai>pip install mage-ai 
 **(installation completed)**
 
 Incase of any ERRORS skip the next steps, kindly follow **6.NOTE & 7.SOLUTION** (specific to those errors only)
	
	• C:\Users\abc\Downloads\mage\mageai>mage init new_proj
 
 **(to initiate a project)**:

 	• C:\Users\abc\Downloads\mage\mageai>pip freeze > new_proj/requirements.txt

 **(to save project dependencies to requirements.txt file)**:

	• C:\Users\abc\Downloads\mage\mageai>mage start metro_proj 
 
 **(to launch project localhost on PORT 6789 / localhost:6789)**

 
	• C:\Users\abc\Downloads\mage\mageai>mage init new_proj 

 **(to create/initialise a new project)**

   	• C:\Users\abc\Downloads\mage\mageai>pip install psycopg2 
 
 **(for postgresql connections)**

# 6.NOTE:
	• This error originates from a subprocess, and is likely not a problem with pip.
### ERROR
	• Failed building wheel for pyzmq (installed microsoft build tools to microsoft visual c++ 14.0 or greater is required)
	• Failed building wheel for pyarrow (pyproject.toml)
### ERROR: 
  	Could not build wheels for **pyarrow, pyzmq**, which is required to install pyproject.toml-based projects

# 7.SOLUTION: 
	
	• C:\Users\abc\Downloads\mage\mageai>pip install streamlit==0.62.0 
 
 **(didn't work again -->Failed building wheel for pyarrow)**

 	• C:\Users\abc\Downloads\mage\mageai>pip install pyzmq 
 
 **(didn't work again)**

 	• C:\Users\abc\Downloads\mage\mageai>pip install --upgrade pip setuptools wheel

Building wheel for pyzmq (pyproject.toml)(again failed for both processes)
	
 **Re-install python 3.11.7(64bit)**

 	• C:\Users\abc\Downloads\mage\mageai>
 
 **(Select a directory)** (follow from **4.To Activate Environment variables** and next steps)

# 8.ADDITIONAL DEPENDECIES IF NEEDED:
• Install Jupiter Notebook inside VS Code
• Need to Select Kernel (default is current virtual env)
 
	• C:\Users\abc\Downloads\mage\mageai>pip install psycopg2 

**(to export to postgre sql)**

   	• C:\Users\abc\Downloads\mage\mageai>pip install sshtunnel
