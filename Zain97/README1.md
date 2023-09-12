URL1 https://project234819118api.azure-api.net
  URL2 https://zainproject2.azurewebsites.net/
 
 
 # EcoPower Logistics CRUD RESTful API

Welcome to the documentation for the EcoPower Logistics CRUD RESTful API. This API allows you to manage logistics data related to customers, orders, and products. Below, you'll find information on how to use the API, a list of available endpoints, and additional aspects that have been implemented.

## How to Use the API

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/your-username/ecopower-logistics-api.git

   Install any necessary dependencies. You might need to run:

bash

dotnet restore

Configure the connection to your database in the appsettings.json file.

Start the API server by running:

bash

dotnet run

The API will be accessible at http://localhost:5000 (or a different port if configured).


Endpoints

Customers

    GET /api/customers: Retrieve all customers.
    GET /api/customers/{customerId}: Retrieve a customer by ID.
    POST /api/customers: Create a new customer.
    PATCH /api/customers/{customerId}: Update an existing customer by ID.
    DELETE /api/customers/{customerId}: Delete a customer by ID.

Orders

    GET /api/orders: Retrieve all orders.
    GET /api/orders/{orderId}: Retrieve an order by ID.
    POST /api/orders: Create a new order.
    PATCH /api/orders/{orderId}: Update an existing order by ID.
    DELETE /api/orders/{orderId}: Delete an order by ID.
    GET /api/customers/{customerId}/orders: Retrieve all orders for a specific customer.

Products

    GET /api/products: Retrieve all products.
    GET /api/products/{productId}: Retrieve a product by ID.
    POST /api/products: Create a new product.
    PATCH /api/products/{productId}: Update an existing product by ID.
    DELETE /api/products/{productId}: Delete a product by ID.
    GET /api/orders/{orderId}/products: Retrieve all products for a specific order.

Additional Aspects Implemented

    Customer Existence Check: Private methods are implemented to check if a customer exists based on the ID before editing or deleting an item.

    Order Existence Check: Private methods are implemented to check if an order exists based on the ID before editing or deleting an item.

    Product Existence Check: Private methods are implemented to check if a product exists based on the ID before editing or deleting an item.

    Authentication: The API requires authentication to restrict access.

    Swagger Documentation: Swagger UI is integrated to provide interactive API documentation. You can access it at http://localhost:5000/swagger when the API is running.
