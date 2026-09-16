## 📁 Project Overview

This project contains a simple C++ program that demonstrates fundamental
object-oriented programming concepts such as classes, objects,
inheritance, polymorphism, and encapsulation. The program included is:

- **Banking System** – Lets you create different types of bank accounts,
  perform deposits/withdrawals, calculate interest, and look up account
  information.

## 📌 Program Included

### 1. Banking System
**File:** `banking-system.cpp`

This program lets you manage a simple in-memory bank made up of
different account types, interacting through a menu. It uses:

- A `BankAccount` base class with attributes (account number, holder
  name, balance) encapsulated as protected members
- Three derived classes — `SavingsAccount`, `CheckingAccount`, and
  `FixedDepositAccount` — each inheriting from `BankAccount`
- **Polymorphism**: `displayAccountInfo()` and `calculateInterest()` are
  declared `virtual` in the base class and `override`n in each derived
  class (using `override`), then called through a `BankAccount*` pointer
  so the correct version runs automatically for each account type
- Default and parameterized constructors, plus a virtual destructor
- Getters and setters for every attribute
- A `Bank` class that owns an array of `BankAccount*` pointers
  (`accounts[100]`), managing account creation, lookup, and display
- A menu-driven interface using `switch` / `do-while`
- User input using `cin` and `cin.getline`

The main menu looks like this:

```
1. Create Account
2. Deposit
3. Withdraw
4. Calculate Interest
5. Display Account Info (by number)
6. Display All Accounts
7. Exit
```

Each account type behaves differently for the same operation — a good
example of polymorphism in action:

```cpp
// Called through a base class pointer — the actual (derived) type
// decides what happens:
acc->withdraw(amount);
```

- `SavingsAccount` earns interest: `balance * (interestRate / 100.0)`
- `CheckingAccount` allows withdrawals into an overdraft, up to
  `overdraftLimit`
- `FixedDepositAccount` locks funds for its `term` (in months) and
  refuses withdrawals until maturity, earning:
  `balance * (interestRate / 100.0) * (term / 12.0)`

## 🛠️ Requirements

You can run this program using:

- GCC / G++ Compiler
- Visual Studio Code

## ▶️ How to Run

Using G++:

## 🎯 Learning Objectives

This project helps practice:

- Basic C++ syntax
- Classes, objects, and encapsulation
- Inheritance (base class + multiple derived classes)
- Polymorphism (virtual functions, `override`, base-class pointers)
- Constructors and destructors
- Getters and setters
- Arrays of pointers to a base class
- Input and output using `cin` and `cout`
- Conditional statements and loops (`switch`, `do-while`, `for`)
- Menu-driven program design
- Basic problem solving

## 📂 Project Structure

```
Banking-System-Project/
│
├── README.md
└── banking-system.cpp
```

## 🔹 Project Explanation Video

👉 Explanation Video: 

https://drive.google.com/file/d/1qvLnt-lkMXlM8mCTPnaRAShy7c4XC2mf/view?usp=sharing

## 👨‍💻 Author

**Krish Sapariya**
