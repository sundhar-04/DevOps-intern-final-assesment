# DevOps-intern-final-assesment
Name : Sundharesan
Date : 02-02-2026
Project Ddescreption : This project demonstrates a basic DevOps workflow using GitHub, Linux scripting, Docker, CI/CD with GitHub Actions, Nomad, and monitoring with Grafana Loki. The project is developed using GitHub Codespaces, which provides a Linux-based environment without requiring a local Linux setup. It showcases essential DevOps concepts through a simple, end-to-end pipeline.

## Docker
This project includes a simple Dockerfile to containerize the Python script `hello.py`.

### Build the Docker image
```bash
docker build -t hello-devops .
```
### Run
```bash
docker run --rm hello-devops
```

#### CI Status Badge
[![Python CI](https://github.com/sundhar-04/DevOps-intern-final-assesment/actions/workflows/ci.yml/badge.svg)](https://github.com/sundhar-04/DevOps-intern-final-assesment/actions/workflows/ci.yml)



## Nomad Job Deployment

This project includes a Nomad job file to run the Docker container.

### Run the Nomad job
```bash
nomad job run nomad/hello.nomad
```

## MLflow Dummy Experiment

This folder contains a simple example of logging a dummy experiment using **MLflow**.

### Files

- `mlflow_dummy.py` – Python script that logs a dummy experiment with:
  - Parameters: `param1`, `param2`
  - Metric: `accuracy`
  - Artifact: `dummy_file.txt`  
  The script **automatically creates the artifact file and logs it** to MLflow.
- `dummy_file.txt` – Example artifact created by the experiment.

### How to Run

 Run the dummy experiment

```bash
python mlflow_dummy.py
