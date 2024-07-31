 
 # Java Web

![netbeans](https://github.com/user-attachments/assets/cbc73d50-c1e0-4566-9916-243fb22b91eb)

# Overview

<h2>Purpose</h2>

The purpose of this project is to serve as a central controller in a Java web application, managing user actions, dispatching requests to appropriate handlers, interacting with JavaDB, and updating or removing items in the shopping cart.


<h2>Features</h2>
<h4>Front Controller Servlet</h4>

- **Centralized Request Handling**: The `Front Controller` servlet acts as a singlr entry point for handling all user actions.
- **Action Dispatching**: Uses a `hashmap` to map actions(Dispatcher clasess) that handle those actions.
- **Request Forwarding**: Forwards request to appropriate JSP pages based on the action.

<h4>JavaDB Integration</h4>

- **Database Conncetivity**: Connects to JavaDb for persistent data storage.
- **Data Operations**: Performs CRUD operations on the database for managing shopping system.

<h2>Debugging Process</h2>

### 1. Check Server Logs

- **Access Logs**: NetBeans intergrates well servers GlassFish. Access the server logs via the `Service` tab
- **Log Files Location**: Navigate to `logs` under the server node in the `Service` tab to view server logs directly within NetBeans.

### 2. NetBeans Debugger

- **Set Breakpoints**: Open you Java classes in NetBeans and click in the left margin of the editor to set breakpoints at lines where you want to pause execution.
- **Start Debugging**: Right-Click on your project and selet `Debug`.
- **Step Through Code**: `Step into`, `Step Over`, `Step Out` navigate through your code and inspect variable values.

<h2>Installation</h2>

- **IDE**: An integrated development environment (IDE) makes development easier [official website](https://netbeans.apache.org/)
- **NetBeans IDE 8.2**: A powerful IDE for Windows, macOS, and Linux, which provides extensive features for Java development.

**Getting Started**

- JDK 8 or higher
- NetBeans IDE

1. **Download and Install GlassFish**: 
   - [Download GlassFish](https://javaee.github.io/glassfish/download)
   - Unzip to preferred location

2. **Add GlassFish to NetBeans**:
   - Open NetBeans, go to **Services** > **Servers** > **Add Server**
   - Select **GlassFish Server**, provide server location, and finish

3. **Set Up Database (JavaDB)**:
   - Start JavaDB: **Services** > **Databases** > **Java DB** > **Start Server**
   - Create and connect to the database

- **Clone the Repository**:
   ```bash
   git https://github.com/ChungmanPARK12/WebJava.git
   cd Assignment2/ICTPRG556-Assignment_OnlineBookStore_Resources_v4/BookShop
  
# Architechture
<h2>Client Layer</h2>

- **Brower**: Users interact with the web application through a web brower, sending HTTP requests and receiving HTTP responses.

<h2>Web Server Layer</h2>

- **GlassFish Server**: The web server that hosts the Java web application, processed HTTP requests and forwards them to the appropriate servlets.

<h2>Controller Layer</h2>

- **Front Controller Servlet**: Acts as a centralized controller to handle all incoming HTTP requests. It determines the requestd action, delegates it to specific action hadlners and forwards the response to the appropriate view.

* ### Example of Code [Click here](https://github.com/ChungmanPARK12/LinkedExampleOfWebJava/blob/ef5693ea748a5eb730c559a8df5f6659d1f59451/README_Controller.md)

<h2></h2>

- **Action Dispatchers**: Classes that handle specific actions below:

- AddToCartDispatcher.java
- CheckoutDispatcher.java
- ContinueDispatcher.java
- HomeDispatcher.java
- UpdateCartDispatcher.java
- ViewCartDispatcher.java

* ### One Example Code of Add To Cart [Click here](https://github.com/ChungmanPARK12/LinkedExampleOfWebJava/blob/8a6244cd8f85211bfff88651a39052f8d156df28/README_AddToCart.md)

<h2>View Layer</h2>

- **JPS Pages**: Dynamic web pages that display the data to the user below:

- cart.jsp
- checkout.jsp
- error.jsp
- final.jsp
- footer.jsp
- header.jsp
- thankyou.jsp
- titles.jsp

* ### One Example Code of Cart [Click here](https://github.com/ChungmanPARK12/LinkedExampleOfWebJava/blob/dfb11fa5c216f677780d2e32fa7e1dff72eb9692/README_cartjsp.md)

<h2>Model Layer</h2>

- **Book**: Represents a book with attributes, ISBN, title, author and price.

* ### Example of Code [Click here](https://github.com/ChungmanPARK12/LinkedExampleOfWebJava/blob/ef5693ea748a5eb730c559a8df5f6659d1f59451/README_Controller.md)

- **Cart Item**: Represents an item in the shopping cart, including the book, quantity and cost.

* ### Example of Code [Click here](https://github.com/ChungmanPARK12/LinkedExampleOfWebJava/blob/ef5693ea748a5eb730c559a8df5f6659d1f59451/README_Controller.md)

<h2>Utility (Data Access Layer) Layer</h2>

- **Admit Book Store DAO**: Provides methods to interact with the database, such as retrieving and storing book and cart information

* ### Example of Code [Click here](https://github.com/ChungmanPARK12/LinkedExampleOfWebJava/blob/ef5693ea748a5eb730c559a8df5f6659d1f59451/README_Controller.md)

<h2>Database Layer</h2>

- **JavaDB**

* ### Example of Code [Click here](https://github.com/ChungmanPARK12/LinkedExampleOfWebJava/blob/ef5693ea748a5eb730c559a8df5f6659d1f59451/README_Controller.md)






## Summary

The Student Management API allows for efficient management of student records through CRUD operations. Users can create, read, update, and delete student data using HTTP methods. The API ensures data integrity with validation and secure endpoints. Postman is used for testing and documentation, providing a reliable interface for interacting with the API.

## Thank you
Thank you for visiting my github :)

 

 
