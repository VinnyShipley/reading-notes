# Ten Thousand 3

## List Comprehension

### List comprehension is a quick way to build a list in Python. Ex:

    digits = [x for x in range(10)]

Using the code above as the example, the first x is the number that is being iterated through, the second x represents each item the list created by the range method. A list of 0-9 with a step of 1 now populates the digits list

### Using a loop with list comprehension

By looping through a range, you can quickly iterate through a range and manipulate the values contained, and then append those values to the list. Ex:

    squares = []

    for x in range(10):
      # raise x to the power of 2
      squares.append(x**2)

Printing the squares list would display the squares of all the digits between 0 and 9.

### Multiplying parts of a list

To have a modifier only be present on part of the list, you can apply a filter, this can be done with an if statement. For example, to print out the even numbers between 1 and 20:

    even_numbers = [ x for x in range(1,20) if x % 2 == 0]

### Showing the first letter of each word using Python

    authors = ["Ernest Hemingway","Langston Hughes","Frank Herbert","Toni Morrison",
    "Emily Dickson","Stephen King"]

    letters = [ name[0] for name in authors ]
    print(letters)

Breaking down the code above, the list authors is populated with the names of authors. In letters, the second name is showing how the elements in authors will be manipulated. The name[0] is referring to how that manipulated second name will be displayed in the list, or rather, what part of the element will be displayed. This can also be used when trying to uppercase and lowercase or also with the filtering method described in the multiplication section.

[Code block examples](https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)
