# CRUD

## Reading

1. **In your own words, describe what each group of status code represents:**

* 100's: Informational status codes. They let the client know that the request has been recieved and the server will try to make the request happen. 

* 200's: Success codes. This request was returned sucessfully.

* 300's: Redirect codes. The information being requested has been moved, and the request has been redirected to another location where hopefully the information now resides.

* 400's: Client error codes. The request sent to the server from the client is invalid for whatever reason.

* 500's: Server error codes. The server is either overwhelmed or unreachable for some reason. The client should retry the request.

2. **What is a status code 202?** The request is valid, but because it is asynchronous, it will finish processing sometime in the future.

3. **What is a status code 308?** The request has been redirected permanently to a different URL.

4. **What code would you use if an update didn’t return data to a client?** 204

5. **What code would you use if a resource used to exist but no longer does?** 410

6. **What is the ‘Forbidden’ status code?** 403

## Video

1. **Why do we need to pull our MongoDB database string out of our server and put it into our .env?** Because when it is deployed you will want to be using a path that isn't your local host to access it.

2. **What is middleware?** Code that gets run after you get a request, but after it is passed to the routes.

3. **What does app.use(express.json()) do?** It allows the server to read JSON files as a body, rather than a GET or a POST element.

4. **What does the /:id mean in a route?** It would mean that id is being passed in as a parameter of the request, allowing you to access anything that is passed in after that backslash in the request.

5. **What is the difference between PUT and PATCH?** Put updates the entire object associated with that JSON file, rather than just the key value pair that exists in the JSON file that the request is manipulating.

6. **How do you make a default value in a schema?** You add a key value pair of default and set it to whatever you want the default value to be within that object.

7. **What does a 500 error status code mean?** Something has gone wrong onthe website's server but the server could not be more specific as to what actually went wrong.

8. **What is the difference between a status 200 and a status 201?** 200 means that the request was a success, and 201 means that it is being processed. 
