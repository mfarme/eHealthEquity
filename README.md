# eHealthEquity
## Active Research
Research Notebooks, Data Sources, and outputs of eHealthEquity research.

*Dissertation Research of Matthew Farmer PhD, RN
 University of Missouri, Sinclair School of Nursing* [@mfarme](https://github.com/mfarme/mfarme)

## Aim
Assess and analyze quantifiable evidence that Internet access and adoption is a social determinant of health in United States counties and describe the interaction effects between other social determinants.
- Why publish on Github? To promote replication with different or new data, grow research in this domain, and do science in the open. [Reference: Coducting Replication and Repoduction in Science](https://esajournals.onlinelibrary.wiley.com/doi/full/10.1002/bes2.1801) 


### Research Question 1 
- What is the relationship between Internet adoption and self-reported diabetes prevalence in United States counties, controlling for other social determinants of health?
### Research Question 2
- Do machine learning algorithms produce a better fit (lower variance and bias) compared to linear regression models? 

---
### Libraries Used
* [Pandas](https://pandas.pydata.org/)
* [Numpy](https://numpy.org/)
* [cenususdis](https://github.com/vengroff/censusdis/tree/main)
* [sodapy](https://github.com/xmunoz/sodapy)
* [scipy](https://www.scipy.org/)
* [matplotlib](https://matplotlib.org/)
* [seaborn](https://seaborn.pydata.org/)
* [geopandas](https://geopandas.org/)
* [shapely](https://shapely.readthedocs.io/en/stable/)
* [SciPy](https://www.scipy.org/)
* [scikit-learn](https://scikit-learn.org/stable/)
* [statsmodels](https://www.statsmodels.org/stable/index.html)
* [plotly](https://plotly.com/python/)
* [os](https://docs.python.org/3/library/os.html)
* [json](https://docs.python.org/3/library/json.html)
* [urllib](https://docs.python.org/3/library/urllib.html)



## Data Sources and Variables
| Variables  | Level        | Concept                                       | Measure                                                                                       | Source               | Note                                                                        |
|------------|--------------|-----------------------------------------------|------------------------------------------------------------------------------------------------|----------------------|-----------------------------------------------------------------------------|
| RQ1 DV     | Outcome      | Diabetes Prevalence                           | Diagnosed diabetes among adults aged >=18 years; % of county                                   | BRFSS/PLACES 2021    | Upper and Lower confidence; crude and age-adjusted                          |
| IV         | Intermediary | Behaviors and Biological Factors: Internet Adoption| Households with internet (Broadband) subscription; %                                    | ACS 5Y 2021          | proportion and raw count with margin of error                               |
| Covariates | Structural   | Gender, Age, Ethnicity                        | Aged 65 & Older, Gender, Race, Ethnicity                                                      | ACS 5Y 2021          | proportion and raw count with margin of error                               |
| Covariates | Structural   | Education, Occupation, Income                 | Educational attainment, Industry employed, employment status, income in past 12 months below poverty level | ACS 5Y 2021          | proportion and raw count with margin of error                               |
| Covariates | Intermediary | Material Circumstances                        | Transportation, Housing type, Health insurance coverage                                       | ACS 5Y 2021; BRFSS 2021 (insurance)| proportion and raw count with margin of error                  |
| Covariates | Intermediary | Behaviors and Biological Factors              | Obesity, smoking status, visit to doctor in past year (adults)                                | BRFSS/PLACES 2021    | Upper and Lower confidence; crude and age-adjusted                          |
| Covariates | Intermediary | Psychological Factors                         | Depression among adults, Mental health “not good” for >= 14 days among adults                  | BRFSS/PLACES 2021    | Upper and Lower confidence; crude and age-adjusted                          |
---

## Data Sources

* [American Community Survey (ACS)](https://www.census.gov/programs-surveys/acs)
    * [ACS 5-Year Data Profiles](https://www.census.gov/data/data-tools.html)
    * [ACS 5-Year Data Profiles API](https://www.census.gov/data/developers/data-sets/acs-5year.html)
* [BRFSS/PLACES](https://www.cdc.gov/brfss/brfssprevalence/index.html)
    * [BRFSS/PLACES API](https://dev.socrata.com/foundry/data.cdc.gov/4qvr-3h4f)
* [NTIA](https://www.ntia.gov/data/broadband-data)
* [RUCA Codes](https://www.ers.usda.gov/data-products/rural-urban-commuting-area-codes.aspx)

## Conceptual Framework
* [WHO Social Determinants of Health Framework](https://www.who.int/teams/social-determinants-of-health)
