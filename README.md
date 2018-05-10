# Food Deserts and Birth Outcomes
#### Final Project for Data Visualization, NYU CUSP, Spring 2018
Prof. Huy Vo

# Group Members:
Dana Chermesh Reshef (dcr346@nyu.edu)
Emily Padvorac (ep2247@nyu.edu)

# Project Discription and Objective
This visualisation is an enhancement of an analysis that had been conducted as a part of Machine Learning for cities class, NYU CUSP Spring 2018. The research identified the important factors impacting low birthweight and preterm births for New York State on the zip code level, using random forests and Bayesian network approaches. This research seeks to understand to what extent living in a food desert may have on birth outcomes. In recent years, the topic of food deserts has become increasingly popular. In short, a food desert is an area that has low-access to healthy, nutritious food.

- _[Full report](https://github.com/danachermesh/Food_Deserts_ML/blob/master/FoodDesertBirthOutcomes_FinalPaper.pdf)_

The deliverable of this DataVis project is an interactive visualization that shows the share of the two negative birth outcomes out of total births for years 2012-2014 in New York State, analysed by zipcodes. The visualization also shows each zipcode's parameters that were found as impactful for predicting birth outcomes.

![byBirth1.png](byBirth1.png) 
_**Fig.1 NYS zipcodes' negative birth outcomes**, interactive map + bar chart + parallel vis of predicting variables; The figure shows mousehover on one of the variables to update the map_

![byBirth2.png](byBirth2.png) 
_**Fig.2 NYS zipcodes' negative birth outcomes**, interactive map + bar chart + parallel vis of predicting variables; The figure shows selections of ranges of variables in the parallel vis, the relevant zipcodes are highlighted_

# Data
_Data that were in used can be found in this GitHub repo under [data folder](https://github.com/danachermesh/Food_Deserts_ML/tree/master/data)_

_Birth Outcome Variables Data_
Two adverse birth outcomes were considered: preterm birth and low birthweight. Data on these outcomes were collected from New York State Department of Health at the zip code level.

_Population Variables Data_
At the beginning of research, a dataset containing variables on food deserts was considered. However, the variables had extremely high multicollinearity. As such, data was gathered on a subset of the variables most relevant to the aim of the research. Data was collected and derived from the **American Community Survey (ACS) 5-year (2009-2016)** at the zip code level. Variables included: 
  - **Citizenship status** 
  - **Poverty rate** 
  - **Health insurance coverage** 
  - **Vehicle Access**
  - **SNAP (Food Stamp) Benefits**
A variable of **teen birth rate** was also considered, and was retrieved from the NYS Department of Health data. Additionally, each zip code was classified as either urban or rural, using classifications as defined by the US Census Bureau.

# How does the visualization help users
Identifying if certain variables are important in determining negative birth outcomes can help decide what policy levers to pull or what demographic groups to focus intervention programs on. These findings are applicable to New York government at both the state and local level, and would be most relevant to the Department of Health. The two visualizations highlight the different relationships between different demographic, social and spatial variables and their impact on negative birth outcomes, make these results and insights accessable to policy makers, as well as for non-professionals.

# Visualization tools used
- D3.js, React
- Python pandas to clean and merge the origional datasets ([link to the Ipython notebook](https://github.com/danachermesh/Food_Deserts_ML/blob/master/FoodDeserts.BirthOutcomes_ML_analysis.ipynb))

# Visualization + Code
The final deliverable is seperated to:

1. Interactive Map + bar chart of Premature Birth and Low Birth Weight % by NYS zipcodes: https://bl.ocks.org/ep2247/raw/1d5e937a9425e80170b81822f43207ea/
2. Parallel Coordinate Chart showing the variables used to predict Premature Birth and Low Birth Weight



