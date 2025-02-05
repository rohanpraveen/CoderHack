## Overview

A RESTful API service built with Spring Boot to manage the leaderboard for a coding platform. The application uses MongoDB to persist user data.

## Features

- **User Registration**: Register a new user with a unique User ID and Username.
- **Update Score**: Update the score of a specific user.
- **Badge Awarding**: Award badges to users based on their scores.
  - 1 <= Score < 30 -> Code Ninja
  - 30 <= Score < 60 -> Code Champ
  - 60 <= Score <= 100 -> Code Master
- **User Retrieval**: Retrieve a list of all registered users.
- **User Deletion**: Deregister a specific user from the contest.

## Installation and Usage

### Prerequisites

- Java 17 or higher
- MongoDB
- Postman for API testing

### Getting Started

1. **Clone the repository:**

    ```bash
    git clone https://github.com/pgprajwal/CoderHack.git
    ```

2. **Navigate to the project directory:**

    ```bash
    cd CoderHack
    ```

3. **Build and run the application using Gradle:**

    ```bash
    ./gradlew bootrun
    ```

## API Endpoints

- **GET /users** - Retrieve a list of all registered users
- **GET /users/{userId}** - Retrieve the details of a specific user
- **POST /users** - Register a new user to the contest
- **PUT /users/{userId}** - Update the score of a specific user
- **DELETE /users/{userId}** - Deregister a specific user from the contest

## API Testing

For testing the API endpoints, you can use the following [Postman Collection](https://www.postman.com/pgprajwal/workspace/api-repository/collection/34348286-160e56c8-d6fe-4195-b63b-e1857bf5bb6d?action=share&creator=34348286)
