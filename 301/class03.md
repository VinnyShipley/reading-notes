# Passing Functions as Props

This reading is essentially to get the reader more comfortable with spread operators, and general React thinking.

## Lists and Keys

1. **What does .map() return?** .map() returns an array of the same size as the one that is passed into it, even if some of the values within the array are undefined.

2. **If I want to loop through an array and display each value in JSX, how do I do that in React?** the best way to do this is to create a variable that is equal to the array.map, and then map that array. From there convert the values that are stored within that value into li by placing that rendered variable within curly braces.

3. **Each list item needs a unique what?** Key

4. **What is the purpose of a key?** Keys identify the variables that have changed added, or that have been removed

## Spread Operator

1. **What is the spread operator?** The spread operator expands the iterable objects within a array into a list of arguments.

2. **List 4 things that the spread operator can do.** It can copy an array, it can use math functions on each part of the array, it can add a item in an array to a list, and it can add certain items in an array to a states in React. 

3. **Give an example of using the spread operator to combine two arrays.** if the first array was named array1 and the second was named array2, to combine you would simply type ...[array1, array2]

4. **Give an example of using the spread operator to add a new item to an array.** With the same array setup, it would be newArray = [value, value2, ...array1]

5. **Give an example of using the spread operator to combine two objects into one.** It's the same as previously, simply refer to the object instead of a variable or an array

## Passing Functions between Components

1. **In the video, what is the first step that the developer does to pass functions between components?** They create the function near the component that they want the function to manipulate.

2. **In your own words, what does the increment function do?** The increment function adds 1 to the value of the count variable of whatever instance of people is clicked.

3. **How can you pass a method from a parent component into a child component?** With props

4. **How does the child component invoke a method that was passed to it from a parent component?** It can access it by accessing this.props.insertWhateverComponentYouWantImportedHere because by accessing props you are accessing whatever the props is bringing between components.
