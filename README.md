# Python-django-app-deployment
# Django Web Application – Docker Deployment

## 📌 Project Overview

This project demonstrates how to containerize and deploy a Django web application using Docker. The application runs inside a Docker container, making it easier to build, deploy, and run consistently across different environments.

The project is deployed on an AWS EC2 Ubuntu instance and can be accessed through its public IP address.

## 🛠️ Technologies Used

- Python
- Django
- Docker
- Linux (Ubuntu)
- AWS EC2
- Git & GitHub

## 📂 Project Structure

```text
python-web-app/
│
├── Dockerfile
├── requirements.txt
├── manage.py
└── devops/
    ├── settings.py
    ├── urls.py
    └── ...
```

## 🐳 Docker Implementation

The Dockerfile automates the application setup:

1. Uses Python as the base image.
2. Creates the application working directory.
3. Installs dependencies from `requirements.txt`.
4. Copies the Django application files.
5. Exposes port 8000.
6. Starts the Django development server.

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/hritikk733/Docker-Zero-to-Hero.git
```

### 2. Navigate to the project directory

```bash
cd Docker-Zero-to-Hero/examples/python-web-app
```

### 3. Build the Docker image

```bash
docker build -t django-app:v1 .
```

### 4. Run the Docker container

```bash
docker run -d -p 8000:8000 --name django-container django-app:v1
```

### 5. Access the application

Open your browser:

```text
http://localhost:8000/demo/
```

## ☁️ AWS EC2 Deployment

The application was deployed on an Ubuntu EC2 instance.

Deployment steps:

- Launched an AWS EC2 Ubuntu instance.
- Connected to EC2 using SSH.
- Installed and configured Docker.
- Built the Django Docker image.
- Ran the application inside a Docker container.
- Configured AWS Security Group inbound rules to allow traffic on port 8000.
- Accessed the application through the EC2 public IP.

## 🎯 Learning Outcomes

- Understanding Dockerfile instructions.
- Building and managing Docker images.
- Running applications inside containers.
- Understanding port mapping and container networking.
- Deploying containerized applications on AWS EC2.
- Using Git and GitHub for version control.

## 👨‍💻 Author

Hritik Dhanve

GitHub: https://github.com/hritikk733
