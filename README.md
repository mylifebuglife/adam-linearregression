# Team information - ADAM - MSc Informatics - Sem 1
#### Group name: **Two is a Bunch**
#### Project name: **Simple Linear Regression**
#### Team members:
- **Debtanu Ganguly(2204026)**

Project Demo is available at : [LinearRegression_ScatterPlot](https://adam-two-is-a-bunch.github.io/linearregression/)

## Running the project

Run the [index.html](https://github.com/mylifebuglife/adam-linearregression/blob/master/index.html) and the results will be visualised in the form of scatter plot and Upon moving the mouse over single dots their respective coordinates should be displayed in a small popping up window.

Values to be displayed on the chart can be configured manually in the **data** section of the code.
Data set by me :
```
{
                    type: 'scatter',
                    name: 'Observations',
                    data: [0.5, 2, 3, 3.2, 4.4, 5],
                    marker: {
                        radius: 4
                    }
                }
```

Project Demo is available at : [LinearRegression_ScatterPlot](https://adam-two-is-a-bunch.github.io/linearregression/)

## About the Project :

**Simple Linear Regression**: 

Simple linear regression is used to estimate the relationship between two quantitative variables. You can use simple linear regression when you want to know:
1. How strong the relationship is between two variables (e.g., the relationship between rainfall and soil erosion).
2. The value of the dependent variable at a certain value of the independent variable (e.g., the amount of soil erosion at a certain level of rainfall).

Regression models describe the relationship between variables by fitting a line to the observed data. Linear regression models use a straight line, while logistic and nonlinear regression models use a curved line. Regression allows you to estimate how a dependent variable changes as the independent variable(s) change.

Consider the model function :

![alt text](https://wikimedia.org/api/rest_v1/media/math/render/svg/bf2c1cac7c1e6c9a426d92e9adad6ff4d8b4152e
)

which describes a line with slope β and y-intercept α. In general such a relationship may not hold exactly for the largely unobserved population of values of the independent and dependent variables; we call the unobserved deviations from the above equation the errors. Suppose we observe n data pairs and call them {(xi, yi), i = 1, ..., n}. We can describe the underlying relationship between yi and xi involving this error term εi by

![alt text](https://wikimedia.org/api/rest_v1/media/math/render/svg/968be557dd22b1a2e536b8d22369cfdb37f58703)

This relationship between the true (but unobserved) underlying parameters α and β and the data points is called a linear regression model.

Example : 

Here the dependent variable (GDP growth) is presumed to be in a linear relationship with the changes in the unemployment rate.

![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/7/77/Okuns_law_quarterly_differences.svg/600px-Okuns_law_quarterly_differences.svg.png)


**Scatter Plot** :

A scatter plot (also called a scatterplot, scatter graph, scatter chart, scattergram, or scatter diagram)is a type of plot or mathematical diagram using Cartesian coordinates to display values for typically two variables for a set of data. If the points are coded (color/shape/size), one additional variable can be displayed. The data are displayed as a collection of points, each having the value of one variable determining the position on the horizontal axis and the value of the other variable determining the position on the vertical axis.

![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/a/af/Scatter_diagram_for_quality_characteristic_XXX.svg/440px-Scatter_diagram_for_quality_characteristic_XXX.svg.png)

Scatter Plot Matrices :

For a set of data variables (dimensions) X1, X2, ... , Xk, the scatter plot matrix shows all the pairwise scatter plots of the variables on a single view with multiple scatterplots in a matrix format. For k variables, the scatterplot matrix will contain k rows and k columns. A plot located on the intersection of row and jth column is a plot of variables Xi versus Xj.This means that each row and column is one dimension, and each cell plots a scatter plot of two dimensions.

A generalized scatter plot matrix offers a range of displays of paired combinations of categorical and quantitative variables. A mosaic plot, fluctuation diagram, or faceted bar chart may be used to display two categorical variables. Other plots are used for one categorical and one quantitative variables.

![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a5/Matriz_de_gr%C3%A1ficos_de_dispers%C3%A3o.svg/1320px-Matriz_de_gr%C3%A1ficos_de_dispers%C3%A3o.svg.png
)
## Overview of my approach :

So calculating Simple Linear Regression and visualiing the data can be done in various ways in JavaScript. Some of them includes :
1. [D3.js](https://d3js.org/) 
2. [Plotly.js](https://plotly.com/javascript/)
3. [Chart.js](https://www.chartjs.org/)
4. [Highchart.js](https://www.highcharts.com/blog/products/highcharts/)

Here in this project I used the **Highcharts JS** methodology.

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



