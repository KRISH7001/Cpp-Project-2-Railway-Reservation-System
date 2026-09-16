📁 Project Overview

This project contains a simple C++ program that demonstrates fundamental object-oriented programming concepts such as classes, objects, encapsulation, and static members. The program included is:

Railway Reservation System – Lets you add train records, view all stored trains, and search for a specific train by its train number.
📌 Program Included
1. Railway Reservation System

File: Railway_Reservation_System.cpp

This program lets you manage a simple in-memory train database, interacting through a menu. It uses:

A Train class with attributes (train number, name, source, destination, time) encapsulated as private members
Encapsulation: all data fields are private, accessed only through public getters and setters
Default and parameterized constructors, plus a destructor
A static int trainCount shared across all Train objects, tracking how many currently exist — incremented in the constructors and decremented in the destructor
A RailwaySystem class that owns a fixed-size array of Train objects (trains[100]), managing addition, display, and search
A menu-driven interface using switch / do-while
User input using cin and cin.getline

The main menu looks like this:

1. Add New Train Record
2. Display All Train Records
3. Search Train by Number
4. Exit

Each Train object stores its own details and knows how to display itself:

cpp
// Called on each Train object stored in the RailwaySystem array:
trains[i].displayTrainDetails();
addTrain() fills the next free slot in the array, up to a maximum of 100 trains
displayAllTrains() loops through every stored train and prints its details
searchTrainByNumber() does a linear scan through the array, comparing each train's number against the one entered
🛠️ Requirements

You can run this program using:

GCC / G++ Compiler
Visual Studio Code
▶️ How to Run

Using G++:

bash
g++ Railway_Reservation_System.cpp -o railway_system
./railway_system
🎯 Learning Objectives

This project helps practice:

Basic C++ syntax
Classes, objects, and encapsulation
Constructors and destructors
Static class members
Getters and setters
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
🔹 Project Explanation Video

👉 Explanation Video:

https://drive.google.com/file/d/1qvLnt-lkMXlM8mCTPnaRAShy7c4XC2mf/view?usp=sharing

👨‍💻 Author

Krish Sapariya
