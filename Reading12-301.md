### *In your own words, describe what each group of status code represents:* ###

- 100 - 199: These are informational status codes; they usually tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client. Like using a different protocol or telling the client that its request will fail before they start sending the body.

- 200 - 299: These are the success codes. They tell the client that its request was accepted. In case of asynchronous processing of a request (202), this doesn’t mean the request was successfully processed only that it met all validation requirements at the time of sending.

- 300 - 399: These are redirection codes. They tell the client that the resource they are requesting isn’t available at the expected location anymore. This can have multiple reasons, be temporary or permanent, but the client has to issue a request to the new location.

- 400 - 499: These are the client error codes. They are all about invalid requests a client sent to a server. There are several causes to this, timeouts, wrong URI, missing authentication, etc. A client is sending incorrect input and should confirm the input parameters are correct before retrying the request

- 500 - 599: These are the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies, but sometimes they can be directly related to client requests that trigger error exceptions on the server. These errors can be temporary or permanent. Usually it’s best for the client to retry the same request.

### *What is a status code 202?* ###

- 202 Accepted - Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future. The response body should include an URL to the finished resource with some information about when it will be available, or an URL to some monitoring endpoint that tells the client when the resource is available.

### *What is a status code 308?* ###

- 308 Permanent Redirect - This tells the client to use another URL to access the resource and not use the current URL anymore. It’s helpful when we have multiple endpoints for one resource, but don’t want to implement reading from all of them.

### *What code would you use if an update didn’t return data to a client?* ###

- 204 No Content

### *What code would you use if a resource used to exist but no longer does?* ###

- 204 No Content - The most fitting status code for this case. It’s better to reduce traffic and simply tell the client the deletion is complete and return no response body (as the resource has been deleted).

### *What is the ‘Forbidden’ status code?* ###

- The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

### *Why do we need to pull our MongoDB database string out of our server and put it into our .env?* ###

- Because when we want to deploy our application, we are going to use something that is not our local host; therefore, we need to take it out and put it into an environment variable.


### *What is middleware?* ###

- It is essentially a code that runs when the server gets a request before it get passed to next routes

### *What does app.use(express.json()) do?* ###

- It let our server accept JSON asa body instead of a post element of a get a element


### *What does the /:id mean in a route?* ###

- It's a parameter that we can access by typing request.params.id and this would give us access to what it's passed in after the first slash.

### *What is the difference between PUT and PATCH?* ###

- PUT: will update all the information, but PATCH will only update based on the user's input

### *How do you make a default value in a schema?* ###

- For instance: setting date, we do Date.now it's just going to default it to the current date now


### *What does a 500 error status code mean?* ###

- There is an error in the server and it's not a user error

### *What is the difference between a status 200 and a status 201?* ###

- Status 201 means successfully created an object vs status 200 means everything was successful.

(References: https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/, https://www.youtube.com/watch?v=fgTGADljAeg)