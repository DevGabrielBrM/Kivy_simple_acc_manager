# Kivy Account Manager

This is a simple account manager application built using Kivy, a Python framework for developing multi-touch applications. The application allows users to create an account, log in, and view account details. User data is stored in a text file (`users.txt`).

## Features

- **Create Account:** Users can create a new account by providing a name, email, and password.
- **Login:** Users can log in with their email and password.
- **View Account Details:** Once logged in, users can view their account details, including the account name, email, and the date the account was created.

## File Structure

- `main.py`: Main application file containing the Kivy application logic and UI flow.
- `database.py`: Contains the `DataBase` class for handling user data storage and validation.
- `my.kv`: Kivy language file defining the UI layout and styling.
- `users.txt`: Text file used for storing user data.

## Requirements

- Python 3.x
- Kivy 2.0.0 or later

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/kivy-account-manager.git
   cd kivy-account-manager
   ```

2. **Create a virtual environment and activate it:**

  ```bash
  # On Windows use `venv\Scripts\activate`
  python -m venv venv
  source venv/bin/activate
  ```

3. **Install the required packages:**
  ```bash
  pip install kivy
  ```
Usage

1. **Run the application:**

  ```bash
  Copiar código
  python main.py
  ```
2. Create a new account:

  Click on "Submit" to create a new account. Ensure all fields are filled correctly.
  
3. Log in:

  Enter your email and password, then click "Login".
  
4. View account details:

  After logging in, your account details will be displayed.

## Code Overview

- `main.py`
The main file that runs the Kivy application. It defines the different screens (create account, login, and main window) and manages the screen transitions.

- `database.py`
This file contains the DataBase class, which handles reading from and writing to the users.txt file. It includes methods for adding new users, validating login credentials, and retrieving user details.

- `my.kv`
A Kivy language file that defines the UI layout for the application. It includes the design for the create account screen, login screen, and main window.

- `users.txt`
A text file used to store user data. Each line in the file represents a user and contains the email, password, name, and account creation date, separated by semicolons.
