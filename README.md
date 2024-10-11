# **eCommerce Application (OOP - Java)**

## **Project Overview**  
This is an Object-Oriented eCommerce application implemented in Java. The application models various components of an online shopping system, including Products (Books, Clothing, Electronics), Customer, Cart, and Order. Each class encapsulates specific features and behaviors associated with an eCommerce platform.

## **Features**
- **Product Management**: Classes for different product categories like books, clothing, and electronics.
- **Customer Interaction**: Customers can add products to their cart, place orders, and view purchase history.
- **Shopping Cart**: A cart system that allows customers to add/remove products and calculates the total order amount.
- **Order Processing**: Handling of customer orders with tracking of products and their quantities.

## **Project Structure**

### 1. **Product** (Superclass)
Represents a generic product with common attributes and methods.  

#### **Attributes**:
- `id`: Unique identifier for the product.
- `name`: Name of the product.
- `price`: Price of the product.
- `description`: Description of the product.

#### **Methods**:
- Getters and setters for each attribute.
- `toString()`: Returns a string representation of the product.

### 2. **Book** (Subclass of `Product`)
A subclass that represents a book product with additional attributes.

#### **Attributes**:
- `author`: The author of the book.
- `publisher`: The publisher of the book.
- `ISBN`: Unique identifier for the book.

### 3. **Clothing** (Subclass of `Product`)
Represents clothing items with specific attributes.

#### **Attributes**:
- `size`: Size of the clothing (e.g., S, M, L).
- `color`: Color of the clothing.
- `material`: Material used (e.g., cotton, polyester).

### 4. **Electronics** (Subclass of `Product`)
Represents electronics with attributes unique to electronic products.

#### **Attributes**:
- `brand`: Brand of the electronic product.
- `warrantyPeriod`: Warranty period for the product.

### 5. **Customer**
Represents a customer in the system with personal details.

#### **Attributes**:
- `customerId`: Unique identifier for the customer.
- `name`: Customer's name.
- `email`: Customer's email address.
- `address`: Customer's shipping address.

#### **Methods**:
- `addProductToCart()`: Adds a product to the customer's cart.
- `placeOrder()`: Places an order for the items in the cart.
- `viewOrderHistory()`: Displays the customer's past orders.

### 6. **Cart**
Represents a shopping cart with products that the customer intends to purchase.

#### **Attributes**:
- `items`: A list of `Product` objects.
- `totalAmount`: The total price of all the items in the cart.

#### **Methods**:
- `addProduct(Product product)`: Adds a product to the cart.
- `removeProduct(Product product)`: Removes a product from the cart.
- `calculateTotal()`: Calculates the total price of the cart.

### 7. **Order**
Represents an order placed by the customer.

#### **Attributes**:
- `orderId`: Unique identifier for the order.
- `products`: List of `Product` objects in the order.
- `totalPrice`: Total price of the order.
