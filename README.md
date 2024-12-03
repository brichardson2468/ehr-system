
# MediTrack

An electronic health records (EHR) system built with Java, Maven, and Spring Boot.

## Table of Contents

- [About](#about)
- [Features](#features)
- [System Architecture](#system-architecture)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Testing](#testing)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Acknowledgements](#acknowledgements)

## About

MediTrack is a web-based electronic health records system designed to help healthcare professionals manage patient data efficiently and securely. The application allows users to store, retrieve, and update patient information, medical histories, appointments, and treatment plans.

## Features

- **Patient Management**: Add, view, edit, and delete patient records with comprehensive details.
- **Appointment Scheduling**: Schedule and manage appointments between patients and healthcare providers.
- **Medical History Tracking**: Document and track patient diagnoses, treatments, lab results, and medications.
- **User Authentication and Authorization**: Secure login system with role-based access control for different user types (doctors, nurses, administrators).
- **Search and Filter**: Advanced search functionality to find patients, appointments, or records quickly.
- **Responsive UI**: User-friendly interface compatible with desktops, tablets, and mobile devices.
- **Data Security**: Implements encryption and follows best practices to ensure patient data privacy and compliance with healthcare regulations.
- **Audit Logging**: Tracks user activities for compliance and auditing purposes.

## System Architecture

MediTrack is built on a multi-layered architecture:

- **Presentation Layer**: Handles user interaction using Spring MVC and Thymeleaf templates.
- **Business Logic Layer**: Contains the application's business logic and services.
- **Data Access Layer**: Manages data persistence using Hibernate and JPA repositories.
- **Database Layer**: Uses MySQL for data storage.

<!-- Placeholder for an architecture diagram -->
<!-- ![System Architecture Diagram](path_to_diagram.png) -->

## Technologies Used

- **Java 11**
- **Spring Boot 2.5**
- **Maven**
- **Spring MVC**
- **Hibernate & JPA**
- **MySQL**
- **Thymeleaf**
- **Bootstrap 4**
- **JUnit 5**
- **Mockito**

## Installation

### Prerequisites

- **Java Development Kit (JDK) 11 or higher**
- **Apache Maven 3.6+**
- **MySQL Server**
- **Git**
- **An IDE (IntelliJ IDEA, Eclipse, etc.)**

### Steps

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/meditrack.git
   cd meditrack

	2.	Configure the database
	•	Create a new MySQL database called meditrack_db.
	•	Update the database configurations in src/main/resources/application.properties:

spring.datasource.url=jdbc:mysql://localhost:3306/meditrack_db
spring.datasource.username=your_mysql_username
spring.datasource.password=your_mysql_password
spring.jpa.hibernate.ddl-auto=update


	3.	Build the project

mvn clean install


	4.	Run the application

mvn spring-boot:run


	5.	Access the application
Open your web browser and navigate to http://localhost:8080.

Usage

Default Credentials

	•	Administrator

Username: admin
Password: admin123


	•	Doctor

Username: doctor
Password: doctor123



Navigating the Application

	•	Dashboard: Provides an overview of the system including statistics and recent activity.
	•	Patients: Manage patient records.
	•	Appointments: Schedule and manage appointments.
	•	Medical Records: Access and update patient medical histories.
	•	Users: Manage user accounts and roles (available to administrators).

Adding a New Patient

	1.	Navigate to the “Patients” section.
	2.	Click on “Add New Patient”.
	3.	Fill in the required details and save.

Scheduling an Appointment

	1.	Go to the “Appointments” section.
	2.	Click on “Schedule Appointment”.
	3.	Select the patient, date, time, and healthcare provider.
	4.	Save the appointment.

Testing

To run the unit and integration tests:

mvn test

Test reports will be generated in the target/surefire-reports directory.

Contributing

Contributions are welcome! Please follow these steps:
	1.	Fork the repository.
	2.	Clone your fork:

git clone https://github.com/yourusername/meditrack.git


	3.	Create a branch for your feature or bugfix:

git checkout -b feature/your-feature-name


	4.	Commit your changes:

git commit -am 'Add new feature'


	5.	Push to your branch:

git push origin feature/your-feature-name


	6.	Submit a Pull Request detailing your changes.

License

This project is licensed under the MIT License - see the LICENSE file for details.

Contact

	•	Your Name
	•	Email: your.email@example.com
	•	LinkedIn: Your LinkedIn Profile
	•	GitHub: yourusername

Acknowledgements

	•	Spring Boot Documentation
	•	Thymeleaf
	•	Bootstrap
	•	Hibernate ORM
	•	MySQL
