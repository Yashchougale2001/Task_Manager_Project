# Yash Assessment Project
This is a simple Python Flask project with a MySQL database running inside Docker containers.

## Prerequisites
Make sure you have the following installed on your machine:
- Docker
- Docker Compose

## Getting Started

### 1. Clone the Repository

First, clone this repository to your local machine:

```bash
git clone https://github.com/yourusername/yash_assessment.git
cd yash_assessment

 2. Set Up Environment Variables
You'll need to create a .env file to store your environment variables. You can copy the .env.example file and modify it as needed:
```bash
Copy code
cp .env.example .env
Modify the .env file with your own values (e.g., MYSQL_ROOT_PASSWORD, MYSQL_DATABASE, etc.).

### 3. Build and Run the Containers
Now you can build and run the Docker containers using docker-compose:

bash
Copy code
docker-compose up --build
This command will:

Build the Docker images for the web application.
Set up a MySQL database in a separate container.
Link the containers and start the services.
### Access the Application
Once the containers are up and running, you can access the web application at:

arduino
Copy code
http://localhost:5000
You should see the Flask web app running.

5. Stopping the Application
To stop the running containers, press CTRL+C in the terminal where Docker is running, or run the following command in a new terminal window:

bash
Copy code
docker-compose down
6. Running in Detached Mode
If you prefer to run the containers in detached mode (in the background), use:

bash
Copy code
docker-compose up --build -d
