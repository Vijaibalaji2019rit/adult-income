# adult-income
an machine learning for census about adult income

![image](https://user-images.githubusercontent.com/90760885/152102380-54b44fee-ffe9-43ef-80af-1900f9e7c057.png)
dataset visualization:
![image](https://user-images.githubusercontent.com/90760885/152102469-659b74dc-6d9e-4694-955e-0ca850dd05c9.png)
train model visualization:
![image](https://user-images.githubusercontent.com/90760885/152102754-18c7cef5-a232-46a4-8b9e-fd8c4b0c360d.png)




https://gallery.cortanaintelligence.com/Experiment/adult-income-2022

In this session
• Sing Up FREE Azure ML Studio Subscription
• Create Azure ML Studio workspace
• Train, Test, Evaluate for Binary Classification
• Import census income dataset
• Create a new Azure Machine Learning experiment
• Train and evaluate a prediction model
• Type of datasets
 

First experiment model
Sing Up FREE Azure ML Studio Subscription
https://studio.azureml.net/

Sing Up FREE Azure ML Studio Subscription

Free Workspace -> sign up here  

Create Azure ML Studio workspace
Go to the Azure portal https://portal.azure.com
Click +New
Select Internet of Things, click Machine Learning Workspace, then click Create
Workspace name = ws1
Subscription = defult
Resource group = Create new: rs1
Location = Southeast Asia
Storage account = Create new: names1
Workspace pricing tier = Standard
Web service plan = Create new: ws1Plan
Click No pricing tier selected
Click DEVTEST
Click Pin to dashboard
Click Create
Click at Machine Learning workgroup on dashboard
Click Launch Machine Learning Studio
Blank, new ML Studio workspace
Predicting whether a person’s income exceeds $50,000 per year based on his demographics or census data

Download, prepare, and upload a census income dataset.
Create a new Azure Machine Learning experiment.
Train and evaluate a prediction model.
The overall workflow of the experiment
• Create New blank experiment. Name = Adult Income 1 • Click Data Input and Output • Drag & drop Import Data

Configure Import data module:
• Data source = Web URL via HTTP
• Data source URL = http://archive.ics.uci.edu/ml/ machine-learning-databases/adult/adult.data • Data format = CSV • Run experiment • Right click at the output of Import Data • Click Visualize • Click on Col2 • Look at Statistics and Histogram

Split up the dataset
• Training data This grouping is used for creating our new predictive model based on the inherent patterns found in the historical data via the ML algorithm we use for the solution. • Validation data This grouping is used for testing the new predictive model against known outcomes to determine accuracy and probabilities.

Add Split Data:
• Click Data Transformation
• Click Sample and Split • Drag & drop Split Data module into canvas • Connect Import Data to Split Data • Set properties Fraction of row to 0.80 • Add Two-Class Boosted Decision Tree and Train Model • Connect Two-Class Boosted Decision Tree to Train Model • Connect Split Data to Train Model • Click Train Model • Click Launch column selector • Include col15 • Click • Save • Run

Score the model:
• Add Score Model to canvas • Connect Score Model to Train and Split model • Run

Visualize the model results
• Visualize output of Score Model • Scored Labels This column denotes the model’s prediction for this row of the dataset. • Scored Probabilities This column denotes the numerical probability (or the likelihood) of whether the income level for this row exceeds $50,000.  

Type of datasets
Training set
• A set of examples used for learning • Where the answer value is known.

Validation set
• A set of examples data • Used to tune the architecture of a classifier • And estimate the error

Test set
• Use to test the performances of a classifier • Never used during the training process • Give estimate of error

project link:
https://gallery.cortanaintelligence.com/Experiment/adult-income-2022
