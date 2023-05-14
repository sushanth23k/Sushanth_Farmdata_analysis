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

# Merged Dataset based on Country:

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









