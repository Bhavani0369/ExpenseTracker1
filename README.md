ExpenseTracker :

The Expense Tracker project aims to provide users with a convenient way to track their expenses. The project addresses the common problem of individuals and businesses needing to monitor and manage their spending habits. By developing an expense tracking application, users can easily record and analyse their expenses, helping them make informed financial decisions.


Event Listeners: 
The script listens for various user interactions, including form submissions, expense editing, deletion, and category filtering.
This JavaScript code is part of a simple expense tracker web application. Here's a brief explanation of its main components:

1. Event Listeners :
   - The DOMContentLoaded event ensures the script runs after the HTML has fully loaded.
   - The form submission is handled with the submit event on the expense form (expenseForm). It prevents the default form submission behavior and instead captures the expense details (name, amount, category, and date) and adds them to an array of expenses. It then updates the displayed list of expenses and the total amount.
   - The click event on the expenseList listens for "edit" and "delete" button clicks. 
     - "Delete" removes the corresponding expense.
     - "Edit" pre-fills the form with the selected expense data for modification.
   - The change event on the filterCategory allows filtering expenses by category.

2. Functions :
   - displayExpenses(expenses): This function displays the list of expenses dynamically in a table format, including buttons to edit or delete each expense.
   - updateTotalAmount(): This calculates and updates the total of all expenses displayed.

3. Data Storage :
   - Expenses are stored in an array, and each expense is represented as an object with fields for name, amount, category, and date. Each expense also has a unique ID generated using Date.now().


Adding Expenses: 
When the user submits the form, the new expense (with name, amount, category, and date) is added to an array and displayed in a list.


Expense Display: 
The displayExpenses function dynamically creates and updates the HTML table with the expense details.


Editing & Deleting: Users can edit or delete an expense. Editing allows pre-filled values to be adjusted, while deleting removes the expense from the list.


Filtering by Category: Users can filter the expense list based on the selected category.


Total Calculation: The total amount of all expenses is calculated and displayed whenever changes occur.


This script provides basic expense management functionality with features for adding, viewing, filtering, editing, and deleting expenses.
