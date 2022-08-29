# Operationalize Machine Learning Microservice API.
[![CircleCI](https://dl.circleci.com/status-badge/img/gh/rayotoo/MLOps-Project/tree/main.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/rayotoo/MLOps-Project/tree/main)

## Project Overview

The goal of the project was to operationalize a working, machine learning microservice using [kubernetes](https://kubernetes.io/), which is an open-source system for automating the management of containerized applications.With a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. `The Data` : [the data source site](https://www.kaggle.com/c/boston-housing). This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

### Tasks performed for this project

* Linting was used to test the project code
* A Dockerfile was written and used to containerize this application
* The application was deployed using Docker and was used to make a prediction
* Kubernetes was configured and used to create a cluster 
* The application was deployed using Kubernetes and afterwards, used to make a prediction
* The project was tested with CircleCI 



**The final implementation of the project will showcase your abilities to operationalize production microservices.**

---

## Setup the Environment

* Create a virtualenv with Python 3.7 and activate it. Refer to this link for help on specifying the Python version in the virtualenv. 
```bash
python3 -m pip install --user virtualenv
# You should have Python 3.7 available in your host. 
# Use a command similar to this one:
python3 -m virtualenv --python=<path-to-Python3.7> .devops
source .devops/bin/activate
```
* Run `make install` to install the necessary dependencies
* Install hadolint using
```
brew install hadolint
```
* install minikube using
```
brew install minikube
```
* Install docker from site `https://docs.docker.com/v17.12/install/`

---
### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`
---
### Kubernetes Steps

* Setup and Configure Docker locally
* Setup and Configure Kubernetes locally
* Create Flask app in Container
* Run via kubectl
---
## Files in the repository.
The `output_txt_files` directory contains 3 files:
1. Output including all log statements and the health of an interaction `docker_out.txt`.
2. Output of kubenetes including the pod’s name and status, as well as the port forwarding and handling text. `kuberbetes.out.txt`.
3. Output after running a prediction via Kubernetes deployment`kubernetes_out.txt`.

