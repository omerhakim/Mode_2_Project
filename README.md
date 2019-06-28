# World-Happiness-Report - Can Predict Happiness be Predicted?  

# Goal

Using publicly available data, I tried to examine which variables can predict happiness. I took the Happiness score from "The World Happiness Report 2017" (which is based mainly on people own personal responses). I collected different data from the world bank sources, and was able eventually to have a model with a resulting Adjusted R^2 value of .711.

# Procedure
Getting the Data
I downloaded two data-sets from kaggle.com: "The World Happiness Report" and World Bank Data regarding the countries of the world. After cleaning the Data I created one merged pandas data frame out of them.  I also scraped "GINI Coefficient" table from indexmundi.com.

<img src = "./images/image1.png" style = max width = 60%>

# Cleaning the Data
The process for cleaning the raw data is covered in the Data Cleaning Jupyter notebook. Entries with missing values were either dropped or replaced manually with information from different sources or with the regional mode/average. 

<img src = "./images/image2.png">


# Exploring and Engineering the Data
Visualization of the data and the choices made for engineering new features can be found in the  Jupyter notebook. In general I tried to distill the variables with lower p value and create model as simple as possible without lowering the Adjusted R^2 significantly.

<img src = "./images/image3.png">

A

<img src = "./images/image4.png">


A


<img src = "./images/image5.png">

A

<img src = "./images/image6.png">

A

<img src = "./images/image7.png">

## Feature Ingineering

<img src = "./images/image8.png">

A


<img src = "./images/image9.png">


A

<img src = "./images/image10.png">

A

<img src = "./images/image11.png">

# Modeling the Data

<img src = "./images/image12.png">

A

<img src = "./images/image13.png">

during the process I found out that predicting Happiness can be very complicated and that some variables cancel others or have different influence in different countries. The final model and the reasoning behind which features were included and excluded can be found in the Jupyter notebook. In general, the main variable which I created was based on log of GDP per Capita. Other variable which stayed part of the final model where Death-rate,GINI Coefficient and to local dummy variables to specific areas (NEAR_EAST and SUB_SAHARAN_AFRICA)

<img src = "./images/image14.png">

A

<img src = "./images/image15.png">

A



![Image of model](images/Screenshot%20(58).png)

<img src = "./images/image17.png">
<img src = "./images/image18.png">
<img src = "./images/image19.png" style = max width = 50%>
<img src = "./images/image20.png" style = max width = 50%>





