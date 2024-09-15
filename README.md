Mortgage Calculation Project
Overview
The Mortgage Calculation project provides a tool for calculating mortgage payments and generating amortization schedules. Utilizing Object-Oriented Programming (OOP) principles, this project is designed to be modular, easy to maintain, and extendable.

Key Features
Calculate Monthly Mortgage Payments: Determines the amount of each monthly payment based on the loan principal, annual interest rate, and loan term.
Generate Amortization Schedule: Provides a detailed schedule of remaining loan balances for each month.
Interactive Console Interface: Collects user input for mortgage parameters and displays the results.
OOP Concepts Applied
1. Classes and Objects
MortgageCalculator: Encapsulates the logic for calculating mortgage payments and remaining balances. Contains methods to compute monthly payments, loan balances, and manage loan parameters.

MortgageReport: Responsible for generating and formatting the output. It uses the MortgageCalculator class to fetch mortgage calculations and print the payment schedule and mortgage details.

Console: Provides a simple interface for reading user input from the console. Ensures that inputs are within specified ranges and handles user prompts.

Main: Entry point of the application. It orchestrates the interaction between the user and the MortgageCalculator and MortgageReport classes.

2. Encapsulation
Private Attributes: The MortgageCalculator class encapsulates loan details like principal, annualInterest, and years. These attributes are only accessed and modified through methods provided by the class.

Public Methods: Methods like calculateMortgage() and printMortgage() in MortgageReport are used to interact with the encapsulated data, ensuring that internal states are managed properly.

3. Inheritance
No explicit inheritance is used in this implementation. All classes are designed to be independent, promoting composition over inheritance.
 
4. Polymorphism
Method Overloading: The Console class demonstrates method overloading with multiple readNumber methods for handling different input scenarios.

Usage
   Start the Application: Execute the Main class.
   Provide Input: Enter the principal amount, annual interest rate, and the loan term when prompted.
   View Results: The application will display the monthly mortgage payment and a detailed payment schedule.
  
Code Structure
   src/com/arijit/
   Console.java - Handles user input.
   MortgageCalculator.java - Core calculations for the mortgage.
   MortgageReport.java - Formats and displays mortgage information.
   Main.java - Entry point for the application.