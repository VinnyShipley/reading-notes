# Class 14 Reading Notes

## What Google Learned from Trying to Create the perfect team

* Regardless of the power dynamic of a group, good ones will allow space for everyone to get their hands on the ball, so to speak. If the talking is distributed relatively evenly throughout the team, the team tends to be more successful

* Teams with a high perception of non-verbal cues and reading between the lines for each other's moods and feelings are also higher achieving teams

* Ultimately, if people feel comfortable enough to share their ideas within a group, and feel that those ideas are being heard and appreciated, the team dynamic will prosper. This starts with the smallest level team, and should spread it's mentality should apply to an entire corporation

## CSS Transforms

[A great reference for CSS](https://learn.shayhowe.com/advanced-html-css/css-transforms/)

Transforming within CSS means to change the size, position, and element itself.

* 2D Rotate: To rotate an element, select it on CSS and change the property by degrees to the degree that you want it rotated. a positive value is clockwise, negative is counter-clockwise

Ex: to rotate an element with the class of box 20 degrees clockwise

  ```
  .box1{
      transform: rotate(20deg);
  }
```

* Scale: Same as the rotate setup, but you change it based on percentage of size that it is originally

* Translate: Translate essentially pushes and pulls the element from it's original positioning without interrupting the flow of the document. Use the translateX property to change it's position on the x-axis, and translateY to do so on the y

* Skew: Skew operates on the same principle as translate, but instead of shifting the image in position, it stretches and distorts the image from it's original shape

## Transitions

Transitions allow someone to manipulate the visual transitions in their images right form CSS with no influence from JavaScript or Flash

* Transition Property: This determines what property or properties will be altered by the transition change. All of the properties within the element will be affected by the change, but only those specified by the transition property will be affected during the transition

* Transitioon Duration: Dictates how long the transition will take

## Things I want to know more about

Honestly this is the first reading that has gotten me excited about using CSS. With this reading's knowledge, there is a ton of stuff that can be done with CSS aside form how it statically looks on the page. I would like to investigate further of how these applications of CSS in a dynamic setting could create a deeper interaction with the user
