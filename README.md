## System Overview
This application provides a user-friendly interface for gym staff to:
* Process Sales: Select products and enter quantities for purchase.
* Monitor Inventory: Real-time tracking of remaining stock.
* Audit Transactions: A dedicated log system to view all past sales.

## Frame Responsibilities

The system is organized into three main windows (Frames):

TransactionFrame
The main dashboard where users select items from a dropdown and input purchase quantities.

InventoryFrame
Displays a complete list of products and their current stock levels in a text area.

LogsFrame
Shows a chronological record of every successful transaction made during the session.

## Use of Arrays

The system relies on Parallel Arrays in a central Data.java class to keep information synchronized:

* products and prices: These arrays store the names and costs of items. They are linked by their index (e.g., products[0] is the name, and prices[0] is its price).
* stock: This integer array manages the quantity. When a purchase is made, the system finds the correct index and subtracts the quantity bought.
* logEntries: A String array that grows every time a purchase is successful, storing the details of the sale as a single line of text.

## How to Run

1. Open the project in Netbeans or any Java IDE.
2. Ensure Data.java, Transaction.java, InventoryFrame.java, and LogsFrame.java are in the same package.
3. Right-click Transaction.java and select Run File.

## Technologies Used
* Language: Java
* GUI Library: Java Swing (JFrame, JPanel, JButton, JTextArea, etc.)
* Storage: In-memory Arrays (Static)
