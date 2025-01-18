ECommerce-API-Assignment

Table of Contents:
- Customer Management
    - Get Customers
    - Add Customers
    - Update Customers
    - Delete Customers
- Customer Account Management
    - Get Customer Accounts
    - Add Customer Accounts
    - Update Customer Accounts
    - Delete Customer Accounts
- Order Management
    - Get Orders
    - Add Orders
    - Update Orders
    - Delete Orders
- Product Management
    - Get Products
    - Add Products
    - Update Products
    - Delete Products
 
  # Customer Management #
  
  The program was properly connected to the database as part of the database integration using Flask-SQLAlchemy. I created the Customers table using the .Model as well as the schema for
  the table. For this part of the program, I created four endpoints with routes using 'GET', 'POST', 'PUT', and 'DELETE'. The 'GET' route uses a simple two lines of code to fetch the
  customers. The line 'customers = Customer.query.all()' is used and this fetches all of the rows in the Customers table. The user can add a new customer using the 'POST' route. The
  fields required are id, name, email, and phone. With all of these fields provided, the user can send the 'POST' request and have the customer added to the database. Once the request
  has gone through successfully, the user will receive back a '201' code for newly created resource. To update a customer, the user would use the 'PUT' route. The 'PUT' route requires
  every field to be provided that the 'POST' route requires in order to send the request. The only difference is that the 'PUT' route will need an 'id' to be inserted into the URL
  (the code is set up to take an 'id' like this: '@app.route('/customers/<int:id>', methods=['PUT'])'). A successful request will result in a '200' code for code works. To delete a
  customer, the user would use a 'DELETE' route. Just like the 'PUT' route, the URL must include an 'id'. This allows the program to delete only the customer with the provided 'id'.
  
  # Customer Account Management #
  
  The program was properly connected to the database as part of the database integration using Flask-SQLAlchemy. I created the CustomerAccounts table using the .Model as well as the
  schema for the table. For this part of the program, I created four endpoints with routes using 'GET', 'POST', 'PUT', and 'DELETE'. The 'GET' route uses a simple two lines of code to
  fetch the customer accounts. The line 'customer_accounts = CustomerAccount.query.all()' is used and this fetches all of the rows in the CustomerAccounts table. The user can add a new
  customer account using the 'POST' route. The fields required are username, password, and customer_id. With all of these fields provided, the user can send the 'POST' request and have
  the customer account added to the database. Once the request has gone through successfully, the user will receive back a '201' code for newly created resource. To update a customer
  account, the user would use the 'PUT' route. The 'PUT' route requires every field to be provided that the 'POST' route requires in order to send the request. The only difference is
  that the 'Put' route will need an 'id' to be inserted into the URL (the code is set up to take an 'id' like this: '@app.route('/customer_accounts/<int:id>', methods=['PUT'])'). A
  successful request will result in a '200' code for code works. To delete a customer, the user would use a 'DELETE' route. Just like the 'PUT' route, the URL must include an 'id'. This
  allows the program to delete only the customer with the provided 'id'.
  
  # Order Management #
  
  The program was properly connected to the database as part of the database integration using Flask-SQLAlchemy. I created the Orders table using the .Model as well as the schema for
  the table. For this part of the program, I created four endpoints with routes using 'GET', 'POST', 'PUT', and 'DELETE'. The 'GET' route uses a simple two lines of code to fetch the
  orders. The line 'orders = Order.query.all()' is used and this fetches all of the rows in the Orders table. The user can add a new order using the 'POST' route. The
  fields required are id, date, delivery date, ordered products, and customer_id. With all of these fields provided, the user can send the 'POST' request and have the order added to
  the database. Once the request has gone through successfully, the user will receive back a '201' code for newly created resource. To update an order, the user would use the 'PUT'
  route. The 'PUT' route requires every field to be provided that the 'POST' route requires in order to send the request. The only difference is that the 'PUT' route will need an 'id'
  to be inserted into the URL (the code is set up to take an 'id' like this: '@app.route('/orders/<int:id>', methods=['PUT'])'). A successful request will result in a '200' code for
  code works. To delete an order, the user would use a 'DELETE' route. Just like the 'PUT' route, the URL must include an 'id'. This allows the program to delete only the order with
  the provided 'id'.
  
  # Product Management #
  
  The program was properly connected to the database as part of the database integration using Flask-SQLAlchemy. I created the Products table using the .Model as well as the schema for
  the table. For this part of the program, I created four endpoints with routes using 'GET', 'POST', 'PUT', and 'DELETE'. The 'GET' route uses a simple two lines of code to fetch the
  products. The line 'products = Product.query.all()' is used and this fetches all of the rows in the Products table. The user can add a new product using the 'POST' route. The
  fields required are id, name, and price. With all of these fields provided, the user can send the 'POST' request and have the product added to the database. Once the request has gone
  through successfully, the user will receive back a '201' code for newly created resource. To update a product, the user would use the 'PUT' route. The 'PUT' route requires every field
  to be provided that the 'POST' route requires in order to send the request. The only difference is that the 'PUT' route will need an 'id' to be inserted into the URL (the code is set
  up to take an 'id' like this: '@app.route('/products/<int:id>', methods=['PUT'])'). A successful request will result in a '200' code for code works. To delete a product, the user
  would use a 'DELETE' route. Just like the 'PUT' route, the URL must include an 'id'. This allows the program to delete only the product with the provided 'id'.
