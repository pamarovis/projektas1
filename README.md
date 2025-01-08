# Simple To-Do Web Application
This is a simple web-based to-do application built with HTML, CSS, and JavaScript. It provides a minimalist interface for managing your tasks efficiently. The application allows users to add, edit, mark as complete, and delete tasks effortlessly.

## Features:
* Add Tasks: Easily add new tasks to your to-do list.
* Mark as Complete: Mark tasks as complete when finished.
* Delete Tasks: Remove tasks from the list.
* Responsive Design: Ensures a seamless experience across various devices and screen sizes.
* Local Storage: Tasks are saved locally, ensuring persistence even after browser refresh.
  
## Future Improvements:
* Implementation of user authentication.
* Integration with backend server for data storage.
* Adding due dates and priority levels to tasks. 

## Technologies Used:
* HTML: Provides the structure and content of the web page.
* CSS: Styles the layout and appearance of the application.
* JavaScript: Implements interactive functionality and task management.
* Docker: Packages the application and its dependencies into a container for easy deployment and portability.

## How to Run the Project with Docker

### Prerequisites
Ensure you have Docker installed on your system. You can verify the installation by running:
```bash
docker --version
```

### Steps to Run
1. Clone the repository to your local machine:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```
2. Build the Docker image:
   ```bash
   docker build -t to-do-app .
   ```
3. Run the Docker container:
   ```bash
   docker run -d -p 8080:80 to-do-app
   ```
4. Open your browser and navigate to:
   [http://localhost:8080](http://localhost:8080)

### Stopping the Container
To stop the running container, find its ID using:
```bash
docker ps
```
Then stop it with:
```bash
docker stop <container-id>
```

## Notes
- The Docker image uses `nginx:alpine` as the base image for serving the application.
- Ensure no other service is running on port `8080` before starting the container.
