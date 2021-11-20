## Reading & writing files in Python


Today we will learn:
- what makes up a filed and why that's important in Python.
- The basics of reading and writing files in Python
- Some basic scenarios of reading and writing files.
---------------------------
## What is a file???? 

- Basically somewhere we can store our big or smal pieces of data. It's got a header (metadata about the contents of the file), the actual Data inside, and the end of the file (Specail characters). Examples of files woul be .GIF .TXT and so onnn...
------------------------------------
## File Paths
Where do you get the file from? While it may be as simple as double clicking your documents folder, you are REALLY transferring to other paths within that main file to find what  you are looking for. The file path is broken down:

 1. Folder path (The file folder location on the file system where subsequent folders are seperated by a forward slash or backslash)

2. The file name

3. and the extension of the file. (.py, .html etc...)

BELOW is a code example taken from the Real Python website:

Here’s a quick example. Let’s say you have a file located within a file structure like this:

`/
│
├── path/
|   │
│   ├── to/
│   │   └── cats.gif
│   │
│   └── dog_breeds.txt
|
└── animals.csv `

Let’s say you wanted to access the cats.gif file, and your current location was in the same folder as path. In order to access the file, you need to go through the path folder and then the to folder, finally arriving at the cats.gif file. The Folder Path is path/to/. The File Name is cats. The File Extension is .gif. So the full path is path/to/cats.gif.

--------------------------------
To access more on files and file paths click [HERE](https://realpython.com/read-write-files-python/)


 
## Exceptions vs Syntax Errors

Difference?
Syntax Errors occur when the parser detects an incorrt statement. EX:

>>> print( 0 / 0 ))
  File "<stdin>", line 1
    print( 0 / 0 ))
                  ^
SyntaxError: invalid syntax

The 3 left arrows indicate where the error was found. In this case, we have one to many parenthesis in our code! 

---------------------------
An exception error occurs whenever the syntactically correct Python code results in an error:

>>> print( 0 / 0)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ZeroDivisionError: integer division or modulo by zero

In the case above, we get a ZeroDivisionEoor returned back becuase we cannot multiple 0 by 0. We can raise our own exceptions that are bulit in to handle errors. just like try/catch!

## The AssertionError Exception
Instead of waiting for a program to crash midway, you can also start by making an assertion in Python. We assert that a certain condition is met. If this condition turns out to be True, then that is excellent! The program can continue. If the condition turns out to be False, you can have the program throw an AssertionError exception. (psst... Unit testing!!)

