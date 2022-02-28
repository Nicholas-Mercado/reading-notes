# CRUD

## Status Codes Based On REST Methods

**In your own words, describe what each group of status code represents:**

**100’s =**

These are informational status codes, telling you that the request has been received.

**200’s =**

These are success codes, telling you that the request has been accepted

**300’s =**

These are redirection codes, telling you that the request is not at the expected location

**400’s =**

These are client error codes, telling you your request is invalid

**500’s =**

These are server error codes, telling you that the server is unreachable or overwhelmed

**What is a status code 202?**

This code tell you that the request is valid, but it will process sometime in the future

**What is a status code 308?**

This code tells you that the resource you have requested has been permanently moved and you should access it directly using the url

**What code would you use if an update didn’t return data to a client?**

204 No Content

**What code would you use if a resource used to exist but no longer does?**

410 Gone

**What is the ‘Forbidden’ status code?**

403 Forbidden 

## Build A REST API With Node.js, Express, & MongoDB

**Why do we need to pull our MongoDB database string out of our server and put it into our .env?**

To protect our sensitive information.

**What is middleware?**

Middleware is software that provides common services and capabilities to applications outside of what's offered by the operating system.

<cite>What is middleware?,https://www.redhat.com/en/topics/middleware/what-is-middleware</cite>

**What does app.use(express.json()) do?**

Its a built in middleware function that parses incoming requests with JSON

**What does the /:id mean in a route?**

I means its a parameter that we can access with reg.params.id

**What is the difference between PUT and PATCH?**

PATCH is used to update a existing entity with new information.

PUT is used to set an entities information completely.

**How do you make a default value in a schema?**

You can make a default value by using the default keyword

**What does a 500 error status code mean?**

It means the actual server has a error

**What is the difference between a status 200 and a status 201?**

Code 201 is a more specific way to say that you created something

## Things I want to know more about