# Credit Card Management System

A **full-stack web application** for managing customers and their associated credit cards. This system is built with **Angular** for the frontend and **Spring Boot** for the backend. The project provides a clean and functional user interface for performing CRUD operations on customers and credit cards.

---

## Features

### Customer Management
- Add, view, edit, and delete customers.
- View customer details, including their credit cards.

### Credit Card Management
- Add, view, edit, and delete credit cards for each customer.
- Manage credit limits, current balances, and other card details.

### Frontend
- Built using **Angular**.
- Dynamic forms for adding and editing customers and credit cards.
- Bootstrap-based responsive design.

### Backend
- Built with **Spring Boot**.
- RESTful API with endpoints for customer and credit card management.
- Integrated with a PostgreSQL database.

### Deployment
- Containerized using **Docker**.
- Uses **NGINX** to serve the frontend in production.
- Backend exposed via port 8080.

---

## Prerequisites
Ensure you have the following installed on your system:
- [Node.js](https://nodejs.org) (v18 or higher)
- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)
- [Java 17](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
- Maven (for local builds)

---

## Project Structure
```plaintext
credit-card-management-system/
├── backend/                # Spring Boot application
│   ├── src/                # Backend source code
│   ├── Dockerfile          # Backend Dockerfile
│   └── pom.xml             # Maven configuration
├── frontend/               # Angular application
│   ├── src/                # Frontend source code
│   ├── Dockerfile          # Frontend Dockerfile
│   └── package.json        # Frontend dependencies
├── docker-compose.yml      # Docker Compose configuration
└── README.md               # Documentation
```

---

## How to Run the Project
This project uses **Docker Compose** to run both the frontend and backend as containers.

### Steps to Run
1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd credit-card-management-system
   ```

2. **Build and Run the Containers**
   Run the following command to build and start the containers:
   ```bash
   docker-compose up --build
   ```

3. **Access the Application**
   - Frontend: Open [http://localhost](http://localhost) in your browser.
   - Backend API: Access [http://localhost:8080](http://localhost:8080).

4. **Stop the Containers**
   Press `Ctrl + C` in the terminal or run:
   ```bash
   docker-compose down
   ```

---

## API Endpoints
The backend exposes the following RESTful endpoints:

### Customers
| Method | Endpoint                 | Description                 |
|--------|--------------------------|-----------------------------|
| GET    | `/api/customers`         | Retrieve all customers      |
| GET    | `/api/customers/{id}`    | Retrieve a single customer  |
| POST   | `/api/customers`         | Add a new customer          |
| PUT    | `/api/customers/{id}`    | Update customer details     |
| DELETE | `/api/customers/{id}`    | Delete a customer           |

### Credit Cards
| Method | Endpoint                      | Description                       |
|--------|-------------------------------|-----------------------------------|
| GET    | `/api/credit-cards`           | Retrieve all credit cards         |
| POST   | `/api/credit-cards`           | Add a new credit card             |
| PUT    | `/api/credit-cards/{id}`      | Update credit card details        |
| DELETE | `/api/credit-cards/{id}`      | Delete a credit card              |

---

## Development Setup (Optional)
If you want to run the frontend and backend separately without Docker, refer to the respective repositories:

### Backend (Spring Boot)
- **Repository**: [Backend Repository](<https://github.com/StevenRBC/credit-card-api>)
- Instructions for running the backend are provided in its README file.

### Frontend (Angular)
- **Repository**: [Frontend Repository](<https://github.com/StevenRBC/credit-card-management>)
- Instructions for running the frontend are provided in its README file.

---

## Technologies Used
- **Frontend**: Angular, TypeScript, Bootstrap
- **Backend**: Spring Boot, Java 17, Maven
- **Database**: PostgreSQL
- **Containerization**: Docker, Docker Compose
- **Server**: NGINX
---

## Documentation and Diagrams

The detailed documentation for this project, including:

- **Entity-Relationship Diagram (ERD)**
- **Class Diagram**
- **Sequence Diagrams**

Can be accessed in the following link:

- **[Documentation and Diagrams](https://docs.google.com/document/d/1hgjb_67UU_B8hA21AQs_-L9li56wlIqPKkADegCrBss/edit?usp=sharing)**

Feel free to view or download the document for a complete overview of the project's design and implementation.

---

## Author
**Steven Rodriguez**

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments
- **Angular** for frontend development.
- **Spring Boot** for robust backend APIs.
- **Docker** for containerization.
- **Bootstrap** for responsive design.

