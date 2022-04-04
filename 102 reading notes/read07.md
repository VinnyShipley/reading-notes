# Programming with JavaScript

## **Control Flow**

Control Flow is the order that computers execute statements in a script. This order is from the first line to the last line unless it encounters a structure or line of code that alters that order.


## **Functions in JavaScript**

A funtion in JavaScript is a codeblock that can be invoked to do something. What that something is is up to the programmer. The sleekness of a function comes from the fact that entire scripts are contained within functions, and these functions can be placed anywhere in the code to carry out their purpose. 

## **Example of Function**

    function treebully(){
        let name = prompt("What is your name?");
        let tree = prompt("What is your favorite tree?");
        if(tree === "douglas fir" || tree === "birch" || tree ==="willow" || 
            tree === "Douglas Fir" || tree === "Birch" || tree === "Willow") {
            document.write("Well aren't you a coder with excellent taste in trees, " + name + ". That is a good tree");
            }
        else {
            document.write("I'm really sorry " + name + ", but your favorite tree is actually a bad tree");
    }

This is a program I wrote asking what someone's favorite tree is, and based on the user's input, they will be congratulated, or 'bullied'. Hence the name of the function that I was then able to drop into HTML, just by placing treebully() in between a script tag.