# ANSWERS
## Question 1
- Python is a high-level general-purpose programming language. It is versatile and readable. It is interpreted language i.e. it is directly executed by the interpreter.
### Python key features that make it popular
- READABILITY - Python uses a simple syntax that is easy to read and understand even for beginners.
- VERSATILE - Python can be used in many places to perform different tasks, i.e. it can be used in web development, it can be used in data science even in automation and writing tests for programs.
- COMMUNITY SUPPORT - It has a large community of users who offer support through documentation
- Extensible - Python has a large number of modules that can be added to enhance its code usability and operation.
- OPEN SOURCE - it is open source allowing people to use it for free, and also allow other developers to contribute to it thus ensuring its performance
### use cases
- DATA SCIENCE - Python has libraries such as pandas and matplotlib that are greatly used for data science.
- WEB DEVELOPMENT - Python has frameworks such as Django and Flask which allow developers to create robust web applications.
- MACHINE LEARNING -  Python has libraries such as PyTorch which is used in machine learning
- AUTOMATION AND SCRIPTING - python is used in writing scripts and doing automations.
## Question 2
- ### Installing Python on Windows
- Open the Microsoft Store search for Python as shown below and choose the Python version of your preference.
 ![image](https://github.com/Powerlearnproject/se-assignment-6-introduction-to-python-stoicdavi/assets/117593948/1ecfcd0f-be44-4a3c-967c-8f4606b60e6d)
- then click the get button, and the Python version you have selected will download and install itself on your machine. NB: MAKE SURE YOU ARE CONNECTED TO THE INTERNET
### To verify the installation
- open your command prompt and type in the following command
- python --version
- You may need to restart your PC if this command doesn't work
## Question 3
- print("Hello, World!")
- A simple Python code to print Hello, World! to the console.
- We use the print function to print on the console. Print is a Python inbuilt function that allows user to display/output their data on the console
## Question 4
- DATA TYPE - this is the type of value that a variable can store
- VARIABLE - a container used to store a data value
  ### Numeric data type
- integer(int) -  this represents the positive or negative whole numbers, zero included
- floats(float) - these are real numbers with decimal points
- complex numbers -  these are numbers that appear in the +bj where a and b are either integers or floats
### Boolean(bool) Data type
- Represents logical values ie true or false
### String(str) datatyoe
- This is made up of letter numbers or special characters that are enclosed inside double or single or triple quotes
### None data type
- Used to represent an empty container, it shows that a variable is yet to be assigned a value.
### Scripts to show how data types are used
- Create variables of different data types
- integer_variable = 10  # Integer
- float_variable = 4.14  # Float
- complex_variable = 1j  # Complex number
- string_variable = "Hello, World!"  # String
- boolean_variable = True  # Boolean
- none_variable = None  # None

- # Print the data type of each variable
- print(type(integer_variable))  # <class 'int'>
- print(type(float_variable))  # <class 'float'>
- print(type(complex_variable))  # <class 'complex'>
- print(type(string_variable))  # <class 'str'>
- print(type(boolean_variable))  # <class 'bool'>
- print(type(none_variable))  # <class 'NoneType'>

- # Perform operations and print the results
- sum_result = integer_variable + float_variable  # Adding an integer and a float
- print("Sum:", sum_result)  # Sum: 14.14

- string_concatenation = string_variable + " - Python Script"  # Concatenating strings
- print("Concatenated String:", string_concatenation)  # Concatenated String: Hello, World! - Python Script
## Question 5
- Conditional statements and loops come in handy when writing programs as they allow programmers to control the flow of execution of a program.
  - # Conditional statements
  - They allow programmers to execute different blocks of code as long as a given condition is met.
  - A simple if....else statement
  - if age >= 18 and country == 'Kenya':
  - print('You are eligible to vote')
  - else:
  - print("you are not legible to vote")
  - This program checks whether a user is 18 years and above and if he/she is also from Kenya.
  - If a user meets these two conditions, a message is printed that they are eligible to vote. If these two conditions are not met, the message 'you are not eligible to vote' is printed on the console
  - # loops
  - They help us as programmers when writing codes to execute a block of code repeatedly until a certain condition is met.
  - for loop statement that prints from 1 - 10
  - for i in range(1, 10):
  - print(i)
  - this program prints numbers starting from 1 to 10 and breaks the loop once this condition is met
 
# Question 6
## Python functions
- Function in Python is a block of reusable code that performs a specific task
- def add_numbers(x, y): # add_number funtion that takes two parameters as input
 -   """
 -   Add two numbers and return the result.
 -   """
  -  return x + y
  - # usage 
- num1 = 8 # variable num1 store value 8
- num2 = 7  # variable num2 store value 7
- result = add_numbers(num1, num2)
- print(f"The sum of {num1} and {num2} = {result}")
- this will print out 'The sum of 8 and 7 = 15
- f is a Python string format specifier.

## Question 7
### Lists and dictionaries
- Lists - They are ordered collections of elements. all elements in a list are indexed, starting from 0 - nth index
- Lists are created using the square brackets e.g names = [] or the list() function e.g names = list(). This initializes an empty list called names.
- Dictionaries - They are unordered collections of key-value pairs. They are not indexed, a key identifies a value.
  - ### Creating a simple list and a dictionary
 - numbers = [20,40, 50, 22]
 - this is a list that contains integer data type
 - to print this list - print(numbers)
 - to print the first element of the list - print(numbers[0])
 - 0 is the index of the first element in the list.
- Dictionary
- dictionary is created using curly braces{} eg grades = {} or the dict() function grades = dict() this creates an empty dictionary called grades.
- grades = {'English: 'A', 'Kiswahili': 'B+', 'Math': 'A-'}
- this is a dictionary that has the subject names as the keys and the grades as their values
- to print this dictionary - print(grades)
- to access a specific value you can print(grades['Math']) this will print out the grade for math. If you want that for English just change the name in the square brackets to English.

## QUESTION 8
### exeption handling
- It allows us to handle and manage them when they occur in Python during program execution.
- TRY Block-  We place a code that is likely to cause an exception inside the try block. if an exception occurs in this block, the execution jumps to the corresponding except block
- EXCEPT block this block catches exceptions and specifies how to handle them.
- FINALLY - The code inside this block executes whether or not an exception occurred
- def divide(a, b):
    try:
        result = a / b
    except ZeroDivisionError:
        print("Error: Cannot divide by zero!")
    else:
        print(f"Result: {result}")
    finally:
        print("Cleanup: Closing resources or performing other tasks.")

### Example usage
numerator = 10
denominator = 0

divide(numerator, denominator)
- "Error: cannot divide by zero!' will be printed
- Explanation
- We attempt to divide the numerator by denominator.
- If ZeroDivisionError occurs (i.e., dividing by zero), the except block handles it by printing an error message.
- If no exception occurs, the else block prints the result.
- The final block ensures that cleanup tasks (like closing files or releasing resources) are executed regardless of exceptions.


## Question 9
### Python modules and packages
- a module is a self-contained unit of code that can be imported and used in other programs or modules
- It allows us to allows us to organize our programs into small and manageable pieces of code
- PACKAGES - These are groups of related modules organized in one directory. They allow us to group several different modules under a single name.
- ### importing and using math modules
- import math
- number = 16
- sqrt_num = math.sqrt(number)
- print(f'The square root of {number} = {sqrt_num}')
- this will output 'The square root of 16 is 4'
- we can import specific functions from the math module as shown below
- from math import pi
- we can also import math as an alias as shown below
- import math as m
- after importing it as m we can use it as shown
- m.sqrt(16) # This will return the square root of 16 which is 4
## Question 10 
### File I/O
- we can directly open a specified file as shown below
- file = open('readme.txt', 'w')
- data = file.write('hello')
- file.close()
- - with this file-handling method, we have to close a file now and then
- It is recommended to use context manager to open Python files as shown below
- with open('readme.txt', 'w') as file: # opening file in write mode
-    file.write("Hello David") # This statement will replace file data with the 'Hello David' string
  - This will also create the file if it does not exist. When using this method to open files, we don't need to close them as they are automatically closed when we finish working with them.
  - let us now open the file in the read mode
  - with open('readme.txt', 'r') as file:
  -   data = file.read()
  -   print(data)
  - this will open the file, read the data that we wrote inside print it, and then close the file once it is done. we don't have to use file.close() as in the first place above
  - #### NB: you should always remember to close a file when you open it. You can avoid this by using the 'with' keyword as the files are automatically closed when you finish your operations on it
  - 
## REFERENCES
- https://www.geeksforgeeks.org/difference-between-list-and-dictionary-in-python/
- https://www.scaler.com/topics/difference-between-list-and-dictionary-in-python/
- https://www.geeksforgeeks.org/python-exception-handling/
- https://realpython.com/python-math-module/
