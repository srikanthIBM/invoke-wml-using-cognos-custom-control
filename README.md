# invoke-wml-using-cognos-custom-control
***Work In Progress***

It is always a tedious task to see a real time Watson Machine Learning(wml) model output from Cognos application. 
To achieve that, we then need to have an external mechanism to invoke the model, pass the required input parameters and finally the scores are written back to the database. Cognos reads the latest scores from the database and displays on the dashboard. This is a little tedious process of displaying the machine learning model outputs at run time.

The latest version of Cognos comes with Custom control feature. It gives the capability to create a real time dashboard where we can pass the inputs through a custom widget which internally invokes the model through REST API, gets the output and displays on the dashboard.

For this, one need to build a custom widget using Java Script to get inputs and to show outputs as d3 chart. Then this widget can be imported into Cognos dashboard and gets real time output.
In this pattern, we will demonstrate to build custom widget, integration of the custom widget in Cognos and to invoke the Machine learning model from the Cognos Dashboard.
The dataset considered here is Telecom sample customer data, using that data we Predict behaviour to retain the customers. You can analyse all relevant customer data and develop focused customer retention programs.
For this, one need to build a custom widget using Java Script to get inputs and to show outputs as [d3 chart](https://d3js.org/). Then this widget can be imported into Cognos dashboard and gets real time output.

After going through this code pattern, you should be able to:
- create a real time dashboard using cognos custom control.
- can invoke machine learning or predictive models hosted on cloud.
- can import the external java script build charts to cognos application.

## Flow

![WRML_Cognos](https://github.com/srikanthIBM/invoke-wml-using-cognos-custom-control/blob/master/images/RWML_Arch.png)

1. Create the forms using js and charts using D3js.
2. Create Watson Machine Learning or the predictive Model.
3. Launch Cognos either on Google chrome or mozilla firefox.
4. From the cognos dashboard, pass the input parameters in the form and click submit button.
5. Invokes ML models based on the input paramaeters.
6. Gets output from the model and sends to the cognos dashboard to display


# Included Components

* [JavaScript](https://www.w3schools.com/js/) - Develop forms to capture user inputs, later these forms can be imported to cognos dashboards.

* [IBM Watson Studio](https://www.ibm.com/cloud/watson-studio): Analyze data using RStudio, Jupyter, and Python in a configured, collaborative environment that includes IBM value-adds, such as managed Spark.

* [IBM Cloud Object Storage](https://console.bluemix.net/catalog/services/cloud-object-storage): An IBM Cloud service that provides an unstructured cloud data store to build and deliver cost effective apps and services with high reliability and fast speed to market. This code pattern uses Cloud Object Storage.

* [d3js](https://d3js.org/) - Develop charts like pie, bar, or some fancy charts sunburst etc which can later be imported to cognos application.

* Cognos (version 11.0.11) BI server - On Prim version of Cognos.

## Featured Technologies

* [D3js](https://d3js.org/):  
* [Analytics](https://developer.ibm.com/code/technologies/analytics/): Analytics delivers the value of data for the enterprise.
* [Cognos Analytics](https://www.computerworld.com/article/2906336/emerging-technology/what-is-artificial-intelligence.html):  

## Watch The Video

Will be uploaded shortly.



## Steps
Follow these steps to setup and run this code pattern. The steps are described in detail below.
1. [Pre-requisites](#1-pre-requisites)
2. [Create watson machine learning model](#2-create-watson-machine-learning-model)
3. [Create custom control widgets](#3-create-custom-control-widgets)
4. [Build cognos report and import custom widget](#4-build-cognos-report-and-import-custom-widget)
5. [Analyse the invoked machine learning model](#5-analyse-the-invoked-machine-learning-model)




## 1. Pre-requisites

- Admin access to cognos 11.0.11 server to place javascript files to the cognos webcontent folder.

- IBM Cloud account: You must have IBM Cloud account to work with this code pattern. If you do not have an IBM Cloud account, you can create a one month free trail account [here](https://console.bluemix.net/)



## 2. Create watson machine learning model

- Follow the steps documented in the below link which has [IBM Watson Studio guided demo](https://www.ibm.com/cloud/garage/demo/try-watson-machine-learning/): Create a learning model to predict customer churn.
Get experience with IBM Watson Studio by creating a decision-tree machine-learning model to evaluate the risk that a customer might leave your service.

- Create a new Watson Studio project

Sign up for IBM's [Watson Studio](http://dataplatform.ibm.com/). 

Click on New project and select Data Science as per below.

![](https://github.com/IBM/xgboost-smote-detect-fraud/blob/master/image/new_project.PNG)

Define the project by giving a Name and hit 'Create'.

![](https://github.com/IBM/xgboost-smote-detect-fraud/blob/master/image/define_project.PNG)

By creating a project in Watson Studio a free tier ``Object Storage`` service will be created in your IBM Cloud account. Choose the storage type as Cloud Object Storage for this code pattern.







## 3. Create custom control widgets



## 4. Build cognos report and import custom widget


## 5. Analyse the invoked machine learning model





