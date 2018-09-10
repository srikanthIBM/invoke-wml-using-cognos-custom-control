# invoke-wml-using-cognos-custom-control
***Work In Progress***

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

* [d3js](https://d3js.org/) - Develop charts like pie, bar, or some fancy charts sunburst etc which can later be imported to cognos application.

* Cognos (version 11.0.11) BI server - On Prim version of Cognos.
