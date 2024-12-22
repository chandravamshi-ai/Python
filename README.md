# Python

Complete Python course form beginner to advance concepts
<!---
### Enhanced Roadmap to Becoming a Python Pro

**Resources:**
- [100 Days of Code Playlist](https://www.youtube.com/playlist?list=PLu0W_9lII9agwh1XjRt242xIpHhPT2llg)
- [Hand Written Python Notes](https://www.codewithharry.com/notes/)
- [Automate the Boring Stuff with Python](https://automatetheboringstuff.com/)
- [Python Documentation](https://docs.python.org/3/)
- [Learning Python – O’Reilly](https://www.oreilly.com/library/view/learning-python/1565924649/)
- [Python Course by Dr. Angela Yu on Udemy](https://click.linksynergy.com/linkid=vzG/OMx7ecI&offerid=1388962.3919715219197173821843440&type=2&murl=https%3A%2F%2Fwww.udemy.com%2Fcourse%2F100-days-of-code%2F)


#### 1. Python Basics

   a. Basic Syntax

   1. **Hello World**
      - Write your first Python program that prints "Hello, World!"
      - Understand the structure of a simple Python script.
      - **Resource**: [Python Official Documentation - First Steps](https://docs.python.org/3/tutorial/introduction.html#using-python-as-a-calculator)
   
   2. **Comments**
      - Learn how to write single-line (`# this is a comment`) and multi-line comments (`""" this is a comment """`).
      - **Resource**: [Automate the Boring Stuff with Python - Chapter 1](https://automatetheboringstuff.com/)
   
   3. **Indentation**
      - Understand the importance of indentation in Python for defining code blocks.
      - **Resource**: [Python Indentation Guide](https://docs.python.org/3/reference/lexical_analysis.html#indentation)
   
   4. **Python Identifiers**
      - Learn about naming conventions and rules for Python identifiers (variable names).
      - **Resource**: [Python Naming Conventions](https://pep8.org/#naming-conventions)
   
   b. Modules & PIP
   
   1. **Importing Modules**
      - Learn how to import and use standard library modules, e.g., `import math`.
      - **Resource**: [Python Official Documentation - Modules](https://docs.python.org/3/tutorial/modules.html)
   
   2. **Installing Packages with PIP**
      - Understand how to use PIP to install external libraries and packages.
      - Example: `pip install requests`.
      - **Resource**: [Python Packaging User Guide](https://packaging.python.org/tutorials/installing-packages/)
   
   3. **Using Packages**
      - Practice using installed packages in your projects.
   
   c. Variables & Data Types
   
   1. **Variables**
      - Learn how to declare and initialize variables.
      - Example: `x = 10`.
      - **Resource**: [Python Variables](https://docs.python.org/3/tutorial/introduction.html#using-python-as-a-calculator)
   
   2. **Data Types**
      - Understand different data types: integers, floats, strings, booleans.
      - Example: `int`, `float`, `str`, `bool`.
      - **Resource**: [Python Data Types](https://docs.python.org/3/library/stdtypes.html)
   
   3. **Type Conversion**
      - Learn how to convert between different data types.
      - Example: `str(10)`, `int('10')`.
      - **Resource**: [Python Type Conversion](https://www.geeksforgeeks.org/type-conversion-python/)
      
   d. Conditionals and Loops
   
   1. **If-Else Statements**
      - Write conditional statements using if, elif, and else.
      - Example: `if x > 0: print("Positive")`.
      - **Resource**: [Python Control Flow](https://docs.python.org/3/tutorial/controlflow.html)
   
   2. **While Loops**
      - Learn how to create loops that run while a condition is true.
      - Example: `while x > 0: x -= 1`.
      - **Resource**: [Python While Loops](https://www.w3schools.com/python/python_while_loops.asp)
   
   3. **For Loops**
      - Iterate over sequences such as lists, tuples, and strings.
      - Example: `for i in range(5): print(i)`.
      - **Resource**: [Python For Loops](https://www.w3schools.com/python/python_for_loops.asp)
   
   4. **Break and Continue**
      - Understand how to control loop execution with break and continue statements.
      - Example: `break` to exit a loop, `continue` to skip an iteration.
      - **Resource**: [Python Break and Continue](https://www.w3schools.com/python/python_while_loops.asp)

   e. Functions & Recursion
   
   1. **Defining Functions**
      - Learn how to define and call functions.
      - Example: `def greet(): print("Hello!")`.
      - **Resource**: [Python Functions](https://docs.python.org/3/tutorial/controlflow.html#defining-functions)
   
   2. **Parameters and Arguments**
      - Understand how to pass parameters to functions and return values.
      - Example: `def add(a, b): return a + b`.
      - **Resource**: [Python Function Arguments](https://www.w3schools.com/python/python_functions.asp)
   
   3. **Default Arguments**
      - Learn how to use default arguments in functions.
      - Example: `def greet(name="World"): print("Hello, " + name)`.
      - **Resource**: [Python Default Arguments](https://www.geeksforgeeks.org/default-arguments-in-python/)
   
   4. **Recursion**
      - Understand the concept of recursion and write simple recursive functions.
      - Example: `def factorial(n): return 1 if n == 0 else n * factorial(n-1)`.
      - **Resource**: [Python Recursion](https://www.geeksforgeeks.org/recursion/)
   
   f. Collections: List, Tuple, Sets, Dictionaries
   
   1. **Lists**
      - Create and manipulate lists, including slicing and list comprehensions.
      - Example: `my_list = [1, 2, 3]`.
      - **Resource**: [Python Lists](https://docs.python.org/3/tutorial/datastructures.html#more-on-lists)
   
   2. **Tuples**
      - Understand tuples and their immutability.
      - Example: `my_tuple = (1, 2, 3)`.
      - **Resource**: [Python Tuples](https://docs.python.org/3/tutorial/datastructures.html#tuples-and-sequences)
   
   3. **Sets**
      - Learn about sets and set operations like union, intersection, and difference.
      - Example: `my_set = {1, 2, 3}`.
      - **Resource**: [Python Sets](https://docs.python.org/3/tutorial/datastructures.html#sets)
   
   4. **Dictionaries**
      - Create and manipulate dictionaries, and understand key-value pairs.
      - Example: `my_dict = {"name": "Alice", "age": 25}`.
      - **Resource**: [Python Dictionaries](https://docs.python.org/3/tutorial/datastructures.html#dictionaries)
   
   g. File I/O
   
   1. **Reading Files**
      - Learn how to open and read files in Python.
      - Example: `with open('file.txt', 'r') as file: contents = file.read()`.
      - **Resource**: [Python File Reading](https://www.w3schools.com/python/python_file_handling.asp)
   
   2. **Writing Files**
      - Understand how to write data to files.
      - Example: `with open('file.txt', 'w') as file: file.write("Hello, World!")`.
      - **Resource**: [Python File Writing](https://www.w3schools.com/python/python_file_write.asp)
   
   3. **File Methods**
      - Explore various file methods such as read(), readline(), and readlines().
      - Example: `file.readline()`.
      - **Resource**: [Python File Methods](https://docs.python.org/3/tutorial/inputoutput.html#methods-of-file-objects)
  
2. Advanced Python

   1. **Iterators and Generators**
      - Learn about creating iterators and generators for efficient looping.
   2. **Regex**
      - Practice complex pattern matching.
   3. **Decorators**
      - Create and use decorators to extend functionality.
   4. **Lambdas**
      - Utilize anonymous functions in various contexts.
   5. **List Comprehensions**
      - Write more complex comprehensions.
   6. **Exception Handling**
      - Learn best practices for error handling.

3. Object-Oriented Programming (OOP)

   1. **Classes & Objects**
      - Deep dive into class structures and instances.
   2. **Methods**
      - Explore class methods, static methods, and instance methods.
   3. **Inheritance and Polymorphism**
      - Understand and implement inheritance and polymorphism.
   4. **OOP Projects**
      - Build larger projects to apply OOP principles.

4. Data Structures & Algorithms

   1. **Basic Concepts**
      - Time Complexity
      - Arrays and Lists
      - Linked Lists
      - Stacks and Queues
      - Trees and Graphs
      - Sorting and Searching Algorithms
   2. **Additional Resources**
      - [Geeks for Geeks DSA Tutorials](https://www.geeksforgeeks.org/data-structures/)

5. Web Development Frameworks

   1. **Flask**
      - [Flask Mega-Tutorial](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world)
   2. **Django**
      - [Django Girls Tutorial](https://tutorial.djangogirls.org/en/)
   3. **FastAPI**
      - [FastAPI Tutorial](https://fastapi.tiangolo.com/tutorial/)

6. Game Development & GUI (Optional)

   1. **Tkinter**
      - Create small projects to practice GUI development.
   2. **PyGame**
      - Build simple games to understand game loops and event handling.

7. Web Scraping

   1. **Requests**
      - Practice making HTTP requests and handling responses.
   2. **BeautifulSoup (BS4)**
      - [Web Scraping Tutorial](https://www.youtube.com/watch?v=ng2o98k983k)
   3. **Selenium**
      - Learn web automation and browser interactions.
   4. **PyAutoGUI**
      - Automate repetitive tasks.

8. Tools to Speed Up Workflow

   1. **Git & GitHub**
      - Master version control and collaboration.
      - [Pro Git Book](https://git-scm.com/book/en/v2)
   2. **Ollama**
      - Explore any video tutorials and documentation.
   3. **GitHub Copilot**
      - Use it to assist with code suggestions and completions.

9. Machine Learning & Data Science

   1. **Core Concepts**
      - Data manipulation with Pandas and NumPy.
      - Data visualization with Matplotlib and Seaborn.
      - [Python for Data Analysis by Wes McKinney](https://wesmckinney.com/book/)
   2. **Machine Learning**
      - [Hands-on ML with Scikit-learn and TensorFlow](https://amzn.to/3xKMgmo)
      - Participate in Kaggle competitions for practical experience.
   3. **Additional Resources**
      - [Coursera Machine Learning Course by Andrew Ng](https://www.coursera.org/learn/machine-learning)


Additional Suggestions

   1. **Practice Regularly**
      - Code daily and practice with real-world projects.
   2. **Join Communities**
      - Engage with Python communities on Reddit, Stack Overflow, and Discord.
   3. **Contribute to Open Source**
      - Start contributing to open-source projects to gain experience.

Project Ideas

   1. **Personal Portfolio Website**
      - Build a website to showcase your projects and resume.
   2. **Blog Platform**
      - Create a blog with a content management system.
   3. **E-commerce Site**
      - Develop an online store with product listings, cart, and checkout.
   4. **Data Analysis Project**
      - Analyze datasets and create visualizations.
   5. **Automation Scripts**
      - Automate repetitive tasks on your computer.
   6. **5 Python Projects in One Video**
      - [Watch here](https://www.youtube.com/playlist?list=PLu0W_9lII9agqZuv_XJen_BEHycIh-FmG)
   7. **JARVIS AI Agent**
   8. **Flappy Bird**
   9. **Indian Railway Announcement System**
   10. **End-to-End ML Project**
   11. **Umpire Decision Review System (DRS)**
--->

