# Problem Domain, Objects, and the DOM

## Understanding Problem Domain

A problem domain is the scope and focus of a problem. In terms of writing code, a problem domain is the feature that the code needs to do. By focusing on understanding your problem domain early on in the process of working on a bug or a feature, you can more efficiently and effectively tackle problems.

## Primitive Values vs. Object References in JavaScript

* **Value vs. Value Reference**
  * let foo = 'bar' is an example of the variable foo being assigned a value directly.

  * When a variable is instead assigned with an object, it instead instead has references to other values stored in it.

  Example:

let = Moe {

      name: 'Moe';
      occupation: 'bartender';
      voiceActor: 'Hank Azaria';
     }

These values have been stored to the variable 'Moe' relatively. within the object linked to the value of 'Moe'.

* **Mutable vs. Unmutable Values**

Mutable simply means that the value is able to be changed or mutated. Primitive values are immutable values, which means that they cannot be changed if they are assigned with the const declaration. If they are assigned with the let variable, that value as a whole cannot be changed, but not the individual values within that value.

Mutable values on the other hand have some leniency with what can be changed within the value. If you create and array, you can change the individual values within that array. This is due to the fact that arrays are actually just special objects in JavaScript

* **Primitive Value and object Relativity in Relation to Equality Comparisons**

Primitive values exist how you would logically expect with equality comparisons, checking to see if the values match up between the variables.

Contesnts do not equal the location of the value within  onjects. This is why if you create a check like [] === [], the value will come back as false. Even if the alues are the same, they are stored in different places. However, if you create a duplicate reference to the same object, then the object location will match each other and come back as true if logged.

## Object Literals

Within an object variables become properties, and functions become methods. These properties and methods have a name and a value, this value is called a key. Two keys cannot exist with the same name. The value of a property can be a string, a number, a boolean, array, or even another object. The value of a method is always a function.

## DOM Trees

The DOM tree is a model of a webpage that the browser first creates when it see the page for the first time. This tree is made up of four types of nodes.

**Node Types**

1. Document Node
    * The starting point of the DOM tree, this node is added and contains all the other nodes inside of it. This is the starting point for all visits to the DOM tree

2. Element Nodes
    * This node describes the structure of the HTML page. As it looks down the tree, it looks for elements and then goes within those elements to see what content to display on the page.

3. Attribute Node
    * If the element has an attribute attached to it, it also has an attribute node attached to it. This tells JavaScript to treat the element with this attached node to behave differently than an elements of the same kind without it. What it does depends on the attribute type

4. Text Node
    * Text nodes cannot have children, so they are always the end of their specific branch. If a text node has children elements, they are not children of that text branch, they are instead children of the containing element.

**Selecting Individual Nodes**

There are a couple ways to select specific elements within the DOM tree

1. getElementById()
   * uses the value of the element's id attribute, which should be unique within the page

2. querySelector()
    * Uses a CSS selector, and returns the first matching element

**Selecting Multiple Nodes**

1. getElementByClassName()
    * Selects all elements that have that specific value for the class attribute

2. getElementsByTagName()
    * Selects all the elements that have that specified tag name

3. querySelectorAll()
    * Uses a CSS selector to select all matching elements

## Things I Want To Know More About

* I'm still a little shaky on the equality of the variables being different when they are stored in objects

* Accessing things in the DOM tree is a really new concept to me, and I think I am going to need to see it in practice to really understand what is going on. 
