[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15305269&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
   Python is an open-source programming language that is free to use and distribute. Many developers worldwide utilized it to create GUI applications and web applications with fewer, easily readable codes. Building large and complicated software applications is much faster with lesser time. Examples of where python is used: Time series analysis, data visualization, sales prediction, language processing.

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

Step 1: Select Python Version
I chose the latest version

Step 2: Download Python Executable Installer
Start by downloading the Python executable installer for Windows:

1. Open a web browser and navigate to the Downloads for Windows section of the official Python website.

2. Locate the desired Python version.

Python executable download page 64 and 32 bit
3. Click the link to download the file. i Chose 64-bit installer

Step 3: Run Executable Installer
The steps below guided me through the installation process:

1. Run the downloaded Python Installer.

2. The installation window shows two checkboxes:

Admin privileges. The parameter controls whether to install Python for the current or all system users. This option allows you to change the installation folder for Python.
Add Python to PATH. The second option places the executable in the PATH variable after installation. You can also add Python to the PATH environment variable manually later.
Python installer admin privileges and path
For the most straightforward installation, we recommend ticking both checkboxes.

3. Select the Install Now option for the recommended installation (in that case, skip the next two steps).

To adjust the default installation options, choose Customize installation instead and proceed to the following step.

Python installer Install Now or Customize
The default installation installs Python to C:\Users\[user]\AppData\Local\Programs\Python\Python[version] for the current user. It includes IDLE (the default Python editor), the PIP package manager, and additional documentation. The installer also creates necessary shortcuts and file associations.

Customizing the installation allows changing these installation options and parameters.

4. Choose the optional installation features. Python works without these features, but adding them improves the program's usability.

Python installer optional features
Click Next to proceed to the Advanced Options screen.

5. The second part of customizing the installation includes advanced options.

Choose whether to install Python for all users. The option changes the install location to C:\Program Files\Python[version]. If selecting the location manually, a common choice is C:\Python[version] because it avoids spaces in the path, and all users can access it. Due to administrative rights, both paths may cause issues during package installation.

Other advanced options include creating shortcuts, file associations, and adding Python to PATH.

Python installer advanced options
After picking the appropriate options, click Install to start the installation.

6. Select whether to disable the path length limit. Choosing this option will allow Python to bypass the 260-character MAX_PATH limit.

Python installer setup successful
The option will not affect any other system settings, and disabling it resolves potential name-length issues. We recommend selecting the option and closing the setup.

Step 4: Add Python to Path (Optional)
If the Python installer does not include the Add Python to PATH checkbox or you have not selected that option, continue in this step. Otherwise, skip to the next step.

Adding the Python path to the PATH variable alleviates the need to use the full path to access the Python program in the command line. It instructs Windows to review all the folders added to the PATH environment variable and to look for the python.exe program in those folders.

To add Python to PATH, do the following:

1. In the Start menu, search for Environment Variables and press Enter.

Start Environment Variables search result
2. Click Environment Variables to open the overview screen.

System properties environment variables button.
3. Double-click Path on the list to edit it.

Environment Variables list Path variable
Alternatively, select the variable and click the Edit button.

4. Double-click the first empty field and paste the Python installation folder path.

Path Python new entry
Alternatively, click the New button instead and paste the path.

5. Click OK to save the changes. If the command prompt is open, restart it for the following step.

Step 5: Verify Python Was Installed on Windows
The first way to verify that Python was installed successfully is through the command line. Open the command prompt and run the following command:

python --version

python --version 3.12.0 CMD output
The output shows the installed Python version.

The second way is to use the GUI to verify the Python installation. Follow the steps below to run the Python interpreter or IDLE:

1. Navigate to the directory where Python was installed on the system.

2. Double-click python.exe (the Python interpreter) or IDLE.

3. The interpreter opens the command prompt and shows the following window:

Python 3.12.0 interpreter window
Running IDLE opens Python's built-in IDE:

Python 3.12.0 IDLE shell
In both cases, the installed Python version shows on the screen, and the editor is ready for use.

Step 6: Verify PIP Was Installed
To verify whether PIP was installed, enter the following command in the command prompt:

pip --version

If it was installed successfully, you should see the PIP version number, the executable path, and the Python version:

pip --version 23.2.1 CMD output
PIP has not been installed yet if you get the following output:

'pip' is not recognized as an internal or external command,
Operable program or batch file.

If an older version of Python is installed or the PIP installation option is disabled during installation, PIP will not be available. To install PIP, see our article How to Install PIP on Windows.

Step 7: Install virtualenv (Optional)
Python software packages install system-wide by default. Consequently, whenever a single project-specific package is changed, it changes for all your Python projects.

The virtualenv package enables making isolated local virtual environments for Python projects. Virtual environments help avoid package conflicts and enable choosing specific package versions per project.

To install virtualenv, run the following command in the command prompt:

pip install virtualenv
3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
   Python syntax can be executed by writing directly in the Command Line: 
  >>> print("Hello, World!")
   Hello, World!

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
Data Types,	Examples,	Explanation
1. Strings	("Hello!", "23.34"	Text - anything between " " becomes string)
2. Integers	(5364 -	Whole numbers)
3. Floats	(3.1415 - Decimal Numbers)
4. Booleans	(True, False	- Truth values that represent Yes/No)


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
Conditional statements with the proper comparison and boolean operators allow the creation of alternate execution paths in the code. Loops allow repeated execution of the same set of statements on all the objects within a sequence. Using an index based for loop is best suited for making changes to items within a list.
The use of else statement has been restricted with the if conditional statements. But Python also allows us to use the else condition with for loops.
Python supports an else clause in for and while loops. The else body is executed only if no break is encountered during the execution of the associated loop body. In one of the scenarios where this can be quite useful is when you are searching for a particular value in the loop and the value is not found.
6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.
Python Functions is a block of statements that return the specific task. The idea is to put some commonly or repeatedly done tasks together and make a function so that instead of writing the same code again and again for different inputs, we can do the function calls to reuse code contained in it over and over again.
def add_two_num(a,b):
sum=a+b;
num1=int(input("Input the first number : "))
num2=int(input("Input the second number :"))
print("The sum of given two numbers is",add_two_num(num1.num2)

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
Both of these are tools used in the Python language, but there is a crucial difference between List and Dictionary in Python. A list refers to a collection of various index value pairs like that in the case of an array in C++. A dictionary refers to a hashed structure of various pairs of keys and values.
# Python3 code to demonstrate working of
# Convert Key-Value list Dictionary to Lists of List
# Using zip() + list comprehension

# initializing Dictionary
test_dict = {'gfg': [1, 3, 4], 'is': [7, 6], 'best': [4, 5]}

# printing original dictionary
print("The original dictionary is : " + str(test_dict))

# Convert Key-Value list Dictionary to Lists of List
# Using zip() + list comprehension
res = [ [key]+value for key, value in zip(test_dict.keys(), test_dict.values()) ]

# printing result
print("The converted list is : " + str(res))

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
Exception handling in Python is a process of resolving errors that occur in a program. This involves catching exceptions, understanding what caused them, and then responding accordingly. Exceptions are errors that occur at runtime when the program is being executed. 
try: numerator = 10 denominator = 0 result = numerator/denominator print(result) except: print("Error: Denominator cannot be 0.") finally: print("This is finally block.")
9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
 In simple terms, a module is a single file containing Python code, whereas a package is a collection of modules that are organized in a directory hierarchy.
 You need to use the import keyword along with the desired module name. When interpreter comes across an import statement, it imports the module to your current program. You can use the functions inside a module by using a dot(.) operator along with the module name.

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.
Reading line by line
Open the file1 , which has content in reading mode.
Open the file2 in writing mode.
Use for in loop to go through every line in file1 and write to file2 .
Content is written to file2 .
Close both the files.
we use the open() function to open the file in read mode (‘r’). The file is then read using the read() function, and its content is stored in the file_content variable. Finally, we print the content to the console. We have also included error handling to manage cases where the file is not found or if any other exception occurs during the execution.
# Open the file in read mode
file_path = 'sample.txt'

try:
	with open(file_path, 'r') as file:
		# Read the content of the file
		file_content = file.read()
		
		# Print the content
		print("File Content:\n", file_content)

except FileNotFoundError:
	print(f"File '{file_path}' not found.")
except Exception as e:
	print(f"An error occurred: {e}")

Steps for script that writes a list of strings to a file in python

Open a .txt file function in w mode (here w signifies write). The open() function shows the file path.
Next, create a list of items. Using a for loop to iterate through all the items in the list.
The write() function adds the list of items to the text file.
Close the file using the close() function.
# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


