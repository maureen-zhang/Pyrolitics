# Pyrolitics: A Study on Wildfire Impact Prediction with Electric Power Usage
A project by Junhui Shi, Faycal Chaouqui, Marco Lopez, Malik Tuerkoen, Maureen Zhang.

## Overview
Wildfires and power grids are deeply interconnected—fires damage electrical infrastructure, incurring high repair costs and economic losses, while power lines are a major ignition source. In Southern California, where dry conditions, strong winds, and dense vegetation heighten wildfire risks, understanding this relationship is essential.

Government agencies and electricity companies suffer significant financial losses from grid failures, legal liabilities, stock fluctuations, and fire victim compensation funds, yet mitigation efforts remain reactive rather than proactive. A quantified cost-risk assessment can incentivize governments and power companies to adopt a strategic, preventive approach to wildfire mitigation.

This project bridges that gap by leveraging machine learning to analyze wildfire-power grid interactions, and offer actionable insights to optimize infrastructure and reduce economic damage.

### Approach
By integrating wildfire records, weather conditions, vegetation indices, power grid geography, and electricity consumption data, this project delivers a comprehensive, data-driven framework for wildfire prediction. Through strategic feature engineering and careful evaluation, we aim to enhance fire prevention and mitigation efforts.

### Results and Implications
- Using a simple model like panel regression, we gain clearer insight into how the structure of the data frame and the selection of features influence the model's performance and reliability.
- There is a significant correlation between product of eletricity comsumption and vegetaion changes and the number of fires in a given county in a given year.
- The frequency of fires appears to correlate more strongly with electricity consumption than with the magnitude or severity of individual fire events.

### Stakeholders:
- Electricity companies: PG&E
- Smart Grid companies: General Electric, Siemens, etc.
- Governments & NGOs: FEMA, The Red Cross, USDA, IAFF, The Salvation Army, etc.
### KPI(s):
- Internal: Prediction Accuracy (MSE), Recall, Area Coverage(?). external: Burn Probability, Aggregate Fire Damage, Energy Efficiency, MTBF, SAIFI, etc.
### Objectives:
- Construct a model‑ready data frame with clean, well‑curated features.
- Insights into apporpriet model for predicting fire.
- Using Machine learning model ro investigate the relation between fire  

### Duration: 
2 months [due 4/21].

### Strategies:
- We applied feature engineering by multiplying time-invariant features with time-dependent variables. These interaction terms captured dynamic relationships more effectively, and several emerged as strong predictors in the regression model.
- We categorized key variables to better represent non-linear effects and support interpretable analysis.
- We merged diverse datasets—including vegetation indices, weather data, and electricity usage—to create a unified, model-ready panel data.
- We leveraged the panel data structure to simultaneously capture both spatial and temporal patterns, enhancing the model's ability to reflect localized and time-varying risk factors.



  
## Index (File Map)
This GitHub repository is divided into the following folders. They are described below in the general logical order that you should access them to understand the project.

### Included Analyses:
- **Electricity Usage and Wildfire Incidents**  
  Examining the correlation between power consumption and fire occurrences.  

- **Geospatial Analysis of Fire and Power Grid**  
  Mapping the locations of wildfires relative to power grid infrastructure.  

- **Geospatial Analysis of Fire Intensity**  
  Identifying high-risk zones based on wildfire severity.  

- **Vegetation and Fire Risk**  
  Investigating how vegetation density influences wildfire spread and ignition near power lines.  

- **Weather Data**  
  Assessing the financial consequences of wildfires, including infrastructure damage and disaster response costs.  

These analyses serve as the foundation for further machine learning modeling and risk assessment in this project.


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
