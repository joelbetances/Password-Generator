# Password Generator

A powerful and essential tool for cybersecurity, this Password Generator creates strong and secure passwords by combining letters, numbers, and symbols. This project demonstrates the use of lists, loops, and the random module in Python.

## How It Works

1. The user specifies the number of letters, symbols, and numbers they want in their password.
2. The program generates a password with the specified characters.
3. The characters are shuffled to ensure randomness.
4. The final password is displayed to the user.

## The Code

Here is the Python code for the Password Generator:

```python
# Password Generator Project

import random

# ASCII Art
print("""
   ____                                      _     _____                          
  / __ \                                    | |   |  __ \                         
 | |  | |_ __ __ _  __ _  ___  _ __ ___   __| |   | |__) | __ _____  ___   _      
 | |  | | '__/ _` |/ _` |/ _ \| '__/ _ \ / _` |   |  ___/ '__/ _ \ \/ / | | |     
 | |__| | | | (_| | (_| | (_) | | | (_) | (_| |   | |   | | | (_) >  <| |_| |     
  \____/|_|  \__,_|\__, |\___/|_|  \___/ \__,_|   |_|   |_|  \___/_/\_\\__, |     
                    __/ |                                                __/ |     
                   |___/                                                |___/      
""")

# Lists of characters to be used in the password
letters = [
    'a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 
    'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', 'A', 'B', 'C', 'D', 'E', 'F', 
    'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 
    'W', 'X', 'Y', 'Z'
]
numbers = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
symbols = ['!', '#', '$', '%', '&', '(', ')', '*', '+']

# Welcome message
print("Welcome to the PyPassword Generator! Your secure password awaits. 🔒")

# User input for password requirements
nr_letters = int(input("How many letters would you like in your password?\n")) 
nr_symbols = int(input("How many symbols would you like?\n"))
nr_numbers = int(input("How many numbers would you like?\n"))

# Hard Level - Randomly select characters and shuffle them
password_list = []

# Add random letters to the password list
for char in range(1, nr_letters + 1):
    password_list.append(random.choice(letters))

# Add random symbols to the password list
for char in range(1, nr_symbols + 1):
    password_list.append(random.choice(symbols))

# Add random numbers to the password list
for char in range(1, nr_numbers + 1):
    password_list.append(random.choice(numbers))

# Debug: Print the list before shuffling
print(f"Password list before shuffling: {password_list}")

# Shuffle the password list to ensure randomness
random.shuffle(password_list)

# Debug: Print the list after shuffling
print(f"Password list after shuffling: {password_list}")

# Combine the list items into a single string
password = ""
for char in password_list:
    password += char

# Display the final password
print(f"Your secure password is: {password}")
# Password Generator

A powerful and essential tool for cybersecurity, this Password Generator creates strong and secure passwords by combining letters, numbers, and symbols. This project demonstrates the use of lists, loops, and the random module in Python.

## How It Works

1. The user specifies the number of letters, symbols, and numbers they want in their password.
2. The program generates a password with the specified characters.
3. The characters are shuffled to ensure randomness.
4. The final password is displayed to the user.

## The Code

Here is the Python code for the Password Generator:

```python
# Password Generator Project

import random

# ASCII Art
print("""
   ____                                      _     _____                          
  / __ \                                    | |   |  __ \                         
 | |  | |_ __ __ _  __ _  ___  _ __ ___   __| |   | |__) | __ _____  ___   _      
 | |  | | '__/ _` |/ _` |/ _ \| '__/ _ \ / _` |   |  ___/ '__/ _ \ \/ / | | |     
 | |__| | | | (_| | (_| | (_) | | | (_) | (_| |   | |   | | | (_) >  <| |_| |     
  \____/|_|  \__,_|\__, |\___/|_|  \___/ \__,_|   |_|   |_|  \___/_/\_\\__, |     
                    __/ |                                                __/ |     
                   |___/                                                |___/      
""")

# Lists of characters to be used in the password
letters = [
    'a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 
    'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', 'A', 'B', 'C', 'D', 'E', 'F', 
    'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 
    'W', 'X', 'Y', 'Z'
]
numbers = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
symbols = ['!', '#', '$', '%', '&', '(', ')', '*', '+']

# Welcome message
print("Welcome to the PyPassword Generator! Your secure password awaits. 🔒")

# User input for password requirements
nr_letters = int(input("How many letters would you like in your password?\n")) 
nr_symbols = int(input("How many symbols would you like?\n"))
nr_numbers = int(input("How many numbers would you like?\n"))

# Hard Level - Randomly select characters and shuffle them
password_list = []

# Add random letters to the password list
for char in range(1, nr_letters + 1):
    password_list.append(random.choice(letters))

# Add random symbols to the password list
for char in range(1, nr_symbols + 1):
    password_list.append(random.choice(symbols))

# Add random numbers to the password list
for char in range(1, nr_numbers + 1):
    password_list.append(random.choice(numbers))

# Debug: Print the list before shuffling
print(f"Password list before shuffling: {password_list}")

# Shuffle the password list to ensure randomness
random.shuffle(password_list)

# Debug: Print the list after shuffling
print(f"Password list after shuffling: {password_list}")

# Combine the list items into a single string
password = ""
for char in password_list:
    password += char

# Display the final password
print(f"Your secure password is: {password}")

