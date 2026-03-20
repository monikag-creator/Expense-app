# Expense-app
Google Pay Expense Sharing
# Expense Tracker
A simple command-line expense splitting tool built with Python. Split bills equally or by custom amounts, track balances, and view transaction history — right from your terminal.

## Features
- **Multi-user support** — Add any number of users at startup
- **Equal split** — Automatically divides expenses evenly among all users
- **Custom split** — Manually assign specific amounts to each user
- **Balance tracking** — See who owes whom at a glance
- **Transaction history** — Review all past expenses with descriptions
- **Clean table output** — Balances displayed using `PrettyTable`

## Requirements
- Python 3.x
- [`prettytable`](https://pypi.org/project/prettytable/)
Install the dependency with:
```bash
pip install prettytable
```

## Getting Started
1. **Clone or download** this repository.
2. **Run the script:**
```bash
python expense-app.py
```

3. **Enter the number of users** and their names when prompted.

## Usage
Once the app starts, you'll see this menu:
```
1. Add Expense
2. Show Balances
3. Show Transactions
4. Exit
```

### Adding an Expense
Choose option `1` and fill in:
- **Payer name** — who paid the bill
- **Total amount** — the full expense amount
- **Description** — e.g., "Dinner", "Groceries"
- **Split type** — `equal` or `custom`

**Equal split example:**
```
Enter payer name: Alice
Enter total amount: 300
Enter expense description: Dinner
Split type (equal/custom): equal
```

**Custom split example:**
```
Split type (equal/custom): custom
Enter amount for Alice: 0
Enter amount for Bob: 150
Enter amount for Charlie: 150
```

### Viewing Balances
Option `2` shows a table like:
```
+----------+---------+
|   User   | Balance |
+----------+---------+
|  Alice   |  200.0  |
|   Bob    | -100.0  |
| Charlie  | -100.0  |
+----------+---------+
```
- **Positive balance** → the user is owed money
- **Negative balance** → the user owes money

### Transaction History
Option `3` lists all recorded expenses:
```
Transaction History
Alice paid ₹300 for Dinner
Bob paid ₹500 for Hotel
```
---

## Project Structure
```
├── README.md                                        # Project documentation
├── google_expense_sharing-checkpoint.ipynb          # Jupyter Notebook (checkpoint backup)
└── google_expense_sharing_checkpoint                # Checkpoint directory
```

## License

This project is open source and free to use.
