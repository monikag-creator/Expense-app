# Expense Sharing App (Google Pay Style)

A command-line expense splitting tool that tracks shared group expenses and calculates exactly who owes whom, similar to Splitwise or Google Pay's expense-sharing feature.

## Problem Statement
Splitting shared expenses among friends, roommates, or travel groups is often done manually — leading to confusion, forgotten payments, and disputes. Most people resort to mental math or messy spreadsheets to track who paid for what, which doesn't scale well for frequent group outings or trips. A simple, structured tool is needed to track group expenses and settle balances accurately.

## Tech Stack
- **Language:** Python
- **Data Structures:** Dictionaries, Lists for transaction and balance tracking
- **Display:** PrettyTable (formatted CLI output)
- **Core Logic:** Custom balance-settlement algorithm

## Approach
1. Designed a command-line interface allowing users to add group members and log expenses.
2. Implemented support for both **equal splits** (divided evenly among all members) and **custom splits** (user-defined amounts per person).
3. Built a real-time balance tracking system that calculates net amounts owed between every pair of users.
4. Added a transaction history log displaying payer name, amount, description, and date for full transparency.
5. Used PrettyTable to render clean, readable tables of balances and transaction history directly in the terminal.

## Business Solution
This project demonstrates the core logic behind consumer expense-sharing features found in apps like Google Pay, Splitwise, and PhonePe. The underlying balance-settlement algorithm can be extended into a full mobile or web application for group trip planning, roommate expense management, or event cost-sharing — a common pain point for any group of people managing shared finances.

## How to Run
```bash
git clone https://github.com/monikag-creator/Expense-app.git
cd Expense-app
pip install -r requirements.txt
python main.py
```

## Author
**Monika G** — [LinkedIn](https://www.linkedin.com/in/monika-g-4a2904388) | [GitHub](https://github.com/monikag-creator)
