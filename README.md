# Purpose
How to use RESTful API. To do this, we'll build a Node.js football app using a football-data API.

* Framework: hapi.js 

## What is an API?
An **API** is an acronym for **Application Programming Interface**, which is defined as a set of subroutine definitions, protocols, and tools for building application software.

* In short, an API can be referred to as an **interface**.
* This is because it hides the details of software implementation by providing methods of communication between various software components.

## What is a RESTful API?
**REST** is an acronym for REpresentational State Transfer.

* Relies on a stateless, client-server, cacheable communications protocol.
* REST response can be in various formats, such as JSON and XML.

Basically a RESTful API defines a set of **endpoints**, which devs can perform requests and receive responses via **HTTP methods** (GET, POST, PUT, PATCH, DELETE).

### Common terms associated with a RESTful API
* **Resource**
* **Endpoint**
* **HTTP Methods/Verbs**

## What are HTTP Methods
HTTP methods are occasionally called HTTP verbs. They perform operations on a RESTful API.

The HTTP verbs include:
* **GET**
* **POST**
* **PUT**
* **PATCH**
* **DELETE**

All correspond to **CRUD** (CREATE, READ, UPDATE, and DELETE) operations.

#### GET
* The **GET** method is used to retrieve a list of resources or a specified resource from a server.

**Examples**
* `GET http://www.example.com/users`
* `GET http://www.example.com/users/89`

The **first request** makes a `GET` request to the `users` endpoint, which will return a response of all users.

The **second request** makes a `GET` request but this time to the `users/:id` endpoint, where `:id` refers to the a ID (89 in the case above) of a specified user.

#### POST
* The **POST** method is used to create a new resource on the server.

**Examples**
* `POST http://www.example.com/users`

Making a `POST` request to the `users` endpoint will create a new resource with the `POST`ed data.

#### PUT
* The **PUT** method is used to update a specified resource on the server.

**Examples**
* `PUT http://www.example.com/users/89`

Making a `PUT` request to the `users/:id` endpoint will update the specified user.

#### PATCH
* The **PATCH** method is also used to modify/update a specified resource on the server.

**Examples**
* `PATCH http://www.example.com/users/89`

Making a `PATCH` request to the `users/:id` endpoint will update the specified user with only the needed changes.

#### DELETE
* The **DELETE** method is used to delete a resource from a server.

**Examples**
* `DELETE http://www.example.com/users/89`

Making a `DELETE` request to the `users/:id` endpoint will delete the user with the ID:89.

### The difference between PUT and PATCH
* `PUT` and `PATCH` are both used to update a resource on the server.
* The main difference is that `PUT` will update the entire resource.
* `PATCH` on the other hand, will only update the specified part of the resource.  
