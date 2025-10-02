# Student Management System  

## Problem Statement  
Design and implement a **Student Management System** using **Inheritance, Polymorphism, Abstract Classes, Interfaces, and CRUD Operations**.  

The system should include:  
- An **abstract class `Person`** with fields `name` and `email`.  
- A **`Student` class** extending `Person` with fields `rollNo`, `course`, `marks`, and `grade`.  
- An **interface `RecordActions`** with methods for adding, deleting, updating, searching, and viewing student records.  
- A **`StudentManager` class** to manage records using an **ArrayList** and prevent duplicate roll numbers.  
- Demonstration of **Method Overriding, Method Overloading, and Abstract Methods**.  

---

## Attributes  
1. `String name`  
2. `String email`  
3. `String course`  
4. `int rollNo`  
5. `double marks`  

---


---

##  Code Description  

### **Package: `model`**  

#### `Person.java`  
- Abstract class `Person`  
- Attributes: `name`, `email`  
- Parameterized constructor  
- Abstract method `displayInfo()`  

#### `Student.java`  
- Extends `Person`  
- Attributes: `rollNo`, `course`, `marks`, `grade`  
- Parameterized constructor  
- `calcGrade()` → calculates grade based on marks  
- `displayInfo()` → overridden method (method overriding)  
- `displayInfo(String msg)` → overloaded method (method overloading)  

---

### **Package: `service`**  

#### `RecordActions.java`  
- Interface with CRUD methods:  
  - `addStudent()`  
  - `deleteStudent()`  
  - `updateStudent()`  
  - `searchStudent()`  
  - `viewAllStudents()`  

#### `StudentManager.java`  
- Implements `RecordActions`  
- Uses **ArrayList\<Student\>** to store records  
- Methods:  
  - `addStudent()` → validates duplicate roll numbers and adds student  
  - `deleteStudent()` → deletes student by roll number  
  - `updateStudent()` → updates details of a student  
  - `searchStudent()` → searches student by roll number  
  - `viewAllStudents()` → displays all students  

---

### **Main Class: `StudentManagementSystem.java`**  
- Imports `service` package  
- Creates an object of `StudentManager`  
- Menu-driven program with user choices  

---

## Concepts Implemented  
- **Abstract Methods**  
- **Method Overriding**  
- **Method Overloading**  
- **Inheritance**  
- **Interfaces**  
- **Packages**  
- **CRUD Operations**  
- **OOP Principles (Abstraction, Encapsulation, Polymorphism)**  

---

## How to Run  

