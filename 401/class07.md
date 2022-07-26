# Ten Thousand 2

## Python Scope

### Global Statement

You can manipulate what is a global variable in Python with the global statement. Ex: 

    def function():
      global variable_name

The code above demonstrates the use of the global statement, which now makes the variable variable_name accessible across the entire module.

Generally, it isn't good practice to use the global statement, as it can get unwieldy quick. If for example, that global variable is created in a function, but that function hasn't been called at a point where you need the global variable,, you will run into a NameError, and crash the program

### Things I want to know more about 

* I don't understand why the non-local statement is necessary. It seems like it simply accesses a variable that in a high level of scope, which I though was possible without the use of the non-local statement
