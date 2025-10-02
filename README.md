# Student Management System  

## Problem Statement  
Design and implement a Student Management System using inheritance, 
polymorphism, and interfaces. The system should consist of an abstract class 
Person with common fields such as name and email, and a concrete class Student 
that extends Person with additional fields like rollNo, course, marks, and grade. 
Implement an interface RecordActions with methods to add, delete, update, 
and view student records. Use a StudentManager class to handle the operations 
on student records, ensuring that duplicate roll numbers are prevented. The 
system should demonstrate method overriding, method overloading, and 
the use of abstract methods. 
 

The system includes:  
- An abstract class Person with fields name and email.  
- A Student class extending Person with fields rollNo, course, marks, and grade.  
- An interface RecordActions with methods for adding, deleting, updating, searching, and viewing student records.  
- A StudentManager class to manage records using an ArrayList and prevent duplicate roll numbers.  
- Demonstration of Method Overriding, Method Overloading, and Abstract Methods.  

---

## Attributes  
1. String name
2. String email  
3. String course  
4. int rollNo  
5. double marks  

---
##  Code Description  

### **Package: model**  

#### Person.java  
- Abstract class Person  
- Attributes: name, email  
- Parameterized constructor  
- Abstract method displayInfo()  

#### Student.java 
- Extends Person
- Attributes: rollNo, course, marks, grade  
- Parameterized constructor  
- calcGrade() → calculates grade based on marks  
- displayInfo() → method overriding
- displayInfo(String msg) → method overloading

---

### Package: service 

#### RecordActions.java
- Interface with CRUD methods:  
  - addStudent()
  - deleteStudent()  
  - updateStudent()  
  - searchStudent()  
  - viewAllStudents()  

#### StudentManager.java
- Implements RecordActions  
- Uses ArrayList<Student> to store records  
- Methods:  
  - addStudent() → validates duplicate roll numbers and adds student  
  - deleteStudent() → deletes student by roll number  
  - updateStudent() → updates details of a student  
  - searchStudent() → searches student by roll number  
  - viewAllStudents() → displays all students  

---

### Main Class: StudentManagementSystem.java
- Imports service package  
- Creates an object of StudentManager
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
- **OOP Principles**  

---

## Sample ScreenShot
<img width="1366" height="768" alt="Screenshot (38)" src="https://github.com/user-attachments/assets/3fcfce60-2dd4-4cff-bd39-b778ed070e2d" />
<img width="1366" height="768" alt="Screenshot (39)" src="https://github.com/user-attachments/assets/88b2bb4f-1754-407e-9501-25b3522746e5" />
<img width="1366" height="768" alt="Screenshot (40)" src="https://github.com/user-attachments/assets/81d92b75-0301-4eb6-a113-13ed68afdad0" />





## How to run the StudentManagementSystemMain

- Step 1 : Click on Code in blue color.
- Step 2 : Click on the Codespace.
- Step 3 : Click on the '+' sign.
- Step 4 : After opening the VSCode like setup.
- Step 5 : Open terminal 
- Step 6 : Type ' javac StudentManagementSystemMain.java '
- Step 7 : Type ' java StudentManagementSystemMain ' 
- OR Clicking on any existing CodeSpace.

## Java StudentManagemntSystemMain File -> https://github.com/SidharthBScCS/Student-Management-System-2/blob/main/StudentManagementSystemMain.java
