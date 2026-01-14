What I Learned

In this lab, I learned how to use Python virtual environments (venv) to isolate project dependencies. I practiced creating, activating, installing packages inside, and deactivating a virtual environment. This helped me understand how virtual environments prevent dependency conflicts and ensure consistent project setups.

 Lab Objectives

Understand the purpose and benefits of Python virtual environments

Learn how to create, activate, and deactivate a virtual environment

Practice installing packages inside a virtual environment

Understand dependency isolation for multiple projects

 Prerequisites

Basic familiarity with Python

Basic command line usage

Python 3.3 or later installed

 Lab Tasks Performed

🔹 Task 1: Create a Virtual Environment

Objective:
Create an isolated Python environment for a project.

Commands Used:

mkdir my_project
cd my_project
python -m venv myenv


 Explanation

python -m venv myenv creates a virtual environment named myenv

The environment contains its own Python interpreter and libraries

Helps isolate project dependencies

🔹 Task 2: Activate the Virtual Environment

Objective:
Activate the virtual environment to start using it.

Linux / macOS:

source myenv/bin/activate


Windows:

.\myenv\Scripts\activate


🔍 Explanation

Once activated, the terminal prompt changes (e.g., (myenv))

All Python and pip commands now use the virtual environment

🔹 Task 3: Install a Package Inside the Virtual Environment

Objective:
Install packages without affecting global Python packages.

Command Used:

pip install requests


Verify Installation:

pip list


🔍 Explanation

The requests package is installed only inside myenv

Other projects or global Python remain unaffected

pip list confirms installed packages

🔹 Task 4: Deactivate the Virtual Environment

Objective:
Exit the virtual environment and return to the system Python.

Command Used:

deactivate


🔍 Explanation

Deactivating restores the global Python environment

The (myenv) prefix disappears from the terminal

🧩 Key Concepts

Virtual Environment: Isolated Python workspace for a project

Dependency Isolation: Prevents version conflicts between projects

venv Module: Built-in Python tool for environment management

📌 Examples & Use Cases

Scenario:

Project A → requests==2.25.1

Project B → requests==2.26.0

Using separate virtual environments allows both projects to run without conflicts.

Real-World Application:

Web applications

Microservices

Internship & production environments

Collaborative development

 Summary 

In this lab, I successfully:

Created and activated a Python virtual environment

Installed packages in an isolated environment

Deactivated the environment safely

Understood the importance of dependency isolation

Virtual environments are essential for clean, scalable, and professional Python development.
