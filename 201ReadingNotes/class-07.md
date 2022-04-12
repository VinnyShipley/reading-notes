# Object-Oriented Programming, HTML Tables

## Domain Modeling

Domain Modeling is the process of creating a conceptual model in code for a specific problem. The long and short of making a domain model is to build self-conained objects with the same attributes and behaviors. From there, define what needs to be done at the most granular level with each function. Build that function so it may be applied to each object.

## Tables

**Building a table in HTML**

A table in HTML could be viewed as a series of ul tags structured in a table tag. As stated before the table tage lets the browser know that a table is being created, at which point tr (the tage letting the browser know a new row is being started), can be used. Within each tr tag, a td tag (the tag denoting what the data within each table cell) can be used. th, or table heading tags are used to create a heading for each column, and is useful for viewers who use screen readers. 

**Span**

Using the span attribute, you can denote if you want a column or row cell to span multiple cells. Simply place it in the td tag of the cell you wish to affect and select how many columns or rows you would like it to span (for columns us the 'colspan' tag, and rows the 'rowspan' tag).

**Long Tables**

By breaking up the list into theader, tbody and tfooter sections, you can break the table up and make it more readable codeside as well as to the reader.

## Functions, Methods, and Objects

**New Keyword** 

By using the new keyword and the object constructor, you can creat a blank object, and then add properties and methods to it.


**Ex:**

```
let hotel = new Object();
  hotel.name = `Quay';
  hotel.rooms = 40;
  hotel.booked = 25;

hotel.checkavailability = function(){
    return this.room - this.booked;
};
```

By creating a blank object we are able to first create an object and then inject data into that object as you get it. Adding a property name to the object later essentially acts as the .push method for arrays. You can further streamline the process by simply filling in the values to the objects much like you would CSS border shorthand.

**Ex:**

```
let parksHotel = new Hotel('Park', 120, 77);
```

This creats a new hotel with the same structure to the Quay hotel. 

**Arrays in Objects**

Arrays can be put in objects and vice versa to create complex system to be accessed later in your code.
