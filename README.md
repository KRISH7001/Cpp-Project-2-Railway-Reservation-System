📁 Project Overview This project contains a simple C++ program that demonstrates fundamental object-oriented programming concepts such as classes, objects, static members, constructors/destructors, encapsulation, and array-based record management. The program included is:

Railway Reservation System – Manages a database of train records, allowing you to add, display, and search trains by train number.

📌 Program Included

Railway Reservation System File: Railway_Reservation_System.cpp

This program lets you build up a simple in-memory database of trains and interact with it through a menu. It uses:

A Train class with attributes (train number, name, source, destination, time) encapsulated as private members
A static member (trainCount) tracked via the constructor and destructor to count how many Train objects currently exist
Default and parameterized constructors, plus a destructor
Getters and setters for every attribute
C-style strings (char[]) manipulated safely with <cstring> functions such as strcpy
A RailwaySystem class that owns a fixed-size array of Train objects (Train trains[100]) and manages adding, displaying, and searching records
A menu-driven interface using switch / do-while
User input using cin and cin.getline

On startup, the program asks you to enter at least 3 initial train records before showing the main menu:

1. Add New Train Record
2. Display All Train Records
3. Search Train by Number
4. Exit

Searching works by scanning the array for a matching trainNumber:

cpp
for (int i = 0; i < totalTrains; i++)
{
    if (trains[i].getTrainNumber() == number)
    {
        // train found
    }
}

🛠️ Requirements You can run this program using:

GCC / G++ Compiler
Visual Studio Code

▶️ How to Run Using G++

g++ -o Railway_Reservation_System Railway_Reservation_System.cpp
./Railway_Reservation_System

🎯 Learning Objectives This project helps practice:

Basic C++ syntax
Classes, objects, and encapsulation
Static class members
Constructors and destructors
Getters and setters
Working with C-style strings (char[], strcpy)
Arrays of objects
Input and output using cin and cout
Conditional statements and loops (switch, do-while, for)
Menu-driven program design
Basic problem solving

📂 Project Structure

Railway-Reservation-System-Project/
│
├── README.md
└── Railway_Reservation_System.cpp

🔹 Project Explanation Video 👉 Explanation Video: [Add your video link here]

👨‍💻 Author KRISH SAPARIYA This repository is intended for learning and practicing fundamental C++ programming concepts, especially classes, objects, static members, constructors/destructors, and array-based record management.
