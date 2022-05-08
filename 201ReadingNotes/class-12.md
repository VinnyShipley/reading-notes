# Chart.js and Canvas

## Charts

Charts are a good way to display data on your webpage, as they convey the information quickly, but are hard to build.

**Building a Table**

* Download [Chart.js](https://github.com/chartjs/Chart.js) and unzip it into the directory you'll be working with

**Drawing a Line Chart**

* To draw a line chart, create a cnavas element in html that the chart will live. Do this with the ```<canvas>``` element, with the attributes ```<id> <width> <height>```
  * Then connect that canvas to the script you will write for the chart in JavaScript, the linking of which looks like this 
  ```  
  <script>
      var buyers = document.getElementById('buyers').getContext('2d');
      new Chart(buyers).Line(buyerData); </script>```

* When filling in the chart on th Java side of things, use an array to indicate the labels of the line chart, and an object to indicate the cell data as well as the styling elements of the cells.

**Drawing a Pie Chart**

* To write a pie chart you also need to create a canvas for the chart to live

* Upon linking it to Java, you simply need to give a percentage value and a color values to all the elements within the pie chart

* After that you add the options that remove the stroke from the segments, as well as animate the scale so that it zooms out from nothing

**Drawing a Bar Chart**

* Again, start with a canvas and link it to the js file

* The process is similar then to the line graph

## Basic Uses of the Canvas Element

The canvas element creates a 2D context for charts to exist on a webpage

* By default the canvas is 300 px wide and 150 px high, but can be changed within the tag with attributes

* By  rendering a fallback image within the canvas tag, you can give browsers who don't support the canvas tag something to display where the chart would have. This is simply done by placing an ```<img>``` within the bounds of the canvas opening and closing tags

* Link the canvas to the js file that will manipulate it with the id attribute within the canvas tag, and DOM manipulation

* You can also build fallback material within the js file with an if else loop, the if checking to see if the browser has the ```getContext()``` method at which point the code of the table will run, the else being if it is unsupported

## Drawing Shapes with Canvas

* The Grid: To manipulate the grid of the canvas, you need to understand the grid of the canvas. The top left corner of the grid is point (0,0), and if you create a new origin for a shape within the grid, that is where the top left corner of that image will render

* Only the primitive shapes rectangles and paths are natively supported in canvas, the rest have to be drawn by coordinate

* To build a rectangle, simply create one of the following objects within the draw function ties to your canvas clearRect, fillRect, or strokeRect, followed by the starting point, the height and the width

* For non-native shapes, you have to use draw paths the can then be filled in

  * This is done by giving a starting coordinate of the shape, giving it it coordinates to the arc, line, or simply move to if you don't want there to be a connecting line between the point, and then fill the shape in if so desired

## Applying Styles and Colors to Canvas

* fillStyle:
  * Sets the style when filling shapes

* strokeStyle:
  * Sets the shape outlines

## Things I want to know more about

* I feel like the bar chart explanation wasn't super well explained, and I would like to know more about that process.
