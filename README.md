# Online Shopping System

## Description
**Online Shopping System** is a simple console-based application developed in C. It simulates an online shopping environment where users can browse products, make purchases, and provide feedback. The system uses binary files as a database to store customer information, product details, payments, and feedback. This project is designed to demonstrate basic file handling, data structures, and queue management in C.

## Features
- **Product Browsing**: Customers can view the available products and their details.
- **Purchase Products**: Customers can add products to their cart and proceed to checkout.
- **Feedback System**: After purchasing, customers can leave feedback, which is stored and managed in a separate binary file.
- **Data Persistence**: All customer data, product information, payment details, and feedback are stored in binary files, ensuring data persistence across sessions.
- **Queue Management**: The system includes a priority queue to manage customer orders.

## File Structure
The project consists of the following files:

- **Source Files**:
  - `main.c`: The entry point of the application, handling the main flow of the program.
  - `interface.c`: Contains the functions for the user interface and interaction with the system.
  - `product.c`: Manages the product-related operations, including adding, viewing, and deleting products.
  - `p-queue.c`: Implements the priority queue for managing customer orders.
  - `validations.c`: Contains functions for validating user inputs and system operations.

- **Binary Files** (Database):
  - `customer_db.bin`: Stores customer information, including login details and purchase history.
  - `products_DB.bin`: Stores product details like product ID, name, price, and stock.
  - `payment_db.bin`: Contains payment records associated with customer purchases.
  - `feedback_DB.bin`: Stores customer feedback for the purchased products.
  - `queue_db.bin`: Manages the priority queue of customer orders.

- **Executable File**:
  - `main.exe`: The compiled executable file to run the Online Shopping System on a Windows machine.

## How It Works
1. **User Interface**: Upon running the `main.exe`, users are greeted with a menu-driven interface where they can choose to browse products, make purchases, or leave feedback.
2. **Database Interaction**: The system reads from and writes to the binary files for all operations, ensuring data persistence.
3. **Queue Management**: Customer orders are managed using a priority queue, ensuring efficient order processing.

## Compilation and Execution
To compile and run the project:

1. **Compile the Source Code**:
   ```
   gcc main.c interface.c product.c p-queue.c validations.c -o main.exe
   ```
   Run the Executable:

2. **On Windows:**
```
main.exe
```
OR
**On Linux (with Wine installed):**
```
wine main.exe
```
3. **Binary Files:**
Ensure that the binary files (customer_db.bin, products_DB.bin, payment_db.bin, feedback_DB.bin, queue_db.bin) are in the same directory as main.exe before running the program.

**Future Enhancements**
GUI Development: Transition from a console-based interface to a graphical user interface (GUI) to enhance user experience.
Database Integration: Replace binary files with a relational database like MySQL for more complex data management and querying capabilities.
Advanced Features: Add features such as user authentication, product search functionality, and more detailed order tracking.

**Contributing**
Contributions are welcome! To contribute to the Online Shopping System project, please follow these steps:
1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and test thoroughly.
4. Submit a pull request with a clear description of the changes.
5. Please ensure that your code adheres to the project's coding standards and includes appropriate documentation.
   
## License
This project is licensed under the MIT License. See the LICENSE file for more details.

## Contact
For questions or feedback, please reach out to me at prabhupugal01@gmail.com.
