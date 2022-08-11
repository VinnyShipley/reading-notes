# Automation

## Python Regular Expression

Regex is the sequence of characters used to check whether a pattern exists.

### Useful Regex functions

* compile() creates a pattern object that can then be used to search for a match inside different tags with match() or search()

* search() scans through ths string looking for the fist location where the regex pattern produces a match

* findall() finds all the instances off the regex expression

* sub(pattern, repl, string) returns a the string that is the result of the leftmost non-overlapping occurrences of pattern in string by the replacement repl

* split() for search and replace

### To Use

1. Import re

2. Create a phrase for regex to look for

3. Find a text to check the regex phrase against

4. Use a regex function on the test

### Useful site to construct regex sites

[Regex 101](https://regex101.com/)

## shutil - High Level File Operations

shutil is a module that helps in the automating process of copying and removing of files and directories

### Copying Files

* copyfile() copies the contents of the source to the destination  and raises IOError if it does not have permission to write to the destination file

* copytree() recurses through the directory tree, copying files to the destination. The destination directory cannot exist in advance

* which() scans a search path looking for a named file
