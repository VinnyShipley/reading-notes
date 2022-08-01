# Data Analysis

## What is Jupyter

[Jupyter Cheat Sheet](https://www.edureka.co/blog/wp-content/uploads/2018/10/Jupyter_Notebook_CheatSheet_Edureka.pdf)

Jupyter is an platform in which you can easily display information. The way that it is displayed runs through markdown, and can be rendered in site.

It runs in two modes, command and edit. In command you can edit the layout of the cells that make up Jupyter, essentially giving you the ability to change the framework of your Jupyter notebook.

In edit mode, you can edit the contents of the cells in the markdown language. When editing, you link the project to a specific shell, which is projects wide and remembers variable values across the project.

## NumPy

### What is NumPy

[NumPy cheat sheet](https://s3.amazonaws.com/dq-blog-files/numpy-cheat-sheet.pdf)

NumPy is a commonly used Python data analysis package that helps with math related functionality.

When dealing with matrices in NumPy, all the elements of the array have to be of the same type to be processed

### To create an array with Numpy

1. Import numpy
2. Pass the list to be analyzed into numpy with whatever function you would like to use to manipulate the information. When passing the information in, make sure you omit header rows that aren't the same data type as the rest of the data. For the same reason, make sure that you convert all of the data to be analyzed by numpy to be the same data type. Change and examine what data type numpy is using by accessing the dtype variable

This process will create an array of the passed in data, that you can then manipulate further.

## To access values from numpy created tables

Numpy creates tables that are in a zero index system, meaning that the index for the first index and column are both 0.

Accessing a value at the third row and the fourth column would be coded like this:

    name_of_numpy_list[2,4]

Slicing a NumPy array:

If we wanted to just get the first three elements from the fourth column of the same list above, the code would look like this:

    name_of_numpy_list[0:3,3]

This slicing counts from and includes the number to the left of the colon, and counts up to and doesn't include the number on the right side of the colon.

The slicing for the most part behaves like it does in vanilla python.

## Assigning values to certain elements in arrays

Simply target the element you wish to target by giving its specific index position, and then use = to assign a value to that cell. This can also be done with entire rows or columns in the same fashion, it is all dependent on how specific you are when targeting the element or collection of elements.

Dealing with multi-dimensional arrays is simply a matter of targeting the correct value in the correct group. Whether that group has subgroups is a matter of how multi-dimensional the array is.

### Array operations

If you access a series of elements with numpy, and then give a basic math operator, that operation will apply to every element selected. This won't change the original array, it will simply return a new array displaying the new values of the elements selected once they have been operated upon.

While you can do this with simply numbers (manipulating all the elements of an array by a static number) you can also swap out that static value with another set of elements from another array.

    wines[:,10] * wines[:,11]

The code above would multiply all the rows from the 10th column with all the rows from the 11th column. Note that this can only work when each group of elected elements are the same size.

### Broadcasting

If the arrays being operated with each other are noth the same size, broadcasting takes place. Broadcasting takes these steps:

* The last dimension of the arrays are compared.

    * If the dimension lengths are equal, or one of the dimesnsions are equal (which would mean all of the cells in the last position of the other collection of cells would be multiplied by this specific cell), then we keep going

    * Otherwise, an error is raised

### NumPy Array methods

* Sum method

    * By using the .sum() method on a set of cells already passed through numpy, adding the .sum() method to the end of it will sum all of the cells specified

* Mean method

    * Finds the mean value of all specified cells passed into numpy

* Std method
    
    * Finds the standard deviation of all specified cells passed into numpy

* Min method
    
    * Finds the minimum value of all specified cells passed into numpy

* Max method
    
    * Finds the maximum value of all specified cells passed into numpy

### Comparison Operators

By using comparison operators in the same method as the operator methods, you can get a list of boolean values back denoting whether the value in that list is true given that comparison operator.

### Subsetting 

By placing the comparison operator shown above in a new list of it's own, instead of getting back a list of boolean values, you will get back a set of those values that would return as true.
