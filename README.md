# UMBC DATA SCIENCE Capstone Project<br /> Chaojie Wang


**Author** : Sushanth Kumar Panasa<br />**Semester**: Spring'23<br />**Campus ID**: YY72411

# Introduction:
The agriculture industry is under extreme strain to supply the increased demand for food as a result of the population's exponential growth. Food shortages and issues with food security are more likely to occur as the population grows. Incorporating population data into our study can help us comprehend the scope of the problem and create solutions to lessen its effects.

We can identify areas with rapid urbanization and population growth using population statistics. We can predict the future rise in food demand in these areas by looking at demographic patterns. With the use of this knowledge, we are able to organize and maximize agricultural resource allocation, distribution, and production in order to fulfill rising population demands for food in the future.

We can investigate the social and economic aspects that affect farming practices by using demographic statistics. Designing tailored interventions to support farmers, boost agricultural output, and encourage sustainable livelihoods in rural regions requires an understanding of the demographic makeup, income levels, and educational levels of the community.

Overall, using population data in our research gives us the ability to handle any possible issues brought on by both a growing population and a lack of food. We can optimize agricultural productivity, improve food security, and assure a sustainable future for future generations by making data-driven decisions based on a thorough understanding of population dynamics, consumer preferences, and socio-economic considerations.

# Objective:

In this project, we will be extracting the numerous insights and its effects on an crop and livestock  data with respect to population and will be discovering the algorithms which can accurately analyse and the understand the data.

Develop predictive models to forecast crop yields and livestock production based on various factors such as weather conditions, soil quality, and farming practices. By accurately predicting output, farmers can make informed decisions regarding planting schedules, resource allocation, and risk management.

# Data Collection:

There are 2 data sets we will be working in this Project, this data sets with combined size of 300.2 are acquired from the Food and Agriculture Organization of the United Nations (FAO) and Department of Economic and Social Affairs, Population Division.

- Fist dataset is from FAO which records crop and livestock statistics for 278 products in various categories, including primary and processed crops, live animals, and primary and processed livestock.
  - https://www.fao.org/faostat/en/#data/QCL
- The second data set is the population data from UN which is the empirical data which show revised estimates of various demographic components (population, mortality, migration) for different countries or regions for the period of 1950-2021.
  - https://population.un.org/wpp/Download/Archive/CSV/

# Data Discription:

After combining 2 datasets and removing the uncessary columns we get the dataset as shown below:

![image](https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/bd6a3818-1d99-4be2-8d3a-0b83b7728323)

The scheam of the dataset is as follows:

![image](https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/8df9b11c-e570-4181-a6a9-d86a5ee8e9fc)

The discriptions of all the features are as follows:

- ID: This column represents the unique identifier for each record in the dataset. It serves as a primary key to distinguish one data entry from another.
- Area: This column refers to the geographical area or location associated with the data entry. It could represent a country, region, state, or any other defined area of interest.
- Item: This column describes the specific crop or livestock item that the data pertains to. It could include various agricultural products such as wheat, corn, rice, cattle, poultry, etc.
- Element: This column specifies the element or attribute of the crop or livestock being measured. It could include parameters like production, yield, consumption, export, import, population, etc.
- Year: This column indicates the year or time period to which the data corresponds. It helps in analyzing trends and changes in crop/livestock-related factors over time.
- Unit: This column represents the unit of measurement for the corresponding value. It provides information on how the data values are quantified, such as kilograms, tons, hectares, liters, etc.
- Variant: This column specifies the variant or subcategory of the element being measured. It may include different subtypes or classifications within the element, allowing for more detailed analysis and comparisons.
- Value: This column contains the numeric value associated with the specific element for a given year and area. It represents the measured quantity or attribute for the crop/livestock item.
- Flag: This column provides additional information or flags related to the data entry. It may indicate any data quality issues, special conditions, or relevant annotations associated with the value.
- PopMale: This column represents the population count of males in the specified area and year. It provides demographic information related to the male population.
- PopFemale: This column represents the population count of females in the specified area and year. It provides demographic information related to the female population.
- PopTotal: This column represents the total population count in the specified area and year, combining both males and females. It provides an overall view of the population size.
- PopDensity: This column calculates the population density for the specified area and year. It represents the number of individuals per unit of land area, such as people per square kilometer or square mile. Population density helps to assess the level of population concentration in a given area.

# Insights:

We gained numerious insights from this dataset. It varies from population density vs Meat production over the years to Average rice production and Yeild from differnt continents.

### Insight 1:

This graph represents top countries where Yoghurt production per person is highest.

<img width="613" alt="image" src="https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/cfdf5600-64dd-41b1-a4b7-3d7347d3d460">

As you can see small countries with low population density is highest like Belarus.

### Insight 2:

This Graph represents the meat production of countries with respect to Population density over the years.

<img width="603" alt="image" src="https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/9c37cd08-b0fe-4a5b-944a-e8975050a9fd">

We can see an increase of both production and population density in between 1990 and 2000.

### Insight 3:

This Graph represents the quantity of beef produced by each country from the years 2010 to 2021.

<img width="613" alt="image" src="https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/2f5d5bd7-f9dd-48cd-9d83-fa4099b8e693">

We can see a unique case of Brazil, which even with less population is producing as much beef or more so than USA  and China.

### Insight 4:

This Graph represents the area used for Crops and Livestock production over the years from different continents.

<img width="575" alt="image" src="https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/ec840abd-3cbc-48b6-8f6a-f5ebae2b195b">

We can see a sudden increase in area usage 1990’s and the unique case of Europe where area has decreased over years.

### Insight 5:

These Graphs represents the area, Production and Yield produced by each continent.

<img width="321" alt="image" src="https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/ae855bd1-bb4e-4858-b8bc-bdabbb29ad47">

<img width="323" alt="image" src="https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/2de0ca93-0345-4c82-8b45-375cedd634b2">

<img width="318" alt="image" src="https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/69320083-5ff4-490a-9c97-4eb6be9d5c14">

We can see that Asia has high quantity of Rice cultivation, but the yield is not high as even Europe.

### Insight 6:

These graphs represents highest and lowest countries with livestock animals per person ratio.

<img width="329" alt="image" src="https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/1f1a5109-253c-40b2-822f-3506d3d0a790">

<img width="316" alt="image" src="https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/505825e3-72c3-4273-b6a9-c816b315908a">

As we can see a unique case of Japan which is not city state such as Singapore and Hong Kong is in the list of countries with lowest ratio.

# Exploratory data analysis:

Discription of the data is as follows:

![image](https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/f56ff1d7-3d6c-426e-bae7-764eabfa6180)

Correlation matrix of the data is as follows:

<img width="555" alt="image" src="https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/b2faf728-7cf0-42eb-9eaa-9cdc39a70fe5">

Boxplot of all the values in the dataset:

![image](https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/69fccb3e-4fdf-4a93-8902-89ff3262bbf1)


# Finding and Removing Outliers:

We get all the outliers of the contionous features in the dataset. Some of the outliers are as follows:

![image](https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/c651d40c-1f24-401c-bab6-8f2d1a6b3c71)

The number of outliers removed are as follows:

![image](https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/81a2cc7d-278d-4ea9-bc82-3500965ccc9f)


# Machine Learning Framework:

The ML opeation done on the dataset till now are as below:

- Merging Data: This step involves combining different datasets or sources of data that are relevant to the project. It could include merging crop data, livestock data, and population data based on common identifiers such as area, year, or other relevant columns. Merging the data allows for a comprehensive analysis that considers multiple factors simultaneously.
- Basic Cleaning: In this step, the dataset is cleaned to ensure data quality and consistency. It involves handling missing values, removing duplicate entries, and addressing any inconsistencies or errors in the data. Cleaning the data helps to ensure accurate and reliable analysis.
- Encoding: Encoding involves converting categorical variables into numerical representations to make them suitable for analysis. It may include techniques such as one-hot encoding or label encoding, depending on the nature of the categorical data. Encoding allows for the inclusion of categorical variables in ML models.
- Exploratory Data Analysis (EDA): EDA is a critical step in understanding the dataset and exploring relationships between variables. It involves statistical analysis, visualization, and summary statistics to identify patterns, trends, and correlations within the data. EDA helps in uncovering insights and formulating hypotheses for further analysis.
- Finding Outliers: Outliers are data points that significantly deviate from the overall pattern of the dataset. Finding and analyzing outliers helps in understanding anomalies in the data and their potential impact on the analysis. Outliers can be identified using statistical techniques or visualization methods.
- Removing Outliers: Once outliers are identified, they can be removed from the dataset if deemed necessary. Removing outliers helps in improving the accuracy and reliability of subsequent analyses and model building.

The overall ML frame work of the project is as follows:

<img width="1060" alt="Screenshot 2023-05-14 at 5 29 37 PM" src="https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/f4e41758-0ecf-4abd-ad78-cb7f78571b50">


## Case 1: Continent (Discrete Data):

- Preparing Data: This step involves preparing the data by performing tasks such as handling missing values, encoding categorical variables (if any), and scaling or normalizing numerical features. The goal is to ensure the data is in a suitable format for analysis.
- Feature Selection: In this step, relevant features are selected from the dataset that are most informative for predicting the target variable. Techniques such as statistical tests, correlation analysis, or domain knowledge can be used to identify the most significant features.
- Splitting Data: The dataset is divided into training and testing datasets. The training dataset is used to train the machine learning models, while the testing dataset is used to evaluate the performance of the models.
- Model Building:
  - Logistic Regression: Logistic Regression is a classification algorithm used to predict categorical outcomes based on input features. It models the relationship between the independent variables and the probability of a specific outcome.
  - K-Neighbors Classifier: The K-Neighbors Classifier algorithm classifies data points based on their similarity to other data points in the training dataset. It assigns the most common class label among the k-nearest neighbors.
  - Decision Tree Classifier: The Decision Tree Classifier algorithm creates a tree-like model of decisions and their possible consequences. It splits the data based on different feature values to build a predictive model.
- Handling Imbalances (SMOTE): Imbalanced datasets occur when one class is significantly more prevalent than the other(s). In this step, SMOTE (Synthetic Minority Oversampling Technique) can be used to address the imbalance by generating synthetic examples of the minority class to balance the dataset.
- Best Model based on Accuracy: The models built in the previous steps are evaluated based on their accuracy on the testing dataset. The model with the highest accuracy is selected as the best model for predicting the continent variable.


## Case 2: Area (Continuous Data):

- Preparing Data: This step involves preparing the data by performing tasks such as handling missing values, scaling or normalizing the continuous features, and encoding categorical variables (if any). The goal is to ensure the data is in a suitable format for analysis.
- Feature Selection: In this step, you identify and select the most relevant features from the dataset. This can be done using techniques like correlation analysis, feature importance, or dimensionality reduction methods.
- Splitting Data: The dataset is split into training and testing subsets. The training set is used to train the models, while the testing set is used to evaluate their performance
- Model Selection:
  - Decision Tree Classifier: This algorithm creates a decision tree based on the training data, where each node represents a feature and each branch represents a decision rule. It is suitable for classification tasks.
  - Random Forest Regression: This algorithm creates an ensemble of decision trees and makes predictions by aggregating the results of individual trees. It is suitable for regression tasks.
- Best Model based on Accuracy: The performance of each model is evaluated based on accuracy, which measures the percentage of correctly predicted instances. The model with the highest accuracy is selected as the best model for predicting the target variable.


# Prediction Modelling:
## Case 1: Predicting best Continent:

#### Before SMOTE:

![image](https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/9ebea4ea-34bc-485e-969b-b01936be416a)

![image](https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/0489e68e-56df-46f6-a8bc-28ef073446dd)

![image](https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/7d8a45cd-3010-4fb3-81a3-1851c3c75e69)

In this case we see that K-Neighbors Classifier has best outcomes. As we can see from the confusion matrix that atlest 50% percent of the prediction are correct (Blue in diagonal Values).


#### After SMOTE:

![image](https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/40936ce3-06a1-4369-903a-610177a22a5a)

![image](https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/50b77393-2ef2-4681-b71d-c5720619507e)

![image](https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/9584a163-7bc2-467a-8cb4-d7319a3d4f99)

In this case we see that K-Neighbors Classifier has best outcomes after performing SMOTE on data. As we can see from the confusion matrix that atlest 65% percent of the prediction are correct (Blue in diagonal Values) and almost none of the other values has atlest 10% correct predictions.


# Prediction Modelling:
## Case 2: Predicting the necesary Area:

![image](https://github.com/sushanth23k/Sushanth_Farmdata_analysis/assets/40069679/6ac64ee6-e628-4594-bbbb-4ea0615c8e6d)

We can say that Random Forest Regression is the best Model for this case.

# Conclusion:

The farm_livestock_population project aimed to analyze and draw insights from the provided dataset, focusing on various aspects of agriculture, livestock, and population data. Additionally, predictive modeling was performed to forecast outcomes based on the available features.

The analysis revealed interesting insights into different areas of the agricultural landscape. For instance, the examination of yogurt production per person highlighted the top countries where yogurt production is highest, showcasing the efficiency of smaller countries with lower population density in this particular aspect.

Furthermore, the analysis of beef production by country unveiled unique cases such as Brazil, which demonstrated high beef production despite having a smaller population compared to countries like the USA and China. This emphasizes Brazil's efficiency and productivity in the beef industry.

In addition to the insights gained from the exploratory analysis, predictive modeling was performed to forecast outcomes based on the available features. The models, including logistic regression, K-Neighbors Classifier, and decision tree classifiers, provided valuable predictions for continent classification and necessary area estimation. The best-performing models were selected based on accuracy metrics, demonstrating the potential for accurate predictions using the dataset.

Overall, the analysis and predictive modeling performed in this project contribute to a comprehensive understanding of the farm-livestock-population dynamics. The insights obtained can inform decision-making processes in the agricultural sector, facilitating sustainable practices, resource allocation, and food security measures.











