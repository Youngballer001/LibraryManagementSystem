\# 📚 School Library Management System



A software application designed to simplify and improve library operations through digital management of books, students, borrowings, and fines.



\## 🚀 Project Overview



The School Library Management System aims to provide an organized way of managing library activities. It brings together a user-friendly frontend, a Java Spring Boot backend, a MySQL database, and a Python-based fines API.



The system is intended to reduce manual record-keeping, improve accessibility of library information, and make everyday library operations more efficient.



\## ✨ Main Components



\* \*\*Frontend:\*\* User interface built with HTML, CSS, and JavaScript.

\* \*\*Backend:\*\* Java application built using Spring Boot.

\* \*\*Database:\*\* MySQL for storing application data.

\* \*\*Fines API:\*\* Python application for fines-related functionality.



\## 🛠️ Technologies Used



| Technology  | Purpose                |

| ----------- | ---------------------- |

| HTML5       | Web page structure     |

| CSS3        | Styling and layout     |

| JavaScript  | Frontend functionality |

| Java        | Backend development    |

| Spring Boot | Backend framework      |

| MySQL       | Database management    |

| Python      | Fines API              |

| Git         | Version control        |

| GitHub      | Source code hosting    |



\## 📁 Project Structure



```text

LibraryManagementSystem/

│

├── Backend/

│   └── src/

│       └── main/

│           └── java/

│               └── com/

│                   └── schoollibrary/

│                       └── Main.java

│

├── Frontend/

│   ├── index.html

│   ├── style.css

│   └── style.js

│

├── Fines\_api/

│   ├── app.py

│   └── requirements.txt

│

├── images/

│   └── Project image assets

│

├── library-backend/

│   └── library-backend/

│       ├── mvnw

│       ├── mvnw.cmd

│       ├── pom.xml

│       └── src/

│           ├── main/

│           │   ├── java/

│           │   │   └── com/schoollibrary/

│           │   └── resources/

│           │       └── application.properties

│           └── test/

│

├── .gitignore

└── README.md

```



\## ⚙️ Requirements



Before running the application, ensure you have the following installed:



\* Java Development Kit (JDK)

\* MySQL Server

\* Python

\* A modern web browser

\* Git



You will also need the database configured for the backend.



\## 🗄️ Database Configuration



The Spring Boot backend uses the following database configuration:



```properties

spring.datasource.url=${DB\_URL:jdbc:mysql://localhost:3307/school\_library}

spring.datasource.username=${DB\_USERNAME:root}

spring.datasource.password=${DB\_PASSWORD}

```



Configure the appropriate environment variables on your computer:



\* `DB\_URL`

\* `DB\_USERNAME`

\* `DB\_PASSWORD`



\*\*Important:\*\* Never commit actual database passwords, API keys, or other private credentials to GitHub.



\## ▶️ Running the Application



\### 1. Clone the repository



```bash

git clone https://github.com/Youngballer001/LibraryManagementSystem.git

```



\### 2. Open the project



```bash

cd LibraryManagementSystem

```



\### 3. Start the MySQL database



Ensure your MySQL server is running and that the `school\_library` database is configured.



\### 4. Start the Spring Boot backend



Navigate to the backend application:



```bash

cd library-backend/library-backend

```



Run:



\*\*Windows:\*\*



```cmd

mvnw.cmd spring-boot:run

```



\*\*Linux/macOS:\*\*



```bash

./mvnw spring-boot:run

```



The backend is configured to use port `8080`.



\### 5. Open the frontend



Navigate to the `Frontend` directory and open `index.html` using a local development server.



\### 6. Run the Fines API



The Python application is located in `Fines\_api/`. Install its dependencies using:



```bash

pip install -r requirements.txt

```



Run the application using the appropriate command for its framework.



\## 🔐 Security



The backend includes authentication functionality and password encryption using BCrypt.



Database credentials should be supplied through environment variables rather than hardcoded into application files.



\## 👨‍💻 Development



This project is developed using a modular structure, separating frontend functionality, backend operations, database configuration, and fines-related services.



\## 📌 Project Status



Under development. Features and functionality may change as development continues.



\## 📄 License



No license has currently been specified for this project.



