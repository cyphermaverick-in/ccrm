# Campus Course & Records Manager (CCRM)

## Project Overview

This is a console-based Java application designed to manage student and course records for a campus. It includes features for student and course management, enrollment, grading, and file operations. The project is built with Java SE and demonstrates key programming concepts such as Object-Oriented Programming (OOP) principles, modern I/O with NIO.2, Streams, and design patterns.

## How to Run

1.  **Prerequisites**: Ensure you have the Java Development Kit (JDK) installed. This project was developed and tested with JDK 11.
2.  **Clone the Repository**:
    ```bash
    git clone https://github.com/cyphermaverick-in/ccrm.git
    cd CCRM
    ```
3.  **Run from IDE**:
    * Open the project in Eclipse.
    * Right-click the `Main.java` file in the `edu.ccrm.cli` package.
    * Select `Run As -> Java Application`.
4.  **Enabling Assertions**:
    Assertions are used to ensure non-null IDs and credit bounds. To enable them, add `-ea` to your JVM arguments in your IDE's run configuration.

## Java Platform Differentiations

### Evolution of Java

* **1995**: Java is released by Sun Microsystems.
* **1996**: First public release of JDK 1.0.
* **2004**: J2SE 5.0 (renamed to Java SE 5) introduces generics, enums, autoboxing, and annotations.
* **2014**: Java 8 introduces lambda expressions and the new Date/Time API.
* **2017-present**: Java moves to a six-month release cycle, with new versions (e.g., Java 11, 17, 21) bringing new features and performance improvements.

### Java SE vs. Java ME vs. Java EE

| Feature          | Java SE (Standard Edition)                            | Java ME (Micro Edition)                          | Java EE (Enterprise Edition)                             |
| ---------------- | ----------------------------------------------------- | ------------------------------------------------ | -------------------------------------------------------- |
| **Purpose** | Desktop, console, and general-purpose applications.   | Embedded systems and mobile devices.             | Large-scale, distributed, multi-tiered applications.     |
| **Scope** | Core Java libraries.                                  | Subset of SE APIs with device-specific libraries. | SE APIs plus enterprise features (servlets, EJBs, etc.). |
| **Target Device** | PCs, servers.                                         | Mobile phones, IoT devices, set-top boxes.       | Web servers, application servers.                        |

### JDK, JRE, and JVM

* **JDK (Java Development Kit)**: This is a software development environment used for developing Java applications. [cite_start]It includes the JRE, a compiler (`javac`), and other tools like a debugger and archiver[cite: 44].
* **JRE (Java Runtime Environment)**: This contains the core class libraries and the JVM. It is the minimum required to run a Java application. [cite_start]It does not include development tools[cite: 44].
* **JVM (Java Virtual Machine)**: This is an abstract machine that provides a runtime environment for executing Java bytecode. [cite_start]It is the component that makes Java "write once, run anywhere"[cite: 44].

## Syllabus Topic to Code Mapping

| Syllabus Topic                               | File/Class/Method Where it is Demonstrated                      |
| -------------------------------------------- | --------------------------------------------------------------- |
| OOP: Inheritance                             | `Person` (abstract class), `Student`, `Instructor`              |
| OOP: Polymorphism                            | `TranscriptService.printTranscript()` method                    |
| Enums with constructors & fields             | `Grade.java`, `Semester.java`                                   |
| Functional Interfaces & Lambdas              | `CourseService.findCoursesBy()` method                          |
| Singleton Design Pattern                     | `AppConfig.java`                                                |
| Builder Design Pattern                       | `Course.Builder` inner class in `Course.java`                   |
| Exceptions (Custom)                          | `MaxCreditLimitExceededException` in `EnrollmentService.java`   |
| NIO.2 & Streams                              | `ImportExportService.java`, `BackupService.java`                |
| Recursion                                    | `BackupService.computeDirectorySize()` method                 |
| `toString()` override                        | `Student.java`, `Course.java`                                   |