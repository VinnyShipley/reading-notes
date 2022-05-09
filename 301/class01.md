# Intro to React and Components

## Component based architecture

### **What is a component?**

A component is a modular, portable, reusable piece of code that is meant to interact with other components. It has a standard form setup so that it can interface with other pieces of code.

### **What are the characteristics of a component?**

* Reusability: While usually designed so that they are modular and can be moved around to serve different purposes in different applications, sometimes they are only designed for one specific task.

* Replaceable: Components need to be able to be substituted out for different, yet similar components.

* Non-context specific: Components are designed to operate in different applications and environments.

* Extensible: A component can be extended upon from previous versions to provide new functionality.

* Encapsulated: A component depicts what it does to the caller so that it may use it's functionality, but doesn't expose how it does it under the hood.

* Independent: Components are designed to have limited need for other components.

### **What are the advantages of components?**

* Ease of deployment: As new versions of a product come out it's easier to replace with no impact to components.

* Cost: Using third-party components can free up time and resources to create other code.

* Ease of development: Components use well known interfaces that play well with a lot of systems and have defined functionality, allowing easy development across other parts of the system.

* Reusable: Because components can be reused, the cost and time needed to create code with components is greatly reduced.

* Modification of complexity: Components modifies complexity through the use of a component container and it's services.

* Reliability: Because of the DRY nature of reusing components, code is far less likely to fail with the use of components.

* Maintenance and evolution: Components are easy to change and update without affecting the whole system.

## Props and How to use them in React

### What are "props" short for?

Props are short for properties, and is used for passing data from one component to the other.

### How are props used in React?

Props are essentially thing that carries the necessary information into a React component so that it can carry out the functionality that it was designed to do.

### What is the flow of props?

Because react has a one way DOM flow, props can only flow from parent to child, not the other way around.

## Things I want to know more about

* I don't understand the point the reading is trying to make with the advantage of independence when using components.
