# Javascript

## **Concept**

If HTML is the walls of a house, and CSS is the way a house looks, one way to think about JavaScript would be to think of it as the furniture and appliances in the house. These are the elements of the house that the person living in it would interact with.

>This metaphor might be getting away from me at this point, but you can come with me on this half baked analogy, can't you?

It is with this interaction that the user is able to input data into the site, and then JavaScript can then take that information and respond. Whether that response is seen by the user is up to the programmer. One of the things that stuck out to me during the lecture today was to treat the computer like a third grader when working in Javascript. it is a logic based system, so it will do what you tell it to do in a the most literal way possible.

## **In Practice**

Essentially, the way you set up a script for JavaScript is to name the variables, create a script that can manipulate those variables, and then designate where you want the resulting data to go. I'm almost certain that this is criminally underselling the complexity of JavaScript, but hey, this is my first day with the program. 

## **Example Code**

    let tree = prompt("What is your favorite tree?");
            if(tree === "douglas fir" || tree === "birch" || tree ==="willow" || 
            tree === "Douglas Fir" || tree === "Birch" || tree === "Willow") {
                document.write("What a good tree you've chosen, " + name + ". That is a good tree");
            }
            else {
                document.write("I'm really sorry " + name + ", but your favorite tree is actually a bad tree");
            }

I have to say I had my first moment of literally jumping out of my chair when I cracked the code on this block of code. This block asks the user, upon opening the webpage, "What is your favorite tree?" and gives them a text field to answer their question. If it is any of the phrases contained in the () immeadiately after "if", then they are given the "What a good tree you've chosen, " + name + ". That is a good tree" response. (The name variable was assigned earlier and is gathered from the user in a prior text box). If they give anything else than those listed phrases though, they are greeted with the "I'm really sorry " + name + ", but your favorite tree is actually a bad tree" reasponse.

[Back to main page](README.md)