---
layout: post
title:      "RESTful -- Explained! "
date:       2019-02-15 19:16:15 +0000
permalink:  restful_--_explained
---


RESTful APIs are an application program interface. REST stands for representational state transfer.  Comparatively, RESTful routing leverages less bandwidth. 

Each URL is a request and data is the response. A request is composed of 4 units.

1. Endpoint: The endpoint is the text from http:// to .com. It determines the requested resource. The path is what follows the / after the .com. It determines the resource you’re requesting for. 

2. Method: 
GET 
Gets resource from server → looks for data and sends it back (READ operation) 

POST
Creates a new resource on a server → new entry in database (CREATE operation)

PUT & PATCH
Updates a resource on a server (UPDATE operation)

DELETE 
Deletes resource from server (DELETE operation)

3. Headers: Provide info to client and server

4. Data (body): contains info you want to be sent to server (if method requires such an action)

Simply put, RESTful routes are a standardized way of routing through HTTP requests. 
The data flow is as follows:

1. An HTTP request, containing an HTTP verb (GET, PATCH, DELETE, UPDATE) is sent
2. The router in the app processes the request and  routes the data to the proper controller and method
3. The controller action wither performs a task or fetches and renders data from the database 

