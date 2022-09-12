# React 2

## Conditional Rendering

Conditional rendering allows you to render different content based on conditional statements. These can also be passed in as props. This can be implemented in many different ways.

## Lists and Keys

In the same way that conditional rendering can have specified circumstances when it renders elements to the page, the same can be done in terms of creating dynamic lists on a page. This is done in React first using keys to identify the thing being changed, added, or removed.

The most common way to identify keys within a list is to specify them based on their id. This ensures that they are unique from their siblings, which is the only place that matters in terms of keys being unique.

## Lifting State Up

Lifting state up is the process of keeping two instances of state in sync with each other, when they might become mutated separately at some point. This is done by setting state at the closest common ancestor point that the two variables share. This becomes the source of truth for both variables in React.

## Things I want to know more about

* I didn't really understand what they were trying to get across in the form section. I think though that as I reacquaint myself with JS it will make more sense.
