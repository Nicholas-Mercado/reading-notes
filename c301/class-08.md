# APIs

## API Design Best Practices

**What does REST stand for?**

REST stands for Representational State Transfer

**REST APIs are designed around a ____.**

Resource

**What is an identifier of a resource? Give an example.**

The identifier of a resource is a URI.

```http

https://adventure-works.com/orders/1

```

**What are the most common HTTP verbs?**

The most common HTTP verbs are GET,POST,PUT,PATCH and DELETE

**What should the URIs be based on?**

URIs should be based on nouns, the actual resource

**Give an example of a good URI. What does it mean to have a ‘chatty’ web API?**

A API that makes a lot of web requests to a web server

**Is this a good or a bad thing?**

A API that is chatty is a bad thing cause it imposes a larger load on the webserver.

**What status code does a successful GET request return?**

status code 200 (OK)

**What status code does an unsuccessful GET request return?**

status code 201 (Created)

**What status code does a successful POST request return?**

status code 201 (Created)

**What status code does a successful DELETE request return?**

status code 204 (No Content)

<cite>RESTful web API design,https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design</cite>

## Things I want to know more about
