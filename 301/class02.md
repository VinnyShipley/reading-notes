# States and Props

**This reading stands to more deeply acquaint us with the inner workings of React, specifically when certain steps of the process happen.**

## React Lifecycle

1. **Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?** Based off the diagram, it looks like the render happens first.

2. **What is the very first thing to happen in the lifecycle of React?** The first thing that happens in the life cycle of a component is the mounting.

3. The order that the things happen are: constructor, render, React Updates, componentDidMount, componentDidUnmount

4. **What does componentDidMount do?** ComponentDidMount loads anything using a network request or a DOM initilization.

## State vs. Prop

1. **What types of things can you pass in the props?** The initial arguments to a fucntion, what you want the function to render. Something that is displayed to the user like a title or subtitle, that may or may not change.

2. **What is the big difference between props and state?** Props are brought into a component, and state is only within the component.

3. **When do we re-render our application?** When the state of that section of the application is changed.

4. **What are some examples of things that we could store in state?** Any sort of form that the user would input information, such as name, age, location, what kind of sandwiched they like. Anyting that is coming from the user and being handled by that component alone can be stored in state.
