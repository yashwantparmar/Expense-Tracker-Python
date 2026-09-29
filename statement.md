# Expense Tracker — Project Statement

## 1. Problem Statement

Managing daily expenses manually can make it difficult to keep track of how much money has been spent and where it has been spent. A simple expense management system can help a user record individual expenses, view recorded entries, calculate total spending, check spending for a particular category, and remove an incorrect or unwanted entry.

The **Expense Tracker** project addresses this problem through a Python-based console application. It provides a simple menu-driven interface through which a user can manage expense records during a program session.

The project is designed as a practical application of Python programming concepts covered in a programming course.

## 2. Scope of the Project

The scope of the current project includes basic expense management operations:

- Adding a new expense.
- Recording the expense category.
- Recording the expense amount.
- Automatically recording the current date and time.
- Viewing all recorded expenses.
- Calculating the total expense.
- Calculating expenses for a selected category.
- Deleting an expense using its displayed number.
- Validating important user inputs.
- Handling invalid numeric input.

The current version stores expenses in an in-memory Python list. Therefore, the data is available only while the program is running and is not permanently stored after the program terminates.

The project does not currently include a database, user authentication, graphical user interface, online synchronization, or permanent file storage.

## 3. Target Users

The primary target users are:

- Students who want to learn basic expense management through a programming project.
- Individuals who want a simple command-line method for recording expenses during a session.
- Beginners learning Python programming concepts through a practical application.

## 4. High-Level Features

### 4.1 Add Expense

The user can enter an expense category and amount. The program validates the amount and records the current date and time.

### 4.2 View Expenses

The user can view all expenses recorded during the current program session. Each record displays its number, category, amount, and date/time.

### 4.3 Calculate Total Expenses

The application processes all recorded expense amounts and displays their combined total.

### 4.4 Category-wise Expenses

The user can enter a category such as `Shopping`. The application then calculates the total amount recorded for that category.

### 4.5 Delete Expense

The application displays expense numbers and allows the user to delete a selected expense by entering its number.

### 4.6 Input Validation

The program checks invalid amount input, rejects non-positive expense amounts, and validates expense numbers used for deletion.

## 5. Functional Requirements

The project must provide the following functional behavior:

1. The system shall allow the user to add an expense.
2. The system shall accept an expense category.
3. The system shall accept and validate an expense amount.
4. The system shall record the date and time of an expense.
5. The system shall display recorded expenses.
6. The system shall calculate the total of all recorded expenses.
7. The system shall calculate the total expense for a selected category.
8. The system shall allow the user to delete a selected expense.
9. The system shall provide an option to exit the application.
10. The system shall display appropriate messages for invalid input.

## 6. Non-Functional Requirements

### Usability
The interface should be simple and menu-driven so users can understand the available operations without complicated instructions.

### Reliability
The program should handle common invalid inputs without unexpectedly terminating. `try-except` blocks are used where numeric conversion can fail.

### Maintainability
The functionality is divided into separate Python functions. This makes individual operations easier to understand and modify.

### Resource Efficiency
The project uses basic Python data structures and built-in functionality. It does not require external packages or a network connection.

## 7. Technical Approach

The project uses a Python list called `expenses` to store expense records.

Each record is stored as a dictionary containing:

- `category`
- `amount`
- `date`

The program uses separate functions for the major operations and a `while` loop for the main menu. Conditional statements determine which function is executed according to the user's choice.

The `datetime` module is used to generate the date and time when an expense is added.

## 8. Expected Outcome

The expected outcome is a working command-line Expense Tracker that can perform the defined expense management operations and demonstrate practical understanding of Python programming concepts.

The project also provides a foundation for future improvements such as permanent storage, reporting, graphical visualization, database integration, and a graphical user interface.

## 9. Project Limitations

The current implementation has the following limitations:

- Expense records are not permanently saved.
- Data is lost when the program stops.
- There is no login or authentication system.
- There is no graphical interface.
- There is no database.
- The current implementation is organized in a single Python source file.
- Automated unit testing is not included in the current version.

## 10. Future Scope

The project can be extended by introducing:

- File-based or database storage.
- Edit/update functionality.
- Monthly and category-based reports.
- Budget management.
- Search and filtering.
- Graphical charts.
- GUI-based interaction.
- Multiple Python modules for improved project structure.
- Automated tests.

