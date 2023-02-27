# Team information
#### Group name: Two is a Bunch
#### Project name: Simple Linear Regression
#### Team members:
- **Debtanu Ganguly(2204026)**
- **Behnam Ahmadpour**

## How to run the project

This project uses [Vite](https://vitejs.dev/)

First, install dependencies by running:
```
npm install
```

To run a local server type in console:
```
npm run dev
```

## Other available commands:

```
npm run build
```
```
npm run preview
```
## About the Project :

Simple Linear Regression: 

Simple linear regression is used to estimate the relationship between two quantitative variables. You can use simple linear regression when you want to know:
1. How strong the relationship is between two variables (e.g., the relationship between rainfall and soil erosion).
2. The value of the dependent variable at a certain value of the independent variable (e.g., the amount of soil erosion at a certain level of rainfall).

Regression models describe the relationship between variables by fitting a line to the observed data. Linear regression models use a straight line, while logistic and nonlinear regression models use a curved line. Regression allows you to estimate how a dependent variable changes as the independent variable(s) change.


## Overview of my approach :

So calculating Simple Linear Regression and visualiing the data can be done in various ways in JavaScript. Some of them includes :
1. [D3.js](https://d3js.org/) 
2. [Plotly.js](https://plotly.com/javascript/)
3. [Chart.js](https://www.chartjs.org/)
4. [Highchart.js](https://www.highcharts.com/blog/products/highcharts/)

Here in this project I tried to use the **Highcharts JS** methodology.

Highcharts, the core library of our product suite, is a pure JavaScript charting library based on SVG that makes it easy for developers to create responsive, interactive and accessible charts.

Create custom user entered data to calculate the linear regression and visualise using the Highcharts js and produce a Scatter-Plot as the outcome.

The main part includes the Configuration :

Type of the plot to be visualised:
```
var series = {
   type: 'scatter'
};
```
and drawing the chart :
```
$('#container').highcharts(json);
```
## Runnning the project

Run the [index.html](/Users/debtanu/Desktop/THB/WS-2022:23/ADAM/LinearRegression/LR/index.html) and the results will be visualised in the form of scatter plot and Upon moving the mouse over single dots their respective coordinates should be displayed in a small popping up window.

Direct Demo is available at : [LinearRegression_ScatterPlot](https://adam-two-is-a-bunch.github.io/linearregression/)




