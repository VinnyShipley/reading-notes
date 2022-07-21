# Classes and Objects

## Classes and Objects

**Objects:** An encapsulation of cariables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially the template with which to build objects

**Creating a Class:** 

    class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")
    myobjectx = MyClass()

This code block has created an object called myobjectx. From there you can access both the function and variable stored within it by citing it with dot notation. To access and print the variable:

    print(myobjectx.variable)

**To create multiple objects and then manipulate individual properties of those objects**:

    class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")
    
    myobjectx = MyClass()
    myobjecty = MyClass()
    
    myobjecty.variable = "yackity"

This would change the value of the variable variable in myobjecty into yackity, while keeping myobjectx as blah

**Accessing an objects functions:** Using the same code as above, you would access the function function within myobjectx as:

    myobjectx.function()

**Init functions** 

Init functions exist as essentially the constructor for the class, with the self variable acting in a similar way to the this in constructors in JavaScript. For example, the init function for the MyClass class would be:

    class MyClass:
      def __init__(self, function)
      def self.function = print('This is a message inside the class')

## Recursivity

**Recursion:** A recursive function is a function that can be defined in terms of itself via self reference. The function will continue to call itself until some condition is met. Example a factorial function, that is recursive:

    def factorial_recursive(n):
    # Base case: 1! = 1
    if n == 1:
        return 1

    # Recursive case: n! = n * (n-1)!
    else:
        return n * factorial_recursive(n-1)

**Maintaining State** 

Each recursive call has its own execution context, so to maintain that context through each loop you need to either:

* Thread that state through each recursive call so that state is part od the current call's execution

* Keep the scope global

Threading it essentially means having a constant function checking to see if some condition is being satisfied, whereas global simply has a variable to check against that is established globally within the function

## Pytest Fixtures and Coverage

**Fixtures:** Fixtures are objects that are shared across multiple tests to make testing easier. Ex:

    @pytest.fixture
    def simple_file():
       return StringIO('\n'.join(['abc', 'def', 'ghi', 'jkl']))

This code block can then be used across the test suite by referencing simple_file

**Scope:** to control the scope of the fixture, or where it can be accessed, include scope='whatever the scope is that you would like it to be included in' in parentheses after @pytest.fixture

**Coverage:** Coverage essentially lets you know where the bugs are in your code, specifically where you are telling it to look. To set it up:

    pytest --cov = the_function_to_test

This sets up the function that you would like to test

    coverage html

This puts it in the form of html on your page so the error report is readable. By then checking the index.html of the directory, you are able to see the points in the function that the test is being failed. 