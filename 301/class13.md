# More CRUD

## CRUD Basics

1. **Which HTTP method would you use to update a record through an API?** Put

2. **Which REST methods require an ID parameter?** Delete, read, and update

## Video

1. **What’s the relationship between REST and CRUD?** CRUD is a way of manipulating information, it is the different kind of calls are that go to the API. Rest is controlling the data that is passed through those commands

2. **If you had to describe the process of creating a RESTful API in 5 steps, what would they be?** You would first have to install all of your dependencies so that you could use them later (mongoose, axios, react, express, nodemon, etc.). Next, you would build your specific routes so that the client side can create, read, update, and delete data in your database. Next, you would build out those routes on your back end, taking in queries for read, taking in id's for delete and read, and taking in id's as well as data to change for updating. Next you would build out how that information would be sent back to the client after the API has been reached by building the response values within the routes. Next, on your front end you would build out the model file for that specific type of data, and then implement that on your final page that the client would see.
