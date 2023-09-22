# Task 3: Kubernetes Deployment with Spring Boot and MongoDB

This repository contains the implementation of Task 3, which involves deploying a Spring Boot application with MongoDB to a Kubernetes cluster. The task includes creating Docker images for the Spring Boot application and MongoDB, defining Kubernetes YAML manifests, and deploying the application to a Kubernetes cluster.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Requirements](#requirements)
- [Installation Setup](#installation-setup)
- [Project Structure](#project-structure)
- [How the Task is Completed](#how-the-task-is-completed)
- [Screenshots](#screenshots)

## Features

- Creation of Docker images for the Spring Boot application and MongoDB.
- Kubernetes deployment using YAML manifests.
- Isolation of MongoDB in a separate pod.
- Configuration of environment variables for the Spring Boot application.
- Persistent storage for MongoDB data.
- Verification of application accessibility from the host machine.

## Technologies Used

- Spring Boot
- MongoDB
- Docker
- Kubernetes
- YAML
- Maven

## Requirements

Before you begin, ensure you have the following requirements met:

- Docker Desktop or another Kubernetes cluster setup.
- `kubectl` command-line tool installed.
- Maven for building the Spring Boot application.
- Java development environment.

## Installation Setup

Follow these steps to deploy the Spring Boot application with MongoDB to Kubernetes:

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/yourusername/your-repo.git
   cd your-repo

Certainly, here's the updated README.md file with a "Project Structure" section:

markdown
Copy code
# Task 3: Kubernetes Deployment with Spring Boot and MongoDB

This repository contains the implementation of Task 3, which involves deploying a Spring Boot application with MongoDB to a Kubernetes cluster. The task includes creating Docker images for the Spring Boot application and MongoDB, defining Kubernetes YAML manifests, and deploying the application to a Kubernetes cluster.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Requirements](#requirements)
- [Installation Setup](#installation-setup)
- [Project Structure](#project-structure)
- [How the Task is Completed](#how-the-task-is-completed)
- [Screenshots](#screenshots)

## Features

- Creation of Docker images for the Spring Boot application and MongoDB.
- Kubernetes deployment using YAML manifests.
- Isolation of MongoDB in a separate pod.
- Configuration of environment variables for the Spring Boot application.
- Persistent storage for MongoDB data.
- Verification of application accessibility from the host machine.

## Technologies Used

- Spring Boot
- MongoDB
- Docker
- Kubernetes
- YAML
- Maven

## Requirements

Before you begin, ensure you have the following requirements met:

- Docker Desktop or another Kubernetes cluster setup.
- `kubectl` command-line tool installed.
- Maven for building the Spring Boot application.
- Java development environment.

## Installation Setup

Follow these steps to deploy the Spring Boot application with MongoDB to Kubernetes:

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/yourusername/your-repo.git
   cd your-repo

2. Build the Spring Boot application into a JAR file:
   ```bash
    mvn clean package
  The JAR file will be located in the target folder.

3. Create Docker images for the Spring Boot application and MongoDB:
   ```bash
    docker build -t task1-app-image -f "path-to-Dockerfile-for-SpringBoot" .
    docker build -t mongo-image -f "path-to-Dockerfile-for-MongoDB" .

4. Create Kubernetes YAML manifests for the application and MongoDB. The YAML files are located in the k8s folder.

5. Apply the YAML manifests to start the application and MongoDB pods:
   ```bash
    kubectl apply -f "path-to-mongo-deployment.yaml"
    kubectl apply -f "path-to-task1-app-deployment.yaml"

6. Verify that the application is running by checking the pod status:
   ```bash
    kubectl get pods

7. Access the application from your host machine using the provided endpoints.

## Project Structure
The project structure is organized as follows:

- `task3/` 
  - `target/`
    - `Dockerfile`: Dockerfile for the Spring Boot application
    - `mongo/`
      - `Dockerfile`: Dockerfile for MongoDB   
    - `k8s`
      - `mongo-deployment.yaml`: Kubernetes YAML manifest for MongoDB
      - `task1-app-deployment.yaml`: Kubernetes YAML manifest for the Spring Boot application
  - `src/`: Source code for the Spring Boot application
    - `...`: AWS CodeBuild configuration file.
  - `pom.xml `: Maven project configuration
  - `README.md`: Project documentation

## How the Task is Completed

The task is completed by following these steps:

Creation of a Spring Boot application named task1.
Building the Spring Boot application into a JAR file using mvn clean package.
Creation of Docker images for both the Spring Boot application and MongoDB.
Definition of Kubernetes YAML manifests for the application and MongoDB.
Deployment of the application to the Kubernetes cluster using kubectl apply.
Verification of the application's accessibility from the host machine.

## Screenshots

### Here are some screenshots that illustrate the workflow

### Creating an S3 Bucket
![App Screenshot](https://drive.google.com/uc?id=15s1-Idv4xzsA4GwCllDYfmJ3aecEta69)

### Creating an S3 Bucket
![App Screenshot](https://drive.google.com/uc?id=15s1-Idv4xzsA4GwCllDYfmJ3aecEta69)

### Creating an S3 Bucket
![App Screenshot](https://drive.google.com/uc?id=15s1-Idv4xzsA4GwCllDYfmJ3aecEta69)

### Creating an S3 Bucket
![App Screenshot](https://drive.google.com/uc?id=15s1-Idv4xzsA4GwCllDYfmJ3aecEta69)

### Creating an S3 Bucket
![App Screenshot](https://drive.google.com/uc?id=15s1-Idv4xzsA4GwCllDYfmJ3aecEta69)

### Creating an S3 Bucket
![App Screenshot](https://drive.google.com/uc?id=15s1-Idv4xzsA4GwCllDYfmJ3aecEta69)

### Creating an S3 Bucket
![App Screenshot](https://drive.google.com/uc?id=15s1-Idv4xzsA4GwCllDYfmJ3aecEta69)

### Creating an S3 Bucket
![App Screenshot](https://drive.google.com/uc?id=15s1-Idv4xzsA4GwCllDYfmJ3aecEta69)

### Creating an S3 Bucket
![App Screenshot](https://drive.google.com/uc?id=15s1-Idv4xzsA4GwCllDYfmJ3aecEta69)

### Creating an S3 Bucket
![App Screenshot](https://drive.google.com/uc?id=15s1-Idv4xzsA4GwCllDYfmJ3aecEta69)
