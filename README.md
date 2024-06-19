---

# Shopping Program

---

This program allows users to input their name and age, determine if they are a "Kid" based on their age, and then calculate the total cost of items they want to buy. The program also applies a discount if the total cost exceeds a certain amount. Additionally, the program can handle unexpected inputs and provides an option to repeat the process.

## Features

1. **Name and Age Input**: 
   - Asks the user to enter their name.
   - Asks the user to enter their age.
   - If the age is less than 0, prints an error message.
   - If the age is between 0 and 6, prints "Kid".

2. **Shopping Process**: 
   - If the user's age is greater than 6, it proceeds to the shopping process.
   - Initializes `total_cost` to 0.
   - Asks the user for the number of items they want to buy.
   - For each item, asks for the item name, price, and quantity.
   - Calculates the cost of each item and adds it to `total_cost`.
   - Prints the cost of each item and the running total cost.
   - If the total cost exceeds 200, applies a 20% discount and notifies the user.

3. **Error Handling**: 
   - Catches invalid inputs and prompts the user to enter valid values.

4. **Loop to Repeat Process**: 
   - After each iteration, asks the user if they want to repeat the process.
   - If the user inputs "yes", the process starts again from the beginning.
   - If the user inputs anything other than "yes", the program exits.

## How to Run

1. Ensure you have Python installed on your machine.
2. Copy the program code into a Python file, e.g., `shopping_program.py`.
3. Run the program by executing `python shopping_program.py` in your terminal or command prompt.

## Example Usage

```plaintext
Enter your name: Abdullah
Enter your age: 30
Enter number of items you want to buy: 2
Enter item name: Book
Enter item price: 15.50
Enter how many one you want: 3
Item cost: 46.5  Total cost:  46.5
Enter item name: Pen
Enter item price: 1.20
Enter how many one you want: 10
Item cost: 12.0  Total cost:  58.5
Do you want to repeat the process? (yes/no): yes
Enter your name: Yousef
Enter your age: 5
Kid
Do you want to repeat the process? (yes/no): no
```

## Note

- Make sure to enter valid numerical values for age, item price, and item quantity.
- If an invalid input is detected, the program will prompt you to enter a valid value and continue.

