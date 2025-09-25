Campus Course & Records Manager (CCRM)
Project Overview

The Campus Course & Records Manager (CCRM) is a console-based Java SE application for educational institutions to manage:

Students → Create, update, list, deactivate, enroll/unenroll in courses.

Courses → Create, update, list, deactivate, search/filter, assign instructors.

Enrollments & Grading → Enroll students in courses, record marks, calculate GPA, generate transcripts.

File Operations → Import/export data to CSV/text files and perform timestamped backups.

Reports → Generate GPA distribution, top performers, etc., using Streams API.

This project demonstrates:

Core Java concepts: OOP, Enums, Interfaces, Nested Classes, Streams API, Date/Time API, Exception Handling.

Design Patterns: Singleton, Builder.

Modern Java Features: NIO.2, Lambdas, and recursion.

Project Structure
CampusCourseRecordsManager
│   README.md
│
├───bin/                # Compiled output files
│   ├───edu/ccrm/...    # .class files for all packages
│   ├───exports/        # Exported CSV files
│   └───backups/        # Backup folders
│
├───lib/                # External libraries (if needed)
│
└───src/                # Source code
    │   App.java
    │
    ├───edu/ccrm/
    │   ├───cli/        # CLIManager, Main.java
    │   ├───config/     # AppConfig (Singleton)
    │   ├───domain/     # Person, Student, Course, Enrollment, etc.
    │   ├───exceptions/ # Custom exceptions
    │   ├───io/         # Import/Export and backup services
    │   ├───service/    # StudentService, CourseService, EnrollmentService
    │   └───util/       # Validators, Recursion utilities
    │
    ├───exports/        # CSV export folder
    └───imports/        # CSV import folder

How to Run
Requirements

Java JDK 24 or above
Check installation:
java -version
javac -version
VS Code with Java Extension Pack installed.

Git for version control.
Compile the Project

Open VS Code terminal, navigate to project root:
cd "C:\Gaurav\Study\Coding\Coding Material\JAVA_PROJECT_VITYYARTHI\CampusCourseRecordsManager"
Compile source files into the bin folder:
javac -d bin -sourcepath src src\edu\ccrm\cli\Main.java src\edu\ccrm\**\*.java

Run the Project
java -cp bin edu.ccrm.cli.Main

