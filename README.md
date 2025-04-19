# Pyrolitics: A Study on Wildfire Impact Prediction with Electric Power Usage
A project by Junhui Shi, Faycal Chaouqui, Marco Lopez, Malik Tuerkoen, Maureen Zhang.

## Overview
Wildfires and power grids are deeply interconnected—fires damage electrical infrastructure, incurring high repair costs and economic losses, while power lines are a major ignition source. In California, where dry conditions, strong winds, and dense vegetation heighten wildfire risks, understanding this relationship is essential.

Residents, government agencies and electricity companies suffer significant financial losses from wild fires in California, yet mitigation efforts remain reactive rather than proactive. A quantified cost-risk assessment can incentivize governments and power companies to adopt a strategic, preventive approach to wildfire mitigation.

This project bridges that gap by leveraging machine learning to analyze wildfire-power grid interactions, and offer actionable insights to optimize infrastructure and reduce economic damage.

### Approach
By integrating wildfire records, weather conditions, vegetation indices, power grid geography, and electricity consumption data, this project delivers a comprehensive, data-driven framework for wildfire prediction. Through strategic feature engineering and careful evaluation, we aim to enhance fire prevention and mitigation efforts.

### Results and Implications

- As part of our initial exploratory analysis, we plotted a map of transmission lines and wildfire locations in California, showing overlapping of transmission lines and wildfires:
  <p align="center">
    <img src="Maps%20and%20Data%20Visualization/transmission_wildfire2011.png" alt="Wildfire Risk Map" width="45%">
  </p>
- We found a significant correlation between the **product of electricity consumption and vegetation change** and the number of fires in a given county per year.
- Fire frequency correlates more strongly with **electricity usage** than with the **magnitude or severity** of individual fire events.

### Stakeholders:
- Electricity companies: PG&E
- Smart Grid companies: General Electric, Siemens, etc.
- Governments & NGOs: FEMA, The Red Cross, USDA, IAFF, The Salvation Army, etc.

### Objectives:
- Construct a model-ready data frame with clean, well-curated features.
- Gain insights into appropriate modeling approaches for predicting wildfire occurrence and frequency.
- Understand how data structure and feature design impact model performance by evaluating various machine learning algorithms.

### Duration: 
2 months [due 4/21].

### Strategies:
- Through cleaning and processing, we have obtained a panel datase.
- We categorized key variables to better represent non-linear effects and support interpretable analysis.
- We enhanced feature variability by multiplying time-invariant features with time-dependent variables. These interaction terms captured dynamic relationships more effectively, with several emerging as strong predictors in the regression model.
- We merged diverse datasets—including vegetation indices, weather data, and electricity comsumption, and wildfire records to create a unified, model-ready panel data containing strategically engineered features ranging from year 1992 to year 2020.
- We leveraged the panel data structure to simultaneously capture both spatial and temporal patterns, enhancing the model’s ability to reflect localized and time-varying risk factors. This was supported by libraries such as GeoPandas, OSMnx, and statsmodels (for OLS regression), and involved handling geospatial formats like shapefiles and GeoJSON, as well as performing spatial joins, distance calculations, and infrastructure mapping.
- Using a simple model like panel regression, we gain clearer insight into how the structure of the data frame and the selection of features influence the model's performance and reliability.

  
## Index (File Map)

This GitHub repository is organized into the following key files, listed in the general order recommended for understanding the project:

- `get_data.ipynb`  
  Downloads all necessary datasets from a shared Google Drive folder and prepares them for analysis.

- `Pyrolitics.ipynb`  
  Contains exploratory analysis, feature engineering, and initial statistical modeling. These analyses lay the groundwork for subsequent machine learning and wildfire risk assessment.

## Conclusion
In this project we introduced panal data strucnture
leveraging the county and time series nature the data, we use
Through our effort, we have enhanced the 


## References
- Sayarshad, H. R. (2023). *Preignition risk mitigation model for analysis of wildfires caused by electrical power conductors.*  
*International Journal of Electrical Power & Energy Systems, 153*, 109353.  
DOI: [10.1016/j.ijepes.2023.109353](https://doi.org/10.1016/j.ijepes.2023.109353) 

- Warner, C., Callaway, D., & Fowlie, M. (2024). *Risk-Cost Tradeoffs in Power Sector Wildfire Prevention.*  
  *Energy Institute at Haas: Berkeley, CA, USA.*  
  [Full Text](https://www.haas.berkeley.edu/wp-content/uploads/WP347.pdf)  

- Sohrabi, B., Arabnya, A., Thompson, M. P., & Khodaei, A. (2024). *A Wildfire Progression Simulation and Risk-Rating Methodology for Power Grid Infrastructure.*  
  *IEEE Access, 12*, 112144-112156.  
  DOI: [10.1109/ACCESS.2024.3439724](https://doi.org/10.1109/ACCESS.2024.3439724)

- Pollack, M., Piansky, R., Gupta, S., Kody, A., & Molzahn, D. (2024). *Equitably allocating wildfire resilience investments for power grids: The curse of aggregation and vulnerability indices.*  
  *arXiv preprint*, arXiv:2404.11520.  
  [Full Text](https://arxiv.org/abs/2404.11520)

## Data Sources

The project utilizes data from the following sources:
*   Wildfire data from [Kaggle](https://www.kaggle.com/datasets/rtatman/188-million-us-wildfires/data)
*   Transmission line data from the [CA  Energy Comission](https://cecgis-caenergy.opendata.arcgis.com/datasets/CAEnergy::california-electric-transmission-lines-1/about)
*   Weather data from [NOAA' National Centers for Environmental Information.](https://www.ncei.noaa.gov/)
*   Electricity consumption data from [California Electricity Consumption Database
](https://catalog.data.gov/dataset/california-electricity-consumption-database-e26e9)
*   Vegetation data from the [California Department of Fish and Wildlife.](https://wildlife.ca.gov/Data/GIS/Vegetation-Data)
*  County data was obtained from [data.gov.](https://catalog.data.gov/dataset/counties2)
