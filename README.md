[![CircleCI](https://dl.circleci.com/status-badge/img/gh/Peculiar907/microservice-projects/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Peculiar907/microservice-projects/tree/master)

## Project Overview

In this project, i will apply the skills i have acquired in the Udacity cloud Devops Nanodegree program to operationalize a Machine Learning Microservice API. 

The project contains a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on.  Read more about the data, which was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). This project tests the ability to operationalize a Python flask app—in a provided file, `app.py`—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

### Project Tasks

The project goal is to operationalize this working, machine learning microservice using [kubernetes](https://kubernetes.io/), which is an open-source system for automating the management of containerized applications. In this project i will:
* Test the project code using linting
* Complete a Dockerfile to containerize this application
* Deploy the containerized application using Docker and make a prediction
* Improve the log statements in the source code for this application
* Configure Kubernetes and create a Kubernetes cluster
* Deploy a container using Kubernetes and make a prediction
* Upload a complete Github repo with CircleCI to indicate that the code has been tested

More details of the  can be find in  detailed [project rubric, here](https://review.udacity.com/#!/rubrics/2576/view).

**The final implementation of the project will showcase your abilities to operationalize production microservices.**

---

## Setup the Environment

* Create a virtualenv with Python 3.7 and activate it. Refer to this link for help on specifying the Python version in the virtualenv. 
```bash
python3 -m venv ~/.devops
source ~/.devops/bin/activate


```
* Run `make install` to install the necessary dependencies
* Run Lint checks
 make lint


### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

### Kubernetes Steps

* Setup and Configure Docker on your Local system
* Setup and Configure Kubernetes on your local system
* Run `./run_docker.sh` in a terminal to prepare and build the image.
* Run `./make_prediction.sh` in a seperate terminal to get the predication of the application running in a container.
* Setup Minikube
* Install Kubectl
* Run `Minikube Start`
* Run the pod in a terminal using `./run_kubernetes.sh`
* Run `./make_prediction.sh` in a seperate terminatal.
