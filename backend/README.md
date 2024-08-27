# Task Management System with Redis

## Project Overview
This project is a task management system built using Redis for queuing tasks and Express.js for the API. The system is designed with scalability in mind, utilizing a cluster setup to make full use of multiple CPU cores.

## Prerequisites
- Node.js and npm installed.
- Redis server running.
- Environment variables set for Redis configuration.

## Project Structure
- **`app.js`**: Main application file.
- **`taskRouter.js`**: Router for task-related routes.
- **`taskController.js`**: Controller handling task requests.
- **`taskQueue.js`**: Service for queuing tasks.
- **`redisConfig.js`**: Configuration for Redis connection.
- **`logs/task.log`**: Log file for task completion.

## Running the Project

1. **Install dependencies**:
    ```bash
    npm install
    ```

2. **Set up environment variables**:
    Create a `.env` file with the following variables:
    ```bash
    REDIS_HOST=127.0.0.1
    REDIS_PORT=6379
    REDIS_USER=your_redis_username
    REDIS_PASSWORD=your_redis_password
    ```

3. **Start the Redis server**:
    Ensure that the Redis server is running.

4. **Run the project**:
    ```bash
    npm start
    ```
    This will start the server on the specified port.

## API Endpoints

- **POST `/api/v1/task`**: Queue a task.
  - **Request Body**:
    ```json
    { "user_id": "string" }
    ```
  - **Response**:
    ```json
    { "message": "Task queued successfully" }
    ```

## Live Deployment
The backend is live and deployed on Render.com:
- **Live Backend**: [RedisProject on Render](https://redisproject.onrender.com)

## Portfolio
You can view my portfolio here:
- **Portfolio**: [itsaadi04.codeclout.in](https://itsaadi04.codeclout.in)

## Acknowledgments
Thank you for the opportunity to work on this project. I look forward to any feedback you may have.

---

**Author**: [Your Name]
