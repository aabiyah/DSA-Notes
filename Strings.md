## What is a String?

A **String** is considered a data type in general and is typically represented as arrays of bytes (or words) that store a sequence of characters. A string is defined as an array of characters. The difference between a character array and a string is that a string is terminated with a special character `\0`. Some examples of strings are: `"geeks"`, `"for"`, `"geeks"`, `"GeeksforGeeks"`, `"Geeks for Geeks"`, `"123Geeks"`, `"@123 Geeks"`.

## String Data Type

In most programming languages, strings are treated as a distinct data type. This means that strings have their own set of operations and properties. They can be declared and manipulated using specific string-related functions and methods.

> **Note:** In some languages, strings are implemented as arrays of characters, making them a derived data type.

## String Operations

Strings support a wide range of operations, including concatenation, substring extraction, length calculation, and more. These operations allow developers to manipulate and process string data efficiently.

Below are fundamental operations commonly performed on strings in programming:

- **Concatenation:** Combining two strings to create a new string.
- **Length:** Determining the number of characters in a string.
- **Access:** Accessing individual characters in a string by index.
- **Substring:** Extracting a portion of a string.
- **Comparison:** Comparing two strings to check for equality or order.
- **Search:** Finding the position of a specific substring within a string.
- **Modification:** Changing or replacing characters within a string.

## Applications of String

- **Text Processing:** Strings are extensively used for text processing tasks such as searching, manipulating, and analyzing textual data.
- **Data Representation:** Strings are fundamental for representing and manipulating data in formats like JSON, XML, and CSV.
- **Encryption and Hashing:** Strings are commonly used in encryption and hashing algorithms to secure sensitive data and ensure data integrity.
- **Database Operations:** Strings are essential for working with databases, including storing and querying text-based data.
- **Web Development:** Strings are utilized in web development for constructing URLs, handling form data, processing input from web forms, and generating dynamic content.

# Syntax of String Data Type in Python

```
string_variable = 'Hello, world!'
```

### Example of String Data Type in Python
```
string_0 = "A Computer Science portal for geeks"
print(string_0)
print(type(string_0))

Output:
A Computer Science portal for geeks
<class 'str'>
```

### Creating a String in Python

Strings in Python can be created using single quotes, double quotes, or even triple quotes. Below are examples demonstrating different ways to create a Python string.

```
# Creating a String with single Quotes
String1 = 'Welcome to the Geeks World'
print("String with the use of Single Quotes: ")
print(String1)

# Creating a String with double Quotes
String1 = "I'm a Geek"
print("\nString with the use of Double Quotes: ")
print(String1)

# Creating a String with triple Quotes
String1 = '''I'm a Geek and I live in a world of "Geeks"'''
print("\nString with the use of Triple Quotes: ")
print(String1)

# Creating a multiline String with triple Quotes
String1 = '''Geeks
            For
            Life'''
print("\nCreating a multiline String: ")
print(String1)

Output:
String with the use of Single Quotes: 
Welcome to the Geeks World
String with the use of Double Quotes: 
I'm a Geek
String with the use of Triple Quotes: 
I'm a Geek and I live in a world of "Geeks"
Creating a multiline String: 
Geeks
            For
            Life
```

### Accessing Characters in Python String

In Python, individual characters of a string can be accessed using the method of Indexing. Indexing allows negative address references to access characters from the back of the string, e.g., -1 refers to the last character, -2 refers to the second last character, and so on.

#### Positive Indexing Example
```
String1 = "GeeksForGeeks"
print("Initial String: ", String1)

# Printing First character
print("First character of String is: ", String1[0])

Output: 
Initial String:  GeeksForGeeks
First character of String is:  G

```

#### Negative Indexing Example

```
String1 = "GeeksForGeeks"
print("Initial String: ", String1)

# Printing Last character
print("Last character of String is: ", String1[-3])

Output:
Initial String:  GeeksForGeeks
Last character of String is:  e
```

#### String Slicing in Python

String slicing is used to access a range of characters in the string. Slicing in a string is done using a slicing operator, i.e., a colon :. The string returned after slicing includes the character at the start index but not the character at the last index.

```
# Creating a String
String1 = "GeeksForGeeks"
print("Initial String: ")
print(String1)

# Printing 3rd to 12th character
print("\nSlicing characters from 3-12: ")
print(String1[3:12])

# Printing characters between 3rd and 2nd last character
print("\nSlicing characters between 3rd and 2nd last character: ")
print(String1[3:-2])

Output:
Initial String: 
GeeksForGeeks
Slicing characters from 3-12: 
ksForGeek
Slicing characters between 3rd and 2nd last character: 
ksForGee
```

#### Reversing a String in Python

By accessing characters from a string, we can also reverse strings in Python.

Example of Reversing a String
```
# Program to reverse a string
gfg = "geeksforgeeks"
print(gfg[::-1])
  
Output:
skeegrofskeeg
```

### Built-In Reverse Function in Python
We can also reverse a string using the built-in reversed() function.

```
# Program to reverse a string
gfg = "geeksforgeeks"

# Reverse the string using reversed and join function
gfg = "".join(reversed(gfg))

print(gfg)

Output:
skeegrofskeeg
```

### Deleting/Updating from a String

In Python, updating or deleting characters from a string is not allowed because strings are immutable. However, deletion of the entire string is possible using the del keyword.

Updating a Character
To update a character in a string, you can first convert the string into a list, update the element, and then convert it back into a string. Another method is using string slicing.

Example:
```
# Python Program to Update a character of a String

String1 = "Hello, I'm a Geek"
print("Initial String: ")
print(String1)

# Updating a character of the String
## Method 1: Converting to List and then back to String
list1 = list(String1)
list1[2] = 'p'
String2 = ''.join(list1)
print("\nUpdating character at 2nd Index: ")
print(String2)

## Method 2: Using String Slicing
String3 = String1[0:2] + 'p' + String1[3:]
print(String3)

Output:
Initial String: 
Hello, I'm a Geek
Updating character at 2nd Index: 
Heplo, I'm a Geek
Heplo, I'm a Geek
```

### Updating Entire String

```# Python Program to Update entire String

String1 = "Hello, I'm a Geek"
print("Initial String: ")
print(String1)

# Updating a String
String1 = "Welcome to the Geek World"
print("\nUpdated String: ")
print(String1)

Output:
Initial String: 
Hello, I'm a Geek
Updated String: 
Welcome to the Geek World
```

### Deleting a Character
Attempting to delete a character from a string will cause an error.

Example:
```
# Python Program to delete a character of a String

String1 = "Hello, I'm a Geek"
print("Initial String: ")
print(String1)

print("Deleting character at 2nd Index: ")
del String1[2]
print(String1)

Output:
Initial String: 
Hello, I'm a Geek
Deleting character at 2nd Index: 
Traceback (most recent call last):
  File "e:\GFG\Python codes\Codes\demo.py", line 9, in <module>
    del String1[2]
TypeError: 'str' object doesn't support item deletion
```

### Deleting Entire String

```
String1 = "Hello, I'm a Geek"
print("Initial String: ")
print(String1)

# Deleting a String with the use of del
del String1
print("\nDeleting entire String: ")
print(String1)

Output:
Traceback (most recent call last): 
File "/home/e4b8f2170f140da99d2fe57d9d8c6a94.py", line 12, in 
print(String1) 
NameError: name 'String1' is not defined 
```

Explanation: In the above example, after deleting String1, when we tried to print it, we got an error stating that String1 is not defined because the string was deleted and does not exist.

### Escape Sequences in Python
While printing strings with single and double quotes, use the backslash (\) escape character to avoid errors. The escape character is followed by the character you want to insert.

Examples:
```
# Python Program for Escape Sequence in String

# Initial String
String1 = '''I'm a "Geek"'''
print("Initial String with use of Triple Quotes: ")
print(String1)

# Escaping Single Quote
String1 = 'I\'m a "Geek"'
print("\nEscaping Single Quote: ")
print(String1)

# Escaping Double Quotes
String1 = "I'm a \"Geek\""
print("\nEscaping Double Quotes: ")
print(String1)

# Printing Paths with the use of Escape Sequences
String1 = "C:\\Python\\Geeks\\"
print("\nEscaping Backslashes: ")
print(String1)

Output:
Initial String with use of Triple Quotes: 
I'm a "Geek"
Escaping Single Quote: 
I'm a "Geek"
Escaping Double Quotes: 
I'm a "Geek"
Escaping Backslashes: 
C:\Python\Geeks\
```
