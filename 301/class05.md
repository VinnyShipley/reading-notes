# Putting it all together

## Thinking in React

1. **What is the single responsibility principle and how does it apply to components?** The single use responsibility principle is the idea that each component should ideally just be doing one thing. If it grows to be bigger than one, the component should be refactored so it only does one again.

2. **What does it mean to build a ‘static’ version of your application?** A static version of an app is one that displays the data one would expect to see on the app, but none of the data is dynamic. In other words, state does not exist, and everything is hardcoded. 

3. **Once you have a static application, what do you need to add?** You need to figure out the minimal amount of state that your app needs to compute all the data points that you want to render onto the page. Once you have that in your head or on a whiteboard, build it.

4. **What are the three questions you can ask to determine if something is state?** If it is passed from the parent in a state, remains unchanged over time, or if it is computed based on any other state or props in that same component, then it isn't a state. 

5. **How can you identify where state needs to live?** Identify which components render something based on that state, find the common ancestor of all of those components. Ideally this common ancestor is where the state should live. If that ancestor doesn't make sense, create a new component with the sole purpose of housing that state.

## Higher order functions

1. **What is a “higher-order function”?** They are either functions that take in other functions as arguments, or return them.

2. **Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?** Line two is setting up the function of greaterThan10 so that when two arguments are passed into that function, it checks if the value in the most nested parentheses is smaller than the one immeadiately to the left of it. Essentially it is acting as almost a callback function for greaterThan10.

3. **Explain how either map or reduce operates, with regards to higher-order functions.** The map function is a relatively simple function, just iterating through every value in an array, and what this means for higher order functions is that it's a relatively simple process to take the result of that functions, or even just parse the entire function itself into another higher function, to then further manipulate the data being iterated through.