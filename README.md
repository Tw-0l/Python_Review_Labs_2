# Python Projects

## Project 1: Lists

This project demonstrates various operations on lists, such as summing items, finding the largest number, filtering even numbers, and slicing the list.

### Code

```python
# Given list
lst = [5, 4, 17, 19, 30, 2, 7, 10, 45]

# Q1: Sum all the items in the list
total = 0
for n in lst:
    total += n
print("Sum of all items in the list:", total)

# Q2: Get the largest number from the list
max_number = max(lst)
print("The largest number is:", max_number)

# Q3: Use list comprehension to create a new list containing only even numbers
even_numbers = [n for n in lst if n % 2 == 0]
print("Even numbers:", even_numbers)

# Q4: Use list slicing to get a new list from the start to the 5th element
new_lst = lst[:5]
print("New list from start to 5th element:", new_lst)
```

### Output

```
Sum of all items in the list: 139
The largest number is: 45
Even numbers: [4, 30, 2, 10]
New list from start to 5th element: [5, 4, 17, 19, 30]
```

## Project 2: Phone Book Dictionary

This project is a phone book program that receives a phone number and returns the name of the owner. It handles invalid inputs and numbers not found in the phone book.

### Code

```python
def find_owner(phone_book, num):
    if num.isdigit() and len(num) == 10:
        owner = phone_book.get(num)
        if owner:
            print("Owner's name is", owner)
        else:
            print("Sorry, the number is not found")
    else:
        print("This is an invalid number.")

phone_book = {
    '1111111111': 'Amal',
    '2222222222': 'Mohammed',
    '3333333333': 'Khadijah',
    '4444444444': 'Abdullah',
    '5555555555': 'Rawan',
    '6666666666': 'Faisal',
    '7777777777': 'Layla',
}

num = input("Enter a 10-digit phone number: ")
find_owner(phone_book, num)
```

### Output

The output will vary based on the input. For example:

```
Enter a 10-digit phone number: 1111111111
Owner's name is Amal

Enter a 10-digit phone number: 1234567890
Sorry, the number is not found

Enter a 10-digit phone number: abcdefghij
This is an invalid number.
```

## Project 3: Try and Except

This project handles user inputs for their name, age, and shopping details. It includes error handling and optional repetition of the process.

### Code

```python
while True:
    try:
        name = input("Enter your name: ")
        age = int(input("Enter your age: "))

        if age < 0:
            print("Wrong age value, you cannot enter a value less than 0")
        elif 0 <= age <= 6:
            print("Kid")
        else:
            total_cost = 0
            num_items = int(input("Enter number of items you want to buy: "))
            for i in range(num_items):
                item_name = input("Enter item name: ")
                item_price = float(input("Enter item price: "))
                item_quantity = int(input("Enter item quantity: "))
                item_cost = item_price * item_quantity
                total_cost += item_cost
                print("Item cost:", item_cost, " Total cost:", total_cost)
            
            if total_cost > 200:
                total_cost *= 0.8  
                print("You've got a 20% discount!")
                print("Total cost after discount:", total_cost)
        
        repeat = input("Do you want to repeat the process? (yes/no): ")
        if repeat.lower() != "yes":
            break

    except ValueError:
        print("Invalid input! Please enter a valid value.")
```

### Output

The output will vary based on the input. For example:

```
Enter your name: Abdullah
Enter your age: 7
Enter number of items you want to buy: 2
Enter item name: Book
Enter item price: 15.50
Enter item quantity: 3
Item cost: 46.5  Total cost: 46.5
Enter item name: Pen
Enter item price: 1.25
Enter item quantity: 10
Item cost: 12.5  Total cost: 59.0
Do you want to repeat the process? (yes/no): no
```

## Conclusion

These projects demonstrate basic Python programming concepts, including list operations, dictionary usage, and error handling with `try` and `except` blocks. Each project solves a specific problem and provides practice in writing Python code.
