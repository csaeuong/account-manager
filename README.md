# Account Manager

## Objective

The objective of this project is to create a simple password manager that allows users to securely create accounts and log in. Passwords are protected by hashing with SHA-256, ensuring that raw passwords are never stored directly. This project demonstrates fundamental cybersecurity concepts such as password handling, hashing, and authentication logic.

### Skills Learned

- Python programming fundamentals (functions, loops, conditionals)
- User authentication flow (account creation and login system)
- Password security (hashing with SHA-256 instead of storing plain text)
- Using external libraries (hashlib for hashing, getpass for secure input)
- Error handling in user interaction (validating username/password correctness)
- Building a CLI (Command-Line Interface) program

### Tools Used

- Python 3 (main programming language)
- hashlib (for password hashing with SHA-256)
- getpass (for hidden password input)

  ## Code 
<img width="1920" height="1040" alt="Passgen" src="https://github.com/user-attachments/assets/d59a6c17-4026-463a-a037-88096a027dbc" />

### Quick Reference

- import hashlib - loads the Python library for hashing algorithms (used for password security).
- import getpass - allows password input without showing characters on the screen.
- password_manager = {} - creates an empty dictionary to store usernames and hashed passwords.
- def create_account(): - defines a function that lets users create a new account.
- username = input("...") - asks the user for a username.
- password = getpass.getpass("...") - asks the user for a password (hidden).
- hashlib.sha256(password.encode()).hexdigest() - converts the password into a secure SHA-256 hash.
- password_manager[username] = hashed_password - saves the username and its hashed password in the dictionary.
- print("Account created successfully") - confirms the account creation.
- def login(): - defines a function that lets a user log in.
- if username in password_manager.keys() - checks if the entered username exists.
- and password_manager[username] == hashed_password - checks if the entered password matches the stored hash.
- print("Login Successful!") - runs if both username and password are correct.
- else: print("Invalid username or password.") - runs if login fails.
- def main(): - defines the main program loop.
- while True: - creates an infinite loop until the user chooses to exit.
- if - runs a block of code only if the condition is true.
- elif - runs if the first if condition is false, but this one is true.
- else - runs if none of the above conditions are true.
- break - exits the loop and ends the program.
- if __name__ == "__main__": - ensures the program runs only when executed directly.

## Project Reflection

I learned a lot while working on this project. I had to research several concepts along the way to fully understand how everything worked, especially around password hashing and secure user input. The tutorial I followed was very helpful in guiding me through the process, and it showed me how different pieces of Python fit together to build a functional program.

Even though I am still new to coding, I recognize that every developer has to start somewhere. This project was a great step forward in my learning journey, and it gave me more confidence in working with Python and cybersecurity concepts. My goal is to eventually reach the point where I can design and build my own scripts entirely from scratch — and this project was an important milestone toward that goal.
