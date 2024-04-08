# Spring Filter Custom Fields Application

This Spring Boot application demonstrates how to filter custom fields from a User object based on user input.

## Overview
The application includes a UserController that exposes an endpoint to retrieve a User object with specified fields. The filterFields method in the controller filters out fields that are not included in the request parameter.

## Getting Started

### Prerequisites
- Java JDK 8 or higher
- Maven
### Installation
1. Clone the repository:
```bash
  git clone https://github.com/abhishekshah2905/spring-filter-custom-fields.git
```
2. Navigate to the project directory:
```bash
  cd spring-filter-custom-fields
```
3. Build the project:
```bash
  mvn clean install
```
4. Run the application:
```bash
  mvn spring-boot:run
```
5. Access the application at http://localhost:8089

### Usage
- Use the / endpoint with a query parameter fields to specify which fields to include in the response. For example, /users?fields=name,age will return a User object with only the name and age fields.