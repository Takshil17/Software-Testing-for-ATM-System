# ATM System

## Overview
This project is a simulation of an ATM system implemented in C. It allows users to generate a PIN, authenticate using the PIN, and perform basic banking operations such as checking balance, depositing money, withdrawing money, and viewing transaction history. The project demonstrates the use of file handling, dynamic memory allocation, and data structures like linked lists in C.

## Key Features
- **PIN Generation and Authentication**:
  - Generates a 4-digit random PIN.
  - PINs are securely stored in a file (`pin.txt`).
  - Allows users to authenticate using a valid PIN.

- **Banking Operations**:
  - **Check Balance**: Displays the current account balance.
  - **Deposit Money**: Increases the account balance by a specified amount.
  - **Withdraw Money**: Decreases the account balance if sufficient funds are available.

- **Transaction History**:
  - Stores the last 10 transactions in a queue using a linked list.
  - Displays the transaction history, including deposits and withdrawals.

## File Structure
- **Source Code**: The entire project is implemented in a single C source file.
- **PIN File**: The `pin.txt` file stores the generated PINs for authentication.

## How It Works
1. **PIN Generation**:
   - A random 4-digit PIN is generated using the `rand()` function.
   - The PIN is stored in the `pin.txt` file for future use.
2. **Authentication**:
   - The user enters a PIN, which is verified against the `pin.txt` file.
   - On successful authentication, the user can access the ATM menu.
3. **Banking Operations**:
   - Users can check their balance, deposit money, or withdraw money.
   - Transactions are logged and maintained in a queue structure.
4. **Transaction History**:
   - The history stores up to 10 transactions.
   - Older transactions are removed automatically when the limit is reached.

## Tools and Technologies
- **Programming Language**: C
- **Compiler**: GCC or any compatible C compiler

## Example Usage
1. Generate a PIN and note it down.
2. Use the same PIN to access the ATM menu.
3. Perform operations like depositing and withdrawing money.
4. View transaction history for recent activities.
