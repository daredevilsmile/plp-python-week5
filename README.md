# PLP Python Week 5

## Password Generator & Your Own Module

This project contains the solutions for the PLP Python Week 5 assignment.

### Files

- `password_generator.py` - generates random passwords using Python random and string modules.
- `helpers.py` - contains reusable functions for calculating tables and creating a welcome message.
- `main.py` - imports and uses the functions from helpers.py.
- `screenshots/` - contains screenshots showing the required program outputs.

### Question 1: Password Generator

The make_password() function generates passwords containing letters and digits.

The default password length is 8, while make_password(12) generates a 12-character password.

The program was run twice. The passwords are different because random.choice() selects characters randomly, while the lengths remain 8 and 12.

### Question 2: Own Module

The helpers.py module contains tables_needed(people, seats), which uses math.ceil() to round up the number of tables required, and welcome(name), which returns a welcome message.

### Why does 3 not appear when running main.py?

The line if __name__ == "__main__": makes sure the test code in helpers.py runs only when helpers.py is executed directly.

When helpers.py is imported by main.py, its __name__ is "helpers", not "__main__". Therefore the test print statement does not run during the import.

When helpers.py is run directly, the condition is true and the output is 3.

### Expected Output

Running main.py:

Welcome to PLP, Amina!
8
4

Running helpers.py directly:

3

### Learning Outcomes

- Using Python standard library modules
- Using random.choice()
- Using math.ceil()
- Creating and importing a custom Python module
- Using if __name__ == "__main__":
- Sharing a Python project through a public GitHub repository
