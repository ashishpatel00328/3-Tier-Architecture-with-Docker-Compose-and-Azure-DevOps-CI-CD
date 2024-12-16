# 3-Tier-Architecture-with-Docker-Compose-and-Azure-DevOps-CI-CD
This project demonstrates a 3-tier architecture consisting of a React frontend, Node.js backend, and PostgreSQL database. The application is containerized using Docker and deployed to an Azure VM using Azure DevOps CI/CD pipelines.

## Prerequisites:

- Docker
- Docker Compose
- Node.js and npm
- Git
- Azure DevOps account
- Azure subscription
- Getting Started:


## Build and Run Locally:

- Start the Docker Compose:
Bash
```
docker-compose up --build
```
Access the Frontend: Open your browser and go to http://localhost:3000.
Azure DevOps CI/CD:

Create an Azure DevOps Project:

Log in to your Azure DevOps organization.
Create a new project.
Create a Pipeline:

In your project, navigate to Pipelines.
Create a new pipeline.
Choose the YAML pipeline option.
Paste the azure-pipelines.yml content into the editor.
Configure the Azure Container Registry service connection and Azure subscription.
Save and run the pipeline.
Deployment to Azure VM:

Ensure your Azure VM has Docker and Docker Compose installed.
The CI/CD pipeline will automatically deploy the latest images to your Azure VM.
Project Structure:

├── frontend
│   ├── public
│   │   └── index.html
│   ├── src
│   │   ├── App.js
│   │   └── index.js
│   ├── package.json
│   └── Dockerfile
├── backend
│   ├── server.js
│   ├── package.json
│   └── Dockerfile
├── database
│   ├── init.sql
│   └── Dockerfile
├── docker-compose.yml
├── azure-pipelines.yml
└── README.md


Feel free to contribute to this project by submitting pull requests.
