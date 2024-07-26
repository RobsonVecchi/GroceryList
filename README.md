# Grocery List Application

This is a simple Flask-based web application for managing a grocery list. Users can view items from a database, add items to a shopping list, and remove items from the list.

## Features

- **View Items**: Displays all items from the grocery list database.
- **Add Items**: Allows users to add items to their shopping list.
- **Remove Items**: Enables users to remove selected items from the shopping list.

## Getting Started

### Prerequisites

- Python 3.x
- Flask
- SQLite

### Installation

1. Clone the repository;
2. Navigate to the project directory;
3. Install dependencies on requirements.txt;
4. Set up the database (Ensure that `grocery_list.db` exists in the project directory and contains a table named `groceries` with a column `name`.);
5. Run the application (The application will be accessible at `http://127.0.0.1:5000/`.)

### Usage

1. **View Items**: When the application is accessed, it displays all items from the database along with a randomly shuffled shopping list.

2. **Add Items**: Use the provided form to select items and add them to the shopping list.

3. **Remove Items**: Select items from the shopping list and click the "Remove" button to delete them.

### Code Overview

- **Routes**:
  - `"/"`: Displays the main page with all items and the shopping list. Handles GET and POST requests.
  - `"/add_items"`: Adds selected items to the shopping list.
  - `"/remove_items"`: Removes selected items from the shopping list.

- **Database Management**:
  - `get_db()`: Connects to the SQLite database and retrieves all items from the `groceries` table. Also generates a shuffled shopping list.
  - `close_connection()`: Ensures the database connection is closed after each request.

## Contact

For any questions or suggestions, please contact [robson.t.vecchi@gmail.com](mailto:robson.t.vecchi@gmail.com).
