StarID:iv9197lp

My portion of the implementaion involved the Orders Class. I did add the isEmpty method to the ClientList Class and the isEmpty, getQtyById and setQtyById methods in the ProductList class to make my portion of the code work. Also previous implementation did not even use the ClientList class or the ProductList class so I had to make some modifications to how some of the add and display functions work so we could use the classes properly.

For the "Add Product to Client's Order" function in the switch statement it checks if a Client Id exists in the ClientList and reprompts the user if the provided Id is not valid. It does the same with products to ensure that a valid product is selected. It also prompts for an qty and checks the ProductList to ensure a valid quantity is avalible. If all the parameters are then it sets the value of the qty in the product list to account for the product ordered and adds the order info to the OrderList.

*Note* It does require the appended "C" or "D" to the front of the of the Id to accept the input.

For the "Display Order By Client ID" function in the switch statement it again prompts the user for a client Id. If the client Id is valid it looks through the order list and returns every instance of an Order that is associated with that client.


Script Session:
@JohnBelair ➜ /workspaces/warehouse-stage-i-implementation-JohnBelair (main) $ javac *.java
@JohnBelair ➜ /workspaces/warehouse-stage-i-implementation-JohnBelair (main) $ java UserInterface

--- Warehouse Management System ---
1. Add Client
2. Add Product
3. Add Product to Client's Wishlist
4. Add Product to Client's Order
5. Display All Clients
6. Display All Products
7. Display Client's Wishlist
8. Display Order By Client ID
9. Exit
Enter your choice: 1
Enter client's name: Jim
Enter client's address: 123 Elm Street
Client added successfully.

--- Warehouse Management System ---
1. Add Client
2. Add Product
3. Add Product to Client's Wishlist
4. Add Product to Client's Order
5. Display All Clients
6. Display All Products
7. Display Client's Wishlist
8. Display Order By Client ID
9. Exit
Enter your choice: 1
Enter client's name: Joan
Enter client's address: 124 Elm Street
Client added successfully.

--- Warehouse Management System ---
1. Add Client
2. Add Product
3. Add Product to Client's Wishlist
4. Add Product to Client's Order
5. Display All Clients
6. Display All Products
7. Display Client's Wishlist
8. Display Order By Client ID
9. Exit
Enter your choice: 2
Enter product name: Nike Shoes
Enter product quantity: 120
Enter product sale price: 100
Product added successfully.

--- Warehouse Management System ---
1. Add Client
2. Add Product
3. Add Product to Client's Wishlist
4. Add Product to Client's Order
5. Display All Clients
6. Display All Products
7. Display Client's Wishlist
8. Display Order By Client ID
9. Exit
Enter your choice: 2
Enter product name: Reebok shoes
Enter product quantity: 100
Enter product sale price: 60
Product added successfully.

--- Warehouse Management System ---
1. Add Client
2. Add Product
3. Add Product to Client's Wishlist
4. Add Product to Client's Order
5. Display All Clients
6. Display All Products
7. Display Client's Wishlist
8. Display Order By Client ID
9. Exit
Enter your choice: 4
Enter Client's ID: C1
Enter Products's ID: P1
Enter product quantity: 20
Order added successfully.

--- Warehouse Management System ---
1. Add Client
2. Add Product
3. Add Product to Client's Wishlist
4. Add Product to Client's Order
5. Display All Clients
6. Display All Products
7. Display Client's Wishlist
8. Display Order By Client ID
9. Exit
Enter your choice: 4
Enter Client's ID: C1
Enter Products's ID: P2
Enter product quantity: 80
Order added successfully.

--- Warehouse Management System ---
1. Add Client
2. Add Product
3. Add Product to Client's Wishlist
4. Add Product to Client's Order
5. Display All Clients
6. Display All Products
7. Display Client's Wishlist
8. Display Order By Client ID
9. Exit
Enter your choice: 4
Enter Client's ID: C2
Enter Products's ID: P1
Enter product quantity: 101
Sorry we only have 100 in stock. Please enter a valid quantity.
Enter product quantity: 100
Order added successfully.

--- Warehouse Management System ---
1. Add Client
2. Add Product
3. Add Product to Client's Wishlist
4. Add Product to Client's Order
5. Display All Clients
6. Display All Products
7. Display Client's Wishlist
8. Display Order By Client ID
9. Exit
Enter your choice: 8
Enter Client's ID: C1
Order [ID: O1 Client ID: C1 Product ID: P1 Product Quantity: 20]
Order [ID: O2 Client ID: C1 Product ID: P2 Product Quantity: 80]

--- Warehouse Management System ---
1. Add Client
2. Add Product
3. Add Product to Client's Wishlist
4. Add Product to Client's Order
5. Display All Clients
6. Display All Products
7. Display Client's Wishlist
8. Display Order By Client ID
9. Exit
Enter your choice: 8
Enter Client's ID: C2
Order [ID: O3 Client ID: C2 Product ID: P1 Product Quantity: 100]

--- Warehouse Management System ---
1. Add Client
2. Add Product
3. Add Product to Client's Wishlist
4. Add Product to Client's Order
5. Display All Clients
6. Display All Products
7. Display Client's Wishlist
8. Display Order By Client ID
9. Exit
Enter your choice: 6
Product [ID: P1, Name: Nike Shoes, Quantity: 0, Sale Price: $100.0]
Product [ID: P2, Name: Reebok shoes, Quantity: 20, Sale Price: $60.0]

--- Warehouse Management System ---
1. Add Client
2. Add Product
3. Add Product to Client's Wishlist
4. Add Product to Client's Order
5. Display All Clients
6. Display All Products
7. Display Client's Wishlist
8. Display Order By Client ID
9. Exit
Enter your choice: 9