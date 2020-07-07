# CECS-277-LAB-2-Inheritance
CECS 277
LAB ASSIGNMENT 2
Assigned date: 9/4
Due date: Monday 9/16
50 points

Objectives

    Implement interface and inheritance
    Implement polymorphism

Prelab

    Read chapter 9 - Inherintance and interfaces
    Review lecture notes on inheritance

Payroll System Using Inheritance and Polymorphism

1. Implement an interface called EmployeeInfo with the following constant variables:

    FACULTY_MONTHLY_SALARY = 5000.00
    STAFF_MONTHLY_HOURS_WORKED = 150

2. Implement an abstract class Employee with the following requirements:

    Attributes
        last name (String)
        first name (String)
        ID number (String)
        Sex - M or F
        Birth date - Use the Calendar Java class to create a date object
    Default argument constructor and argument constructors.
    Public methods
        toString - returning a string with the following format:
        ID Employee number :_________
        Employee name: __________
        Birth date: _______
        mutators and accessors
        abstract method monthlyEarning that returns the monthly earning.

3. Implement a class called Staff extending from the class Employee with the following requirements:

    Attribute
        Hourly rate
    Default argument and argument contructors
    Public methods
        get and set
        The method Earning returns monthly salary (hourly rate times 160)
        toString - returning a string with the following format:
        ID Employee number :_________
        Employee name: __________
        Birth date: _______
        Full Time
        Monthly Salary: _________

Implelment a class Education with the following requirements:

    Attributes
        Degree (MS or PhD )
        Major (Engineering, Chemistry, English, etc ... )
        Research (number of researches)
    Default argument and argument constructors.
    Public methods
        get and set

Implement a class Faculty extending from the class Employee with the following requirements:

    Attributes
        Level (Use enum Java)
        "AS": assistant professor
        "AO": associate professor
        "FU": professor
        Education object
    Default argument and argument constructor
    Public methods
        mutators and accessors
        The method monthlyEarning returns monthly salary based on the faculty's level.
        AS - faculty monthly salary
        AO - 1.5 times faculty monthly salary
        FU - 2.0 times faculty monthly salary
        toString - returning a string with the following format:
        ID Employee number :_________
        Employee name: __________
        Birth date: _______
        XXXXX Professor where  XXXXX can be Assistant, Associate or Full
        Monthly Salary: _________

Implement a class called Partime extending from the class Staff with the following requirements:

    Attributes
        Hours worked per week
    Default argument and argument constructors
    Public methods
        mutators and accessors
        The method monthlyEarning returns monthly salary . The monthly salary is equal to hourly rate times the hours worked in four weeks.
        toString - returning a string with the following format:
        ID Employee number :_________
        Employee name: __________
        Birth date: _______
        Hours works per month: ______
        Monthly Salary: _________

mplement a test driver program that creates a one-dimensional array of class Employee to store the objects Staff, Faculty and Partime.

Using polymorphism, display the following outputs:

a. Employee information using the method toString

    Staff
    Faculty
    Part-time

b. Total monthly salary for all the part-time staff .
c. Total monthly salary for all employees.
d. Display all employee information ascending by employee id using interface Comparer
e. Display all employee information descending by last name using interface Comparable
f. Duplicate a faculty object using clone. Verify the duplication.

Test Data

Staff

    Last name:  Allen
    First name: Paita
    ID: 123
    Sex: M
    Birth date: 2/23/59
    Hourly rate: $50.00
    Last name: Zapata
    First Name: Steven
    ID: 456
    Sex: F
    Birth date: 7/12/64
    Hourly rate: $35.00
    Last name:Rios
    First name:Enrique
    ID: 789
    Sex: M
    Birth date: 6/2/70
    Hourly rate: $40.00

Faculty

    Last name: Johnson
    First name: Anne
    ID: 243
    Sex: F
    Birth date: 4/27/62
    Level: Full
    Degree: Ph.D
    Major: Engineering
    Reseach: 3
    Last name: Bouris
    First name: William
    ID: 791
    Sex: F
    Birth date: 3/14/75
    Level: Associate
    Degree: Ph.D
    Major: English
    Reseach: 1
    Last name: Andrade
    First name: Christopher
    ID: 623
    Sex: F
    Birth date: 5/22/80
    Level: Assistant
    Degree: MS
    Major: Physical Education
    Research: 0

Part-time

    Last name: Guzman
    First name: Augusto
    ID: 455
    Sex: F
    Birth date: 8/10/77
    Hourly rate: $35.00
    Hours worked per week: 30
    Last name: Depirro
    First name: Martin
    ID: 678
    Sex: F
    Birth date: 9/15/87
    Hourly rate: $30.00
    Hours worked per week:15
    Last name: Aldaco
    First name: Marque
    ID: 945
    Sex: M
    Birth date: 11/24/88
    Hourly rate: $20.00
    Hours worked per week: 35
