# The Orient Store - Interactive Shopping Experience

This Python script simulates an interactive shopping experience at "The Orient Store." It allows users to browse products, add items to a cart, proceed to checkout using a simulated payment system, and track their order history.  The script stores customer data, including account information, cart contents, and order history, in a JSON file for persistence.

## Features

*   **Customer Registration and Login:**  New customers can create accounts, providing their name, email, address, and phone number. Returning customers can log in using their ID.
*   **Product Browsing:** Customers can browse products by category and subcategory.  Product details, including price and availability, are displayed.
*   **Shopping Cart:** Customers can add items to their cart. The cart is saved between sessions for returning customers.
*   **Checkout Process:** A simulated payment system is implemented, including basic card validation (Luhn algorithm) and expiry date check.  Successful payments update the customer's order history.
*   **Order History:** Customers can view their past orders, including the items purchased, total cost, and order status.
*   **Data Persistence:** Customer data, including account information, carts, and order history, is stored in a `customers.json` file.
*   **User-Friendly Interface:** The script uses clear prompts and menus to guide the user through the shopping experience.

## Requirements

*   Python 3.x
*   No external libraries are required (other than standard Python libraries).

## How to Use

1.  **Save the code:** Save the Python code as a `.py` file (e.g., `orient_store.py`).
2.  **Run the script:** Open a terminal or command prompt, navigate to the directory where you saved the file, and execute the script using `python orient_store.py`.
3.  **Follow the prompts:** The script will guide you through the store interaction. You can choose to create an account, browse products, add items to your cart, proceed to checkout, and view your order history.

## Code Explanation

*   **`Store` Class:** Manages the overall store operations, including welcoming customers, handling new/returning customer logic, creating accounts, and generating customer IDs.
*   **`Customer` Class:** Represents a customer and handles their interactions, such as browsing, managing the cart, checking out, and viewing order history.
*   **`Product` Class:** Manages the product catalog and displays products by category and subcategory.
*   **`Cart` Class:** Manages the customer's shopping cart, allowing them to add, remove, and view items.  The cart is associated with the customer's data and saved to the JSON file.
*   **`PaymentSystem` Class:** Simulates the payment process, including basic card validation (Luhn algorithm) and expiry date checks.
*   **Data Storage (`customers.json`):** Customer data is stored in JSON format. The file structure includes customer ID, name, email, address, phone number, cart contents, and order history.
*   **Random ID Generation:** Customer IDs are generated randomly using a combination of "ort" prefix and a 5-digit number, ensuring uniqueness.
*   **Error Handling:** The script includes basic error handling to catch invalid inputs and other potential issues.
