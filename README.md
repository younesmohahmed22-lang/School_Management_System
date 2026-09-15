# School Management System

## Project Description

The **School Management System** is a Python project built using **Object-Oriented Programming (OOP)** concepts.

The project simulates a simple school system where you can manage:

* Students
* Teachers
* Courses
* Student enrollment in courses
* Student grades
* Grade status (Passed or Failed)
* School statistics

The project demonstrates several important Python OOP concepts, including:

* Classes and Objects
* Inheritance
* Encapsulation
* Polymorphism
* Class Variables
* Class Methods
* Properties
* Getters and Setters
* Private Attributes
* Magic Methods such as `__str__` and `__len__`

---

## Features

### Person Class

The base class for people in the school system.

Each person has:

* Name
* Email
* Introduction method

### Student Class

The `Student` class inherits from the `Person` class.

Each student has:

* Name
* Email
* Private grade attribute
* List of enrolled courses

The class also supports:

* Grade validation using Getter and Setter
* Adding courses
* Displaying student information
* Counting the total number of students

### Teacher Class

The `Teacher` class inherits from the `Person` class.

Each teacher has:

* Name
* Email
* Subject
* List of assigned courses

### Course Class

The `Course` class manages courses in the school.

Each course has:

* Course name
* Assigned teacher
* List of enrolled students

The class supports:

* Adding students to a course
* Preventing duplicate enrollment
* Automatically adding the course to the student's course list
* Automatically assigning the course to the teacher
* Displaying all students in the course
* Counting the number of enrolled students

### Grade Status

The project checks whether a student has passed or failed.

* Grade `50` or higher → Passed
* Grade below `50` → Failed

### School Statistics

The system displays:

* Total number of students
* Total number of courses

---

# Requirements

To run this project, you need:

* Python 3.x

No external libraries are required.

The project uses only built-in Python features.

---

# How to Run

### 1. Download or Clone the Project

Download the project files to your computer.

### 2. Open the Project Folder

Open the project folder using **Visual Studio Code** or any Python code editor.

### 3. Make Sure Python Is Installed

Check that Python is installed by running:

```bash
python --version
```

or:

```bash
py --version
```

### 4. Run the Program

Open the terminal inside the project folder and run:

```bash
python school_management.py
```

If your file has a different name, replace `school_management.py` with your Python file name.

For example:

```bash
python main.py
```

You can also run the program directly using the Run button in Visual Studio Code.

---

# Example Output

The program will display information about:

* Students
* Teachers
* Courses
* Students enrolled in each course
* Introductions using Polymorphism
* Grade status
* School statistics
* Grade validation
* Number of students in each course

---

# Technologies Used

* Python
* Object-Oriented Programming (OOP)

---

# OOP Concepts Used

## Inheritance

`Student` and `Teacher` inherit from the `Person` class.

```python
class Student(Person):
```

```python
class Teacher(Person):
```

## Encapsulation

The student's grade is stored as a private attribute:

```python
self.__grade = grade
```

The project uses Getter and Setter methods through `@property`.

## Polymorphism

The `introduce()` method behaves differently for students and teachers.

```python
for person in people:
    person.introduce()
```

## Class Methods

The project uses a class method to get the total number of students.

```python
Student.get_total_students()
```

## Magic Methods

The project uses:

* `__str__()` to display objects as readable text.
* `__len__()` to return the number of students in a course.

---



Younes Mohammed
