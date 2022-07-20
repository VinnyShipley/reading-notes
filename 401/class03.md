# FileIO and Exceptions

## Reading and Writing Files in Python

To reference a file in python to ultimately open it or manipulate it, you simply need to write out the relative path for the file. When printed, the file will also have line endings embedded within it (noted as \r\n with different variations based on the operating system).

## Opening and Closing a Document

To open a file in python, use the built in command open(), and then include the filename in the open function. Store this action in a variable so you can later close it.

Ex: new_file = open('this_is_a_file_name.txt')

Once open, manipulate or read the document, and then close the document with the following code, in reference to the above opening opening code.

Ex: new_file.close()

You can also open a file with a with statement, shown  below:

Ex: with open('this_is_a_file_name.txt', 'r') as reader:

### Commonly used characters for action on files:

* r = opens the file for reading (the default action)
* w = opens the file for writing, which overwrites the original file
* rb or wb = opens the file in binary mode

## Reading a File

* .read(size=x) will read from the file based on the number of bytes specified by size. If the value of size is left blank the entire document will be read.

* .readline(size=-1) reads at most the number (specified by size) of characters from the line. This continues on to the end of the line and then wraps back around. If no size is given the entire line is read.

* .readlines() reads the remaining lines from the file and returns them as a list.

**Important Note** 

These functions can be used in loops to achieve different ends

## Writing into a file

* .write(string) writes the string to the file

* .writelines(seq) write the sequence to the file. Keep in mind that no line endings are automatically added to the end of lines, and will need to be included in the sequence

## Python Exceptions

**Exception Errors:** A type of error that occurs when syntactically correct python runs into an error. This error is raised by the program to fire on a specific condition.

**Asserting Exceptions:** Because assertions will stop the code if their conditions are falsey, you can put the condition within the assertion to make sure that the code will not run if the condition is not true.

**Try and Except:** By using a try and except pair, you can setup up a state where if the assertion is false and in the try section of the code block, instead of crashing the entire program, you can instead create an error message in the except section to be displayed.

**Else Clause:** This will fire if no exceptions were fired during the program.

**Finally:** Will fire at the end of the program regardless of if any exceptions were triggered during the program.
