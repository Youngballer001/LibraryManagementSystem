# School Library Management System

A digital School Library Management System designed to help manage books, students, borrowing records, and library fines.

## Project Overview

The system is developed using multiple technologies:

* **Frontend:** HTML, CSS, and JavaScript
* **Main Backend:** Java and Spring Boot
* **Database:** MySQL
* **Fines API:** Python and Flask

## Project Structure

```text
LibraryManagementSystem/
│
├── Backend/
│   └── src/main/java/com/schoollibrary/
│       └── Main.java
│
├── Fines_api/
│   ├── app.py
│   └── requirements.txt
│
├── Frontend/
│   ├── index.html
│   ├── style.css
│   └── style.js
│
├── images/
│
├── library-backend/
│   └── library-backend/
│       ├── src/
│       ├── pom.xml
│       └── mvnw.cmd
│
├── .gitignore
└── README.md
```

## Technologies Used

* HTML5
* CSS3
* JavaScript
* Java
* Spring Boot
* Python
* Flask
* MySQL
* Maven
* Git and GitHub

## Running the Project

### 1. Main Java Spring Boot Backend

Make sure MySQL is running and the `school_library` database exists.

Open a terminal and navigate to the Spring Boot project:

```bash
cd library-backend/library-backend
```

Configure the database environment variables in your terminal.

For Windows Command Prompt:

```cmd
set DB_URL=jdbc:mysql://localhost:3307/school_library
set DB_USERNAME=root
set DB_PASSWORD=your_database_password
```

Start the backend:

```cmd
mvnw.cmd spring-boot:run
```

The Spring Boot backend runs on:

```text
http://localhost:8080
```

### 2. Python Fines API

Navigate to the project root and create a virtual environment:

```bash
python -m venv venv
```

Activate it in Git Bash:

```bash
source venv/Scripts/activate
```

Install the dependencies:

```bash
pip install -r Fines_api/requirements.txt
```

Start the API:

```bash
python Fines_api/app.py
```

The fines API runs on:

```text
http://127.0.0.1:5000
```

Available endpoints:

| Method | Endpoint          | Purpose                           |
| ------ | ----------------- | --------------------------------- |
| GET    | `/health`         | Checks whether the API is running |
| POST   | `/calculate-fine` | Calculates overdue book fines     |

The fine rate is KES 10 per overdue day.

### 3. Frontend

Open `Frontend/index.html` using a local development server.

The frontend communicates with the Spring Boot backend.

### 4. Separate Java Console Program

The `Backend` directory also contains a simple Java console program.

From the project root, compile it:

```bash
javac -d out Backend/src/main/java/com/schoollibrary/Main.java
```

Run it:

```bash
java -cp out com.schoollibrary.Main
```

## Configuration and Security

* Database credentials should be supplied through environment variables.
* Do not commit passwords, API keys, or other sensitive credentials.
* Environment files such as `.env` should remain excluded from Git.
* Use secure authentication and authorization when deploying the application.

## Project Status

The School Library Management System is under development. Features and components may change as development continues.
