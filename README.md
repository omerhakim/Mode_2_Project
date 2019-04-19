# Mode_2_Project  - What Can Predict Happiness?

# Goal

Using publically available data I tried to examine which variables can predict happiness. I took the Happiness score from "The World Happiness Report 2017" (which is based mainly on people own personal feelings). I collected different data from the world bank, and was able eventually to have a model with a resulting Adjusted R^2 value of .711.

# Procedure
Getting the Data
In downloaded two datasets from kagggle.com: "The World Happiness Report" and World Bank Data regardings the countries of the world. After cleaning the Data I created one pandas dataframe out of them.  I also scraped "Gini Coefficient" table from indexmundi.com.

# Cleaning the Data
The process for cleaning the raw data is covered in the Data Cleaning Jupyter notebook. Entries with missing values were either dropped or replaced manualy with infomation from different sources or with the regional mode/avarage. 

# Exploring and Engineering the Data
Visualization of the data and the choices made for engineering new features can be found in the EDA & Feature Engineering Jupyter notebook. In genaral I tried to distill the variables with lower p value and create model as simple as possible without lowering the Adjusted R^2 significantly/

# Modeling the Data
during the process I found out that predicting Happiness can be very complicated and that some variables cancel others or have different influence in different countries. The final model and the reasoning behind which features were included and excluded can be found in the Modeling Jupyter notebook. I general the main variable which i created was based on log of GDP per Capita. Other variblae which stayed part of the final model where Deathrate,GINI Coefficient and to local dummy variables to specific areas (NEAR_EAST and SUB_SAHARAN_AFRICA)


