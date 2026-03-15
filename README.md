### **Dine-In Delight: Project Overview**

**Dine-In Delight** is a console-based, multi-restaurant food ordering and management system developed using the **C programming language**. Designed to simulate modern online food delivery platforms, the project provides a structured digital solution for both customers and restaurant owners, eliminating the errors associated with manual ordering.

---

### **Core Interfaces**

* 
**Customer Interface**: Allows users to sign up and log in securely to browse menus from **16 different restaurants**. Customers can add items to a virtual cart, modify their selection, and generate a final bill that includes **18% GST**.


* 
**Owner Interface**: Provides a backend for restaurant owners to manage their specific branch. Owners can securely log in to view their menu, restock items to maintain real-time availability, and update estimated delivery time ranges.



---

### **Key Features & Technical Implementation**

* 
**Secure Authentication**: The system uses **password masking** via the `getch()` function, displaying `*` characters instead of plain text to improve login security.


* 
**Data Persistence**: The project utilizes **file handling** (`FILE *` pointers) to permanently store and retrieve data from text files, including `owners.txt`, `customers.txt`, and individual menu files for each restaurant.


* 
**Stock Management**: The system tracks real-time inventory, automatically deducting quantities from the menu files once an order is finalized.


* 
**Modular Programming**: Logic is organized into specific functions like `load_menu()`, `save_menu()`, and `show_menu()` to ensure the code is readable and easy to maintain.


* 
**User Details**: During signup, the system collects and stores personal details such as the user's phone number and address, which are then displayed on the final invoice.



---

### **C Concepts Utilized**

* 
**Structures (`struct`)**: Used to group related data, such as item names, prices, and stock levels, into a single `MenuItem` type.


* 
**Arrays**: One-dimensional arrays manage the shopping cart (`idx[]` and `qty[]`), while two-dimensional arrays organize menu data across all restaurants.


* 
**Buffer Handling**: A dedicated `clear_buffer()` function is implemented to remove leftover characters (like `\n`) from the input buffer, preventing skipped or incorrect inputs after `scanf()`.


* 
**String Manipulation**: Standard functions such as `strcmp()`, `strcpy()`, and `strlen()` are used to handle usernames, passwords, and item descriptions.



**Would you like me to explain how any specific part of the code (like the file handling or the billing logic) works in more detail?**
