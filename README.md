# CodeAlpha DevOps Task 2 – Jenkins Remoting Project

## Project Overview

This project demonstrates a distributed Jenkins architecture using:

- Jenkins Master (Controller)
- Docker-based Jenkins Agent (Remote Worker)
- GitHub SCM Integration
- Pipeline defined using Jenkinsfile

## Architecture

GitHub → Jenkins Master → Docker Agent

The Jenkins Master distributes build workloads to a labeled remote Docker agent using Jenkins Remoting.

## Technologies Used

- Jenkins (LTS)
- Docker
- GitHub
- Jenkins Pipeline (Jenkinsfile)

## Key Features Implemented

- Master–Agent Architecture
- Label-based build restriction
- Pipeline as Code (Jenkinsfile)
- Remote build execution
- Secure agent connection using secret key

## How to Run

1. Run Jenkins master container
2. Create remote agent container
3. Configure node in Jenkins
4. Connect GitHub repository
5. Run Pipeline build

## Author

Sabari Karthick
