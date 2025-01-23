# **Task Management App**
A simple and powerful backend application for managing daily tasks. Built with **Java Spring Boot** and **PostgreSQL**, this application is designed to help users stay organized by creating, managing, and tracking their tasks effectively. The project is backend-focused, but it is ready to integrate with a React frontend if needed.

---

## **Features**
- **Task Management**
    - Create, read, update, and delete tasks.
    - Assign priorities: High, Medium, Low.
    - Set task statuses: To-Do, In Progress, Done.
    - Add due dates to tasks.

- **User Authentication**
    - Secure user login and registration using **JWT (JSON Web Token)**.
    - Each user can only access their own tasks.

- **Search and Filter**
    - Search tasks by title or description.
    - Filter tasks by priority, status, or due date.

---

## **Technologies Used**
- **Backend**: Java Spring Boot
- **Database**: PostgreSQL
- **Authentication**: Spring Security with JWT
- **Build Tool**: Maven
- **Testing**: JUnit 5

---

## **Getting Started**

### **1. Prerequisites**
- Java 17+
- PostgreSQL
- Maven

### **2. Clone the Repository**
```bash
git clone https://github.com/onuda22/task-management.git
cd task-management
```

### **3. Configure the Database**
Update the `src/main/resources/application.properties` file with your PostgreSQL credentials:
```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/task_manager_db
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
```

### **4. Run the Application**
Build and run the project using Maven:
```bash
mvn spring-boot:run
```

The application will be accessible at `http://localhost:8080`.

---

## **API Endpoints**
### **Authentication**
- `POST /api/auth/register`: Register a new user.
- `POST /api/auth/login`: Login and obtain a JWT token.

### **Tasks**
- `GET /api/tasks`: Get all tasks for the logged-in user.
- `POST /api/tasks`: Create a new task.
- `PUT /api/tasks/{id}`: Update an existing task.
- `DELETE /api/tasks/{id}`: Delete a task by ID.

---

## **Future Improvements**
- Add support for task categories.
- Implement reminders for due tasks via email.
- Integrate with a React frontend for a full-stack experience.

---

## **Contributing**
Contributions are welcome! Feel free to fork this repository, make changes, and submit a pull request.

---