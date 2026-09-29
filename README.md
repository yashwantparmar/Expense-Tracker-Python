# Expense Tracker

## Project Overview

**Expense Tracker** is a simple Python-based console application designed to help users record, view, calculate, organize, and delete their daily expenses.

The project applies basic Python programming concepts such as variables, input/output, conditional statements, loops, functions, lists, dictionaries, exception handling, and the `datetime` module.

The application provides a menu-driven workflow so that the user can select an operation and perform it directly from the terminal.

## Features

The current implementation provides the following major functional modules:

1. **Add Expense**
   - Accepts an expense category from the user.
   - Accepts the expense amount.
   - Supports amounts entered with commas, such as `1,000`.
   - Rejects zero or negative amounts.
   - Handles invalid numeric input using exception handling.
   - Automatically records the current date and time.

2. **View Expenses**
   - Displays all recorded expenses.
   - Shows an expense number, category, amount, and date/time.
   - Displays a message when no expenses are available.

3. **Calculate Total Expenses**
   - Calculates the total amount of all recorded expenses.
   - Displays the calculated total to the user.

4. **Category-wise Expenses**
   - Allows the user to enter a category.
   - Calculates the total amount spent in that category.

5. **Delete Expense**
   - Displays the existing expenses with numbers.
   - Allows the user to select an expense number.
   - Deletes the selected expense from the list.
   - Validates the entered expense number.

6. **Exit**
   - Allows the user to safely exit the Expense Tracker.

## Technologies / Tools Used

- **Python 3**
- `datetime` module
- Python Lists
- Python Dictionaries
- Functions
- Loops (`while`, `for`)
- Conditional statements (`if`, `elif`, `else`)
- Exception handling (`try-except`)
- Git and GitHub for version control

## Installation and Setup

### Prerequisites

- Python 3.x installed on the computer.
- A terminal, command prompt, or Python IDE such as VS Code, IDLE, or PyCharm.

### Steps

1. Clone or download the GitHub repository.
2. Open the project folder in a terminal.
3. Run the Python program using:

```bash
python expense_tracker.py
```

If the Python command is configured as `python3`, use:

```bash
python3 expense_tracker.py
```

> Replace `expense_tracker.py` with the actual Python filename used in the repository.

No external Python packages are required because the project uses Python's built-in `datetime` module.

## How to Use

After starting the program, the following menu is displayed:

```text
=====EXPENSE TRACKER=====
1. Add Expense
2. View Expenses
3. Calculate Total Expenses
4. Category-wise Expenses
5. Delete Expense
6. Exit
```

Enter the number corresponding to the required operation.

### Example: Adding an Expense

```text
Enter your choice: 1

=====ADD EXPENSE=====
Enter the expense category(shopping): Shopping
Enter the expense amount: ₹ 7800
Expense added successfully!
```

### Example: Viewing Expenses

```text
=====EXPENSES=====
1. Shopping - ₹7800.0 - 29-09-2026 13:00:00
```

The exact date and time depend on when the expense is added.

## Input Validation and Error Handling

The program includes validation for important user inputs.

- Expense amount must be greater than zero.
- Non-numeric expense amounts are rejected.
- Commas in numeric amounts are removed before conversion.
- Invalid delete selections are handled.
- The program checks whether expenses exist before viewing or deleting them.
- Invalid main-menu choices produce an error message and return the user to the menu.

## Testing Instructions

The project can be tested manually by running the program and checking each menu option.

### Test Cases

| Test Case | Input / Action | Expected Result |
|---|---|---|
| Add valid expense | Category = Shopping, Amount = 7800 | Expense is added successfully |
| Add amount with comma | Amount = 1,500 | Amount is accepted as 1500 |
| Add invalid amount | Amount = abc | Error message is displayed |
| Add negative amount | Amount = -500 | Amount is rejected |
| View with no data | Select View Expenses initially | "No expenses found." is displayed |
| Calculate total | Add multiple expenses and select option 3 | Correct total is displayed |
| Category-wise total | Enter an existing category | Total for that category is displayed |
| Delete valid expense | Enter a valid expense number | Selected expense is deleted |
| Delete invalid number | Enter a number outside the list | Invalid expense number message is displayed |
| Exit | Select option 6 | Program exits |

## Project Scope

The current project focuses on basic personal expense management through a console application. It is suitable for recording expenses during a program session, viewing them, calculating totals, checking category-wise spending, and deleting records.

The current implementation does **not** provide permanent storage, login/authentication, graphical interface, database integration, or online synchronization.

## Current Technical Structure

The submitted code currently uses a single Python source file with multiple functions.

The main components are:

- `add_expense()`
- `view_expenses()`
- `calculate_total_expenses()`
- `category_wise_expenses()`
- `delete_expense()`
- Main menu loop

For a future expanded version, these components can be separated into multiple files/modules.

## Future Enhancements

Possible future improvements include:

- Saving expenses permanently using a file or database.
- Adding an edit/update expense option.
- Adding monthly and daily expense reports.
- Adding budget limits.
- Adding graphical charts.
- Adding a graphical user interface.
- Adding search and filtering.
- Separating the project into multiple Python modules.
- Adding automated unit tests.

## Academic Relevance

This project is relevant to a Python programming course because it demonstrates practical use of programming concepts including functions, lists, dictionaries, loops, conditions, input/output, exception handling, and modules.

## Author

**Expense Tracker Project – By Yashwant Parmar**

