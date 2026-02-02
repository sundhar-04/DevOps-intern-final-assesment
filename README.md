# DevOps-intern-final-assesment
Name : Sundharesan
Date : 02-02-2026
Project Ddescreption : This project demonstrates a basic DevOps workflow using GitHub, Linux scripting, Docker, CI/CD with GitHub Actions, Nomad, and monitoring with Grafana Loki. The project is developed using GitHub Codespaces, which provides a Linux-based environment without requiring a local Linux setup. It showcases essential DevOps concepts through a simple, end-to-end pipeline.

## Docker
This project includes a simple Dockerfile to containerize the Python script `hello.py`.

### Build the Docker image
```bash
docker build -t hello-devops .

### Run
docker run --rm hello-devops
