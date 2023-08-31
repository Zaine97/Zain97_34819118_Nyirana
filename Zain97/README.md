User Functionality

The CRUD RESTful API project allows users to perform Create, Read, Update, and Delete operations on a collection of resources using HTTP requests. In this project, we have implemented a simple API for managing customer data. Users can interact with the API to perform the following actions:
1. Create a New Customer

Users can send a POST request to /api/customers with a JSON payload containing customer details. The API will create a new customer record and return the created customer's information.
2. Retrieve Customer Information

Users can send a GET request to /api/customers/{id} to retrieve information about a specific customer. Replace {id} with the customer's unique identifier.
3. Update Customer Information

Users can send a PATCH request to /api/customers/{id} with a JSON payload containing the updated customer details. The API will update the customer's information and return a success response.
4. Delete a Customer

Users can send a DELETE request to /api/customers/{id} to delete a customer from the database. Replace {id} with the customer's unique identifier.