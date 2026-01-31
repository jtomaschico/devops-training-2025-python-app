# DevOps Training 2025 - Python App

Repository for the Python app used in the course to practice CI/CD DevOps strategies for interpreted-language projects.

## Course context
- Tools: Jenkins (on-prem), GitHub/GitLab (SaaS), and Azure DevOps (cloud 360 platform).
- This `feat/base` branch contains the minimal code to start the training and the statements for all practices.

## Project repositories and branches
- Python app: https://github.com/contreras-adr/devops-training-2025-python-app/tree/feat/base
- Java app: https://github.com/contreras-adr/devops-training-2025-java-app/tree/feat/base
- IaC/DevOps: https://github.com/contreras-adr/devops-training-2025-iac-devops/tree/feat/base


## Repository purpose
- Simple Python application with container support.
- Base for pipelines, tests, and deployments across different CI/CD systems.


## Local usage guide

### Run the app with Docker
```bash
docker build -t my-app:0.0.1 -f devops/Dockerfile .
docker run -d --name app1 -p 8080:5000 my-app:0.0.1
docker exec -it app1 bash
docker stop app1
docker start app1
docker logs app1
```

### Run db and app with Docker Compose
```bash
docker-compose up -d
curl localhost:5001
```
