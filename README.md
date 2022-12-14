*NOTE:* This file is a template that you can use to create the README for your project. The *TODO* comments below will highlight the information you should be sure to include.


# Operationalizing Machine Learning

## Overview
In this project which is a part of the Azure ML Engineer Nanodegree, we continued to work with the Bank Marketing dataset.
We used Azure to configure a cloud-based machine learning production model, deploy it, and consume it. We also learned 
to create, publish, and consume a pipeline.

## Architectural Diagram
![image](/Users/nikhilrego/Documents/Projects/operationalizing-machine-learning/images/architectural-diagram.png)

## Key Steps
1. Authentication : In this step we were supposed to create a Security Principal (SP) to interact with the Azure Workspace.
I skipped this step as I am not using my own Azure account but instead using the lab Udacity account.
2. Automated ML Experiment : I configured a compute cluster (Standard_DS3_v2) and set up an Automated ML experiment. 
I then proceeded to run the experiment and identified the best model.
3. Deploy the best model : I deployed the best model using Azure Container Instance (ACI) with authentication enabled. 
This allowed me to interact with the HTTP API service and the model by sending data over POST requests.
4. Enable logging : I created a virtual conda environment and installed *az* as well as the Python SDK for Azure.
 Logging helped monitor the deployed model and keep track of the request frequency, latency, etc.
5. Swagger Documentation :  I downloaded *swagger.json* and ran both *swagger.json* and *serve.py*. I interacted
with the swagger instance running with the documentation for the HTTP API for the model.
6. Consume model endpoints : I successfully demonstrated the model was consumable by modifying and running *endpoint.py*.
7. Create and publish a pipeline : I uploaded and updated the jupyter notebook provided to match the environment.
8. Documentation:

## Screen Recording
*TODO* Provide a link to a screen recording of the project in action. Remember that the screencast should demonstrate:

## Standout Suggestions
One small modification I made was to use environment variables to pass sensitive arguments to my scripts. This is a 
good practice as a machine learning engineer to secure passwords, keys, ...etc.