### Modules & PIP

Lets focus on understanding Python modules, how to use them, and how to install and manage external packages using PIP.

**1. Modules**

   Modules in Python are files containing Python code that can define functions, classes, and variables. They can also include runnable code. The code in the module can be reused in other Python scripts.
   
   1. **Creating and Using Modules**
   
      - Create a new Python file named `mymodule.py` and add the following code:
        ```python
        def greet(name):
            return f"Hello, {name}!"
        ```
   
      - Now, create another Python file named `main.py` and use the module:
        ```python
        import mymodule
   
        print(mymodule.greet("Alice"))
        ```
   
      - Run `main.py`:
        ```sh
        python main.py
        ```
   
      - You should see the output: `Hello, Alice!`
   
   2. **Using Standard Library Modules**
   
      Python comes with a rich standard library. Here are some examples:
   
      - **Math Module**:
        ```python
        import math
   
        print(math.sqrt(16))  # Outputs: 4.0
        ```
   
      - **Datetime Module**:
        ```python
        import datetime
   
        now = datetime.datetime.now()
        print("Current date and time:", now)
        ```
   
   3. **Importing Specific Attributes**
      - You can import specific functions or variables from a module:
        ```python
        from math import pi, sqrt
   
        print(pi)         # Outputs: 3.141592653589793
        print(sqrt(16))   # Outputs: 4.0
        ```
   
   4. **Aliasing Modules**
      - You can give a module a different alias:
        ```python
        import datetime as dt
   
        now = dt.datetime.now()
        print("Current date and time:", now)
        ```

**2. PIP (Python Package Installer)**

   PIP is the package installer for Python. It allows you to install and manage additional libraries and dependencies that are not included in the standard library.
   
   1. **Checking PIP Version**
      - Verify that PIP is installed and check its version:
        ```sh
        pip --version
        ```
   
   2. **Installing Packages**
      - Install a package using PIP:
        ```sh
        pip install requests
        ```
   
      - Verify the installation by importing the package in a Python script:
        ```python
        import requests
   
        response = requests.get('https://api.github.com')
        print(response.status_code)
        ```
   
   3. **Listing Installed Packages**
      - List all installed packages:
        ```sh
        pip list
        ```
   
   4. **Uninstalling Packages**
      - Uninstall a package:
        ```sh
        pip uninstall requests
        ```
   
   5. **Upgrading Packages**
      - Upgrade a package to the latest version:
        ```sh
        pip install --upgrade requests
        ```
   
   6. **Requirements File**
      - Create a `requirements.txt` file to manage project dependencies. This file lists all the packages your project depends on.
      - Example `requirements.txt`:
        ```
        requests==2.25.1
        numpy==1.20.1
        ```
   
      - Install packages from `requirements.txt`:
        ```sh
        pip install -r requirements.txt
        ```

**Practical Exercises**

   1. **Exercise 1: Creating a Module**
      - Create a module called `math_operations.py` with functions for addition, subtraction, multiplication, and division.
      - Example:
        ```python
        # math_operations.py
        def add(a, b):
            return a + b
   
        def subtract(a, b):
            return a - b
   
        def multiply(a, b):
            return a * b
   
        def divide(a, b):
            if b != 0:
                return a / b
            else:
                return "Division by zero is not allowed"
        ```
   
      - Use this module in another script:
        ```python
        # main.py
        import math_operations as mo
   
        print(mo.add(10, 5))
        print(mo.subtract(10, 5))
        print(mo.multiply(10, 5))
        print(mo.divide(10, 5))
        ```
   
   2. **Exercise 2: Installing and Using an External Package**
      - Install the `requests` package and use it to make an HTTP request.
      - Example:
        ```python
        import requests
   
        response = requests.get('https://jsonplaceholder.typicode.com/todos/1')
        print(response.json())
        ```

**Resources and Further Reading**

   1. **Python Modules**
      - [Python Official Documentation - Modules](https://docs.python.org/3/tutorial/modules.html)
      - [Automate the Boring Stuff with Python - Chapter 6](https://automatetheboringstuff.com/2e/chapter6/)
   
   2. **PIP**
      - [Python Packaging User Guide](https://packaging.python.org/tutorials/installing-packages/)
      - [PIP Documentation](https://pip.pypa.io/en/stable/)

**Summary**

   You have:
   - Learned how to create and use Python modules.
   - Explored some standard library modules.
   - Installed and managed external packages using PIP.
   - Completed practical exercises to reinforce your learning.
