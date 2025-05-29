Simple C++ Banking System

This is a simple object-oriented banking system written in C++. It supports account creation, login
with PIN, deposit/withdrawal, fixed deposit (FDR), and monthly savings plans (DPS). User data is
stored in a file (accounts.txt) for persistence.

Features
- Create bank accounts with a 4-digit PIN
- Secure login using masked PIN input
- Deposit and withdraw money
- Open Fixed Deposit Receipt (FDR) with 10% interest
- Open Deposit Pension Scheme (DPS) with 6% interest
- Display account details
- Persistent data storage using file I/O

Requirements
- C++ compiler (e.g., g++, MSVC)
- Windows (for _getch() input masking)
- You can replace _getch() with platform-independent alternatives for portability
- accounts.txt will be created automatically if it doesn't exist

How to Compile
Use your preferred C++ compiler. For example, with g++:
g++ -o BankSystem main.cpp
Run the executable:
./BankSystem

File Structure
main.cpp -> Main program and menu interface
accounts.txt -> Stores account data (auto-created)

Account Data Format
Stored in accounts.txt using | - separated values:
Name|AccountNumber|PIN|Balance|FDRAmount|DPSAmount
Example:
Alif|1001|1234|5000.00|0.00|0.00

Limitations
- Only supports up to 10 users (MAX_USERS = 10)
- Platform-specific _getch() for PIN masking
- No encryption for saved PINs
- Basic error handling (can be improved)

To Do
- Modularize code into multiple files
- Use OOP principles more deeply (e.g., FDR/DPS as classes)
- Improve input validation
- Add PIN encryption
- Cross-platform support (Linux/Mac)

License
This project is open for educational use and practice. Feel free to modify and expand it.
Author:
MD Mahamudul Hasan (MHT)
