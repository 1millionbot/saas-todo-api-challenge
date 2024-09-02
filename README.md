# Technical assessment: Backend Developer - SaaS To Do list API
## Objective
Develop a RESTful API for a SaaS-based "To Do List" application that allows users to manage tasks. The API must include full CRUD operations, user authentication, and multi-tenancy support. Additionally, the application should be containerized using Docker for easy deployment.

## Requirements
1. Core features
- User authentication: Implement user registration and login functionality. Each user should have their own workspace to manage tasks.
- Multi-Tenancy: Ensure that tasks are isolated per user (i.e., User A cannot see User B's tasks).
- CRUD operations on tasks:
  - Create task: Users can create a task with a title, description, and status.
  - Read tasks: Users can retrieve a list of all their tasks or a specific task by its ID.
  - Update task: Users can update the title, description, or status (completed/not completed) of a task.
  - Delete task: Users can delete a task by its ID.
- Task sharing: Implement a feature where users can share tasks with other users. Shared tasks should appear in both users' task lists.
2. Middleware
- Implement a middleware that logs every incoming request. The middleware should capture:
  - The requested URL.
  - The HTTP method used.
  - The timestamp of the request.
  - The execution time of the request.
- Implement any other needed middleware.
- Optionally, extend the middleware to log the authenticated user’s ID and the user’s role (e.g., admin, user).
3. Docker
- Create a Dockerfile to build a Docker image for the application.
- Create a docker-compose.yml file that sets up the application, including any required services such as the database.
- Ensure the application can be fully run within Docker containers.
4. SaaS considerations
- Subscription plans: Simulate different subscription tiers with varying levels of access (e.g., free plan with a limit on the number of tasks, premium plan with unlimited tasks). This can be implemented using feature flags or a simple conditional check based on the user's plan.
- Rate limiting: Implement rate limiting for API requests based on the user's subscription plan.
 

## Technical specifications
- Language & framework: You may use Node.js (Express or Fastify).
- Database: Preferably use a relational database such as PostgreSQL or MySQL, but other databases are acceptable.
- Authentication: Implement authentication using JWT (JSON Web Tokens) or session-based authentication.
- Testing: Include unit tests for key functionalities.
- Documentation: Provide clear documentation in a README.md file, including instructions on how to set up, run, and use the application both locally and in Docker.
- Evaluation bonus: You can implement any other feature or improvement (e.g: basic frontend application, postman file to test endpoints, file attachment to the task, etc.)


## Deliverables
1. Source code: 
- Push the complete source code to a private GitHub repository.
- Include the Dockerfile and docker-compose.yml.
- Ensure the repository is well-structured and the code is clean and organized.
2. Documentation:
- Include a README.md file with:
  - A description of the project.
  - Setup and installation instructions.
  - API usage examples.
  - Instructions for running the application in Docker.
  - Notes on middleware, subscription plans, and rate limiting.


## Submission deadline
You have 7 days from the date of assignment to complete the assessment and push it to GitHub.

## How to submit
- Create a private repository on GitHub.
- Notify us via email once you have completed the assessment with the link to the repository.
