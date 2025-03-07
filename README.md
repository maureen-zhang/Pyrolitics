# Pyrolitics: A Study on Wildfire Impact Prediction with Electric Power Usage
A project by Junhui Shi, Faycal Chaouqui, Marco Lopez, Malik Tuerkoen, Maureen Zhang.

## Overview
Wildfires and power grids are deeply interconnected—fires damage electrical infrastructure, incurring high repair costs and economic losses, while power lines are a major ignition source. In Southern California, where dry conditions, strong winds, and dense vegetation heighten wildfire risks, understanding this relationship is essential.

Government agencies and electricity companies suffer significant financial losses from grid failures, legal liabilities, stock fluctuations, and fire victim compensation funds, yet mitigation efforts remain reactive rather than proactive. A quantified cost-risk assessment can incentivize governments and power companies to adopt a strategic, preventive approach to wildfire mitigation.

This project bridges that gap by leveraging machine learning to analyze wildfire-power grid interactions, predict financial losses, and offer actionable insights to optimize infrastructure and reduce economic damage.

### Approach
By integrating wildfire data, power grid geography, electricity usage, stock prices, fire victim trust funds, and electricity revenue, this project delivers a comprehensive, data-driven approach to wildfire mitigation. By predicting financial losses and infrastructure risks, it empowers governments and electricity companies to minimize economic damage, enhance fire prevention, and optimize power grid resilience. The ultimate goal is to build a sustainable, cost-effective energy infrastructure in Southern California while mitigating the devastating impact of wildfires.

### Results and Implications

### Stakeholders:
- Electricity companies: PG&E
- Smart Grid companies: General Electric, Siemens, etc.
- Governments & NGOs: FEMA, The Red Cross, USDA, IAFF, The Salvation Army, etc.
### KPI(s):
- Internal: Prediction Accuracy (MSE), Recall, Area Coverage(?). external: Burn Probability, Aggregate Fire Damage, Energy Efficiency, MTBF, SAIFI, etc.
### Objectives:
- Identify High-Risk Areas: Use geospatial and environmental data to pinpoint grid alignments that pose higher fire risks.
- Quantify Financial Losses: Assess the economic impact of wildfire-induced power grid failures on infrastructure, company valuation, and fire-related compensation.
- [Maybe not??] Optimize Power Grid Strategy: Guide infrastructure planning and power usage adjustments to minimize future losses and enhance grid resilience.

### Duration: 
2 months [due 4/21].

### Strategies:

## Index (File Map)
This GitHub repository is divided into the following folders. They are described below in the general logical order that you should access them to understand the project.
## Exploratory Data Analysis (This is for the Mar 7 checkpoint)
This folder contains preliminary and exploratory data visualization and analysis of the current dataset we have gathered. 
The analysis includes pairwise comparisons between different datasets to uncover patterns and relationships related 
to wildfires and power grid infrastructure.

### Included Analyses:
- **Electricity Usage and Wildfire Incidents**  
  Examining the correlation between power consumption and fire occurrences.  

- **Geospatial Analysis of Fire and Power Grid**  
  Mapping the locations of wildfires relative to power grid infrastructure.  

- **Geospatial Analysis of Fire Intensity**  
  Identifying high-risk zones based on wildfire severity.  

- **Vegetation and Fire Risk**  
  Investigating how vegetation density influences wildfire spread and ignition near power lines.  

- **Economic Impact of Disasters**  
  Assessing the financial consequences of wildfires, including infrastructure damage and disaster response costs.  

These analyses serve as the foundation for further machine learning modeling and risk assessment in this project.


### Raw Data

### Cleaned Data

### Papers

### Models

### Maps and Data Visualization

## Conclusion



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
