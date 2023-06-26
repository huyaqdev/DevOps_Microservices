[![CircleCI](https://dl.circleci.com/status-badge/img/gh/huyaqdev/DevOps_Microservices/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/huyaqdev/DevOps_Microservices/tree/main)

## Project Overview

In this project, you will apply the skills you have acquired in this course to operationalize a Machine Learning Microservice API. Project using a pre-trained model that could predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on.

### Project Tasks

* Test project code using linting: hadolint
* Complete a Dockerfile to containerize this application
* Deploy containerized application using Docker and make a prediction
* Improve the log statements in the source code
* Configure Kubernetes and create a Kubernetes cluster
* Deploy a container using Kubernetes and make a prediction
* Upload a complete Github repo with CircleCI

---

### Run project
* Start minikube
`minikube start`
* Forward in kubernetes
`./run_kubernetes.sh`
* Input payload to get prediction
`./make_prediction.sh`
* Delete minikube cluster
`minikube delete`

### Files explanation
* app.py: use to serve house prediction through api
* docker_out.txt: the output of server (log)
* kubernetes_out.txt: the prediction result when run kubernetes
* Dockerfile: setup build image
* Makefile: env setup and lint test
* run_docker.sh: run docker local
* make_prediction.sh: send input payload to get prediction
* upload_docker.sh: upload image to docker hub
* run_kubernetes.sh: run application in kubernetes
