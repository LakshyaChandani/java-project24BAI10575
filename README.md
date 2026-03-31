# Campus Course & Records Manager (CCRM)

**Name:** Lakshya Chandani  
**Reg No:** 24BAI10575

This is a comprehensive console-based Java application designed to manage the core data and processes of a higher education institution. It's built to handle everything from student and course information to managing enrollments and grades, all while keeping your data safe with robust file operations.

# Project Overview

The Campus Course & Records Manager (CCRM) is a hands-on project that puts fundamental and advanced Java programming concepts into a single, functional application. It's a great example of object-oriented programming, modern Java APIs, and file handling in action.

Key Features:

* Student Management: You can create, list, update, and even deactivate student records.  
* Course Management: Easily create, update, and deactivate courses, and assign instructors to them.  
* Enrollment & Grading: Manage student enrollments, making sure they don't exceed credit limits, and handle grading and GPA calculations.  
* File Operations: Import and export data in CSV format using modern NIO.2 file operations.  
* Backup System: Create timestamped backups with recursive directory operations to protect your data.  
* System Reports: Generate comprehensive statistics and reports to get a clear overview of the system.

# The Evolution of Java

Java has a rich history of evolution, constantly improving to meet the needs of modern development. Here's a brief timeline:

* 1995: Java 1.0 \- The original release that introduced the "Write Once, Run Anywhere" (WORA) philosophy.  
* 1997: Java 1.1 \- Added new features like inner classes and JDBC (Java Database Connectivity).  
* 1998: Java 2 (J2SE, J2EE, J2ME) \- A major update that established the three main platforms: Standard Edition, Enterprise Edition, and Micro Edition.  
* 2004: Java 5 (J2SE 5.0) \- A huge release that brought us generics, enums, and the enhanced for-loop, among other things.  
* 2014: Java 8 \- A game-changer with the introduction of lambda expressions and the Streams API, making functional programming in Java a reality.  
* 2017: Java 9 \- Introduced the Java Platform Module System (JPMS), which modularized the JDK.  
* 2018: Java 11 \- The first long-term support (LTS) release under the new release cadence, which removed some of the older Java EE modules.  
* 2023: Java 21 \- The latest LTS release, featuring modern concurrency with virtual threads and enhanced pattern matching.

# Java Platform Comparison

Here’s a simple breakdown of the different Java platforms:

* Java SE (Standard Edition): This is for building standard desktop, server, and embedded applications. It includes the core Java APIs, which is what this project uses.  
* Java EE (Enterprise Edition): This platform is for large-scale, multi-tiered enterprise applications. It provides APIs for things like servlets, JSPs, and web services.  
* Java ME (Micro Edition): This version is specifically for mobile and embedded devices with limited resources.

# Java Architecture: JDK, JRE, and JVM

The Java platform is built on three key components that work together seamlessly.

* JDK (Java Development Kit): Think of this as the complete toolbox for a Java developer. It includes the compiler ('javac'), a debugger, and all the other tools you need to write and build a Java program.  
* JRE (Java Runtime Environment): This is what you need to run a Java program. It includes the JVM and the necessary class libraries. You can't develop with it, but you can definitely run applications.  
* JVM (Java Virtual Machine): This is the magic behind Java's "Write Once, Run Anywhere" philosophy. The JVM takes the platform-independent bytecode from your compiled code and translates it into code that your computer can understand and execute. 

# Getting Started

#### Prerequisites

* Java 8 or higher  
* Any Java IDE (like Eclipse, IntelliJ IDEA, or VS Code)  
* Command-line access

# Enabling Assertions

To enable assertions, you just need to use the '-ea' flag when you run the Java application from the command line. This is super helpful for debugging and for internal consistency checks.

Sample Command:

'java \-ea com.ccrm.CampusCourseRecordsManager'  
