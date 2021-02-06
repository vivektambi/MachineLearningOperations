# Project Overview
	The project "Operationalizing Machine Learning" is a part of Udacity ML Nanodegree.
	In this project, we build, deply and consume an Azure ML pipeline using Python SDK, and Swagger Documentation.
# Architectural Diagram
 ![alt text](https://github.com/vivektambi/MachineLearningOperations/blob/master/screenshots/4ArchitecturalDiagram.PNG?raw=true)
# Future Improvements
	1. In the dataset I am using for AutoML model, I will introduce new variables to increase the power of features in the modelling.
	2. In real life ML problems, batches of new data are introduced at regular intervals. Training on the latest data will make our model more robust. 
	Hence, I will introduce an automation where the training happens on regular intervals(hourly/daily/weekly etc.)
	
# Screenshots and Steps
##### Create a new Auto ML run
create a new automl run. As step one, craete a bank dataset. A screenshot of the bank dataset upload is shown below.
![alt text](https://github.com/vivektambi/MachineLearningOperations/blob/master/screenshots/1registeredDatasets.PNG?raw=true)
Screenshot: Registered Dataset
Register the automl experiment. set the minimum nodes in compue as 1 and maximum nodes as 6. A screenshot of the completed experiment is shown below.
![alt text](https://github.com/vivektambi/MachineLearningOperations/blob/master/screenshots/2ExperimentCompleted.PNG?raw=true)
Screenshot: Experiment Completed

##### Select the best run for deployment and Deploy
Once the run is complete, you can observe the accuracy and metrics of all models. Select the best model for deployment. set enable authentication to protect your project pipeline from external attacks. 
![alt text](https://github.com/vivektambi/MachineLearningOperations/blob/master/screenshots/3bestmodel.PNG?raw=true)
Screenshot: Best Model

##### Enable Application insights and produce Run Logs
The model is now deployed. The deployment needs constant monitoring. In the logs.py file, set enableapplications insights as true. Run the logs.py file to get detailed insights about the deployment.
![alt text](https://github.com/vivektambi/MachineLearningOperations/blob/master/screenshots/5ApplicationInsightsEnabled.PNG?raw=true)
Screenshot: Application Insights Enabled

![alt text](https://github.com/vivektambi/MachineLearningOperations/blob/master/screenshots/7logsp2.PNG?raw=true)
![alt text](https://github.com/vivektambi/MachineLearningOperations/blob/master/screenshots/6logsp1.PNG?raw=true)
Screenshot: Logs

##### Interact with Swagger Instance running with documentation
Swagger documentation helps to interact with the api. Create swagger.json file from the endpoints tab. In swagger.sh, set port to 9000. run swagger.sh. Run serve.py. 
Checkout the swagger responses on localhost.
![alt text](https://github.com/vivektambi/MachineLearningOperations/blob/master/screenshots/8swaggerp1.PNG?raw=true)
![alt text](https://github.com/vivektambi/MachineLearningOperations/blob/master/screenshots/9swaggerp2.PNG?raw=true)
![alt text](https://github.com/vivektambi/MachineLearningOperations/blob/master/screenshots/10swaggerp3.PNG?raw=true)
![alt text](https://github.com/vivektambi/MachineLearningOperations/blob/master/screenshots/11swaggerp4responses.PNG?raw=true)
Screenshot: Swagger Documentation and Responses

##### Modify and Run the Endpoint.py file
update endpoint.py file. update the uri, primary key and input data. run endpoint.py file to interact with the endpoint.
![alt text](https://github.com/vivektambi/MachineLearningOperations/blob/master/screenshots/12endpoint.PNG?raw=true)
Screenshot: Endpoint
![alt text](https://github.com/vivektambi/MachineLearningOperations/blob/master/screenshots/13endpointOutput.PNG?raw=true)
Screenshot: Endpoint Output

## Screenshots from Python SDK steps
![alt text](https://github.com/vivektambi/MachineLearningOperations/blob/master/screenshots/sdk1pipelineCreated.PNG?raw=true)
Screenshot: Pipeline Created

![alt text](https://github.com/vivektambi/MachineLearningOperations/blob/master/screenshots/sdk2pipelineEndpoint.PNG?raw=true)
Screenshot: Pipeline Endpoint

![alt text](https://github.com/vivektambi/MachineLearningOperations/blob/master/screenshots/sdk3pipelineOverviewEndpoint.PNG?raw=true)
Screenshot: Pipeline Overview Endpoint

![alt text](https://github.com/vivektambi/MachineLearningOperations/blob/master/screenshots/sdk4JupyterRundetails.PNG?raw=true)
Screenshot: Jupyter Run Details

![alt text](https://github.com/vivektambi/MachineLearningOperations/blob/master/screenshots/sdk5Scheduled%20Runs.PNG?raw=true)
Screenshot: Scheduled Runs

![alt text](https://github.com/vivektambi/MachineLearningOperations/blob/master/screenshots/sdk6BankMarketingDatasetWithAMLNEW.PNG?raw=true)
Screenshot: Bank Marketing Dataset with AML

# Screencast Video Link
https://youtu.be/-RNkJgt_7kQ
