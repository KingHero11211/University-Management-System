# University Management System 🎓

A comprehensive desktop application built in Java Swing to manage student, teacher, and administrative data for a university. This system provides a user-friendly interface for handling day-to-day university operations efficiently.

## 📸 Screenshots

*(Pro Tip: Replace these placeholder links with screenshots of your actual application!)*

| Login Screen | Main Dashboard | Student Details |
| :--- with screenshots of your actual application!)*

| Login Screen | Main Dashboard | Student Details |
| :---: | :---: | :---: |
| ![Login Screen](link-to-your-login-screenshot.png) | ![Main Dashboard](link-to-your-dashboard-screenshot.png) | ![Student Details](link-to-your-student-details-screenshot.png) |

---

## ✨ Features

This system is packed with features to facilitate university administration:

- **👤 User Authentication**: Secure login for administrators.
- **👨‍🎓 Student Management**:
    - Add new students with detailed information (name, address, course, etc.).
    - View a complete list of all students.
    - Update existing student records.
- **👨‍🏫 Teacher Management**:
    - Add new teachers with their details.
    - View a list of all faculty members.
    - Update existing teacher records.
- **📝 Attendance Tracking**:
    - Mark student and teacher attendance.
    - View attendance records.
- **💯 Examination & Marks**:
    - Enter student examination marks for various subjects.
    - View and generate student mark sheets.
- **💵 Fee Management**:
    - View the complete fee structure for different courses.
    - Process and record student fee payments.
- **🌴 Leave Management**:
    - Manage and approve leave requests from both students and teachers.
    - View details of all approved leaves.

---

## 🛠️ Tech Stack & Libraries

- **Language**: **Java**
- **UI Framework**: **Java Swing**
- **Database**: **MySQL**
- **Libraries**:
    - **MySQL Connector/J**: To connect the Java application with the MySQL database.
    - **JCalendar**: For a user-friendly date picker component.
    - **rs2xml.jar**: To help display database query results in a `JTable`.

---

## 🚀 Getting Started

Follow these instructions to set up and run the project on your local machine.

### Prerequisites

You will need the following software installed on your system:
- **Java Development Kit (JDK)** 11 or higher.
- **MySQL Server**
- **Apache NetBeans IDE** (or any other Java IDE like Eclipse or IntelliJ IDEA).

### 1. Database Setup

1.  Start your MySQL server.
2.  Create a new database for the project:
    ```sql
    CREATE DATABASE universitymanagementsystem;
    ```
3.  **Create the required tables.** As the database schema is not provided in a `.sql` file, you will need to create the tables manually. To do this, you must examine the SQL queries within the `.java` source files to determine the table names, column names, and data types.

    **Key files to inspect:**
    - `AddStudent.java` (for the `student` table)
    - `AddTeacher.java` (for the `teacher` table)
    - `EnterMarks.java` (for `marks` and `subject` tables)
    - `MarkAttendance.java` (for the `attendance` table)
    - `StudentFeeForm.java` (for the `fee` table)
    - And other similar files.

### 2. Project Setup

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/KingHero11211/Your-Repository-Name.git
    ```
    *(Replace `Your-Repository-Name` with the actual name of your repository)*

2.  **Open the project** in your preferred Java IDE (e.g., NetBeans).
3.  **Add Libraries**: Manually add `mysql-connector-j.jar`, `jcalendar.jar`, and `rs2xml.jar` to the project's library path. You will the MySQL database.
    - **JCalendar**: For a user-friendly date picker component.
    - **rs2xml.jar**: To help display database query results in a `JTable`.

---

## 🚀 Getting Started

Follow these instructions to set up and run the project on your local machine.

### Prerequisites

You will need the following software installed on your system:
- **Java Development Kit (JDK)** 11 or higher.
- **MySQL Server**
- **Apache NetBeans IDE** (or any other Java IDE like Eclipse or IntelliJ IDEA).

### 1. Database Setup

1.  Start your MySQL server.
2.  Create a new database for the project. You can use the following SQL command:
    ```sql
    CREATE DATABASE universitymanagementsystem;
    ```
3.  **Create the required tables.** The Java application expects specific tables and columns to be present.
    > **Note:** A full SQL schema script to create all tables automatically will be added to this repository soon. Until then, the tables must be created manually based on the SQL queries found within the `.java` source files.

### 2. Project Setup

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/KingHero11211/Your-Repository-Name.git
    ```
    *(Replace `Your-Repository-Name` with the actual name of your repository)*

2.  **Open the project** in your preferred Java IDE (e.g., NetBeans).
3.  **Add Libraries**: Manually add `mysql-connector-j.jar`, `jcalendar.jar`, and `rs2xml.jar` to the project's library path. You will need to download these JAR files separately.
4.  **Configure the database connection:**
    - Open the `Conn.java` file located inside the `src` folder.
    - Modify the database connection string, username, and password to match your MySQL setup.
    ```java
    // Inside Conn.java
    c = DriverManager.getConnection("jdbc:mysql:///universitymanagementsystem", "YOUR_USERNAME", "YOUR_PASSWORD");
    ```

### 3. Running the Application

1.  **Build the project** using your IDE's build command.
2.  **Run the main file**. The entry point for the application is `Splash.java`. Right-click on `Splash.java` and select "Run File".
3.  The splash screen will appear, followed by the login window. The default credentials are `admin` and `12345`.

---

## 📂 Project Structure

The repository contains the essential source code and configuration files for the project.
```
University-Management-System/
├── src/
│ ├── icons/
│ │ └── (All image and icon files)
│ └── university/management/system/
│ └── (All .java source files)
├── .gitignore
├── build.xml
├── manifest.mf
└── README.md
```
