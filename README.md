# E-Commerce-API


# ABOUT
This API provides functionality for managing product inventory in an e-commerce platform. It allows admins to add products, list products, delete products, and update product quantities. The API is built using Node.js and MongoDB.

**STEPS TO USE THE API: **
1) Type "npm install" command in view section of terminal 
1) run "npm init" command on terminal 
2) start the server using "node app.js"
3) Open postman using https://www.postman.com/
4) Make a GET request on localhost:3000/products
5) The products should be visible


**API Endpoints**
  
  
  Add a product

URL: POST /products/create
Request body:


{ "name": "laptop", "quantity": 10 }
  
Response body:


{ "product": { "name": "laptop", "quantity": 10 } }
  
  
List products

URL: GET /products
Response body:

{ "products": [ { "id": 1, "name": "laptop", "quantity": 10 }, { "id": 2, "name": "camera", "quantity": 5 }, ... ] }

  
Delete a product

URL: DELETE /products/:id
Response body:

{ "message": "Product deleted" }
Update product quantity

URL: POST /products/:id/update_quantity/?number=10
Response body:

{ "product": { "id": 1, "name": "laptop", "quantity": 20 }, "message": "Updated successfully" }


# TECHSTACK
Node.Js, MongoDB
