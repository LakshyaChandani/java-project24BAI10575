# CAPSTONE PROJECT REPORT

**Project Title:** Campus Course & Records Manager (CCRM)  
**Student Name:** Lakshya Chandani  
**Registration Number:** 24BAI10575  
**Course:** Programming in Java  

---

## 1. Introduction and Problem Statement

### 1.1 Problem Statement
To run their daily operations such as recording student information or tracking their enrollments and courses offered, educational institutions must have secure, reliable, and effective means of managing these records. If the institution does not use an electronic system for storing these records, many issues arise like duplicated data entry, risks associated with the security of records, potential for human errors in students’ grades and lack of administrative efficiency among others.

### 1.2 Objective
This project, called Campus Course and Records Manager, is to assist with a real-life issue and is a complete, console-based university management solution. It securely manages all of the core entities of a university using advanced object-oriented Java, and it provides functionality to manage students, instructors, classes, grades, and automatic backups.

---

## 2. Key Features

The CCRM application offers several distinct administrative features:

*   **User/Student Management:** Administrators can create, assign, list, update, and deactivate student or instructor profiles.
*   **Course Management:** Capability to dynamically create, update, and deactivate courses, alongside mapping instructors to teach specific course modules.
*   **Enrollment & Academic Tracking:** A sophisticated enrollment system that regulates student credit limits, registers them for classes, handles course grading, and computes their final GPA.
*   **File I/O & State Persistence:** The system imports and exports data securely to `.csv` and `.dat` formats. This avoids the use of typical Relational Databases (like MySQL) to demonstrate mastery of the Java NIO.2 File API.
*   **Disaster Recovery (Backup System):** The system integrates a timestamp-driven recursive directory backup protocol to protect the institution's sensitive files against accidental corruption.

---

## 3. Technical Architecture and Java Concepts

The project was rigorously developed to meet the constraints of a final Java capstone. The following core and advanced Java methodologies were utilized in the source code architecture:

### 3.1 Object-Oriented Principles (OOP)
*   **Encapsulation:** Implemented globally through private class fields with controlled access via public getter/setter methodologies (e.g., `model/Person.java`).
*   **Inheritance:** The base abstract class `Person` elegantly branches into `Student` and `Instructor` subclasses, minimizing code duplication.
*   **Abstraction:** The `Person.java` parent class sets up explicit contracts via abstract methods like `getRole()`, forcing implementations downstream.
*   **Polymorphism:** Utilizing `Person` references dynamically at runtime to accept and manipulate both `Student` and `Instructor` objects fluidly.

### 3.2 Advanced Java Features & Modern APIs
*   **Design Patterns:** 
    *   *Singleton:* Applied to the `DataStore.java` to prevent memory leaks and ensure that the administrative data state remains identical across all system threads.
    *   *Builder:* Applied to `CourseBuilder` and `TranscriptBuilder` to construct heavily detailed, complex objects step-by-step.
*   **Custom Exceptions:** Developed business-specific errors (e.g., `MaxCreditLimitExceededException`) to throw highly semantic, descriptive stack traces representing real administrative logic failures.
*   **Java NIO.2 (Non-blocking I/O):** For modern, fast file operations like parsing existing student databases and writing directory backups.
*   **Collections Framework & Java Streams:** The application pipelines bulk academic data through Java 8+ Streams for complex filtering operations without iterating manually. 
*   **Recursion:** Utilized practically within `BackupUtils.java` to dynamically traverse and clone complex parent-child folder structures for the backup generator.

---

## 4. Software Requirements
*   **Runtime Environment:** Java Development Kit (JDK) 8 or higher (Tested up to JDK 21).
*   **Storage Access:** Minimum 10 MB logical disk space for running configurations and recursive backups.
*   **Execution Mechanism:** Native OS terminal/console.

---

## 5. Future Enhancements

While CCRM is functionally complete, future updates could implement:
1.  **Graphical User Interface (GUI):** Replacing the console CLI with JavaFX to give university clerks a more visual interface.
2.  **Multithreading:** Designing concurrent background threads for the auto-backup sequences so they do not block the main application thread during I/O delays.
3.  **Relational Database Integration:** Transitioning from NIO.2 file storage systems to a robust SQL database (JDBC/PostgreSQL) for large-scale production scalability.

---

## 6. Conclusion
The **Campus Course & Records Manager** thoroughly demonstrates how raw syntactic mechanics of the Java programming language (Collections, Streams, NIO.2, OOP) map perfectly to tangible solutions for real-world enterprise logic constraints. It meets and exceeds all requirements outlined for the BYOP Capstone submission.
