# [PLACES/BRFSS Data](https://www.cdc.gov/places/methodology/index.html)
The 36 measures include 13 health outcomes, 9 prevention practices, 4 health risk behaviors, 7 disability measures (new for the 2023 release), and 3 health status measures.
The measures include major risk behaviors that lead to illness, suffering, and early death related to chronic diseases and conditions, as well as the conditions and diseases that are the most common, costly, and preventable of all health problems.
Each measure has a comprehensive definition that includes the background, significance, limitations of the indicator, data source, and limitations of the data resources.
Measures complement existing sets of surveillance indicators that report state, metropolitan area, and county data, including County Health Rankings and Chronic Disease Indicators.
The 95% confidence intervals (CIs) of modelled estimates are generated using a Monte Carlo simulation.

Estimates were provided by the Centers for Disease Control and Prevention (CDC), Division of Population Health, Epidemiology and Surveillance Branch. PLACES was funded by the Robert Wood Johnson Foundation in conjunction with the CDC Foundation. This dataset includes estimates for 36 measures: 13 for health outcomes, 9 for preventive services use, 4 for chronic disease-related health risk behaviors, 7 for disabilities, and 3 for health status. These estimates can be used to identify emerging health problems and to help develop and carry out effective, targeted public health prevention activities. Because the small area model cannot detect effects due to local interventions, users are cautioned against using these estimates for program or policy evaluations. Data sources used to generate these model-based estimates are Behavioral Risk Factor Surveillance System (BRFSS) 2021 or 2020 data, Census Bureau 2021 or 2020 county population estimate data, and American Community Survey 2017–2021, or 2016–2020 estimates. The 2023 release uses 2021 BRFSS data for 29 measures and 2020 BRFSS data for 7 measures (all teeth lost, dental visits, mammograms, cervical cancer screening, colorectal cancer screening, core preventive services among older adults, and sleeping less than 7 hours) that the survey collects data on every other year. More information about the methodology can be found at www.cdc.gov/places.

[API Docs](https://dev.socrata.com/foundry/data.cdc.gov/swc5-untb)

## [ACS 2021 5-year](https://www.census.gov/data/developers/data-sets/acs-5year.html)

The American Community Survey (ACS) is an ongoing survey that provides data every year -- giving communities the current information they need to plan investments and services. Information from the survey generates data that help determine how more than $675 billion in federal and state funds are distributed each year.

Raw data estimates and percentages for each variable, for each tract, are included in the database. In addition, 
the margins of error (MOEs) for each estimate, at the Census Bureau standard of 90%, are also included. 
Confidence intervals can be calculated by subtracting the MOE from the estimate (lower limit) and adding the 
MOE to the estimate (upper limit). Because of relatively small sample sizes, some of the MOEs are high. It is 
important to identify the amount of error acceptable in any analysis.

[Calculate MOE - Youtube] (https://www.youtube.com/watch?v=nM2RZJag320)

[API Docs](https://www.census.gov/data/developers/data-sets/acs-5year.html)

## [National Broadband Map, FCC, API](https://us-fcc.app.box.com/v/bdc-public-data-api-spec)

Before you can use the API, you need to generate an API access token. This is done by logging into the National Broadband Map (NBM) application with your FCC User Registration credentials and navigating to the “Manage API Access” option. From there, you can generate a token which will be used for authenticating your API requests.

Use the 'View List of Availability Data Downloads' API Endpoint: Once you have the token, you can use the API to extract the broadband data. For data related to 2021, you will use the 'View List of Availability Data Downloads' endpoint. This endpoint's method is GET, and its path is /api/public/map/downloads/listAvailabilityData/{as_of_date}. The {as_of_date} in the path needs to be replaced with the specific date you're interested in, formatted as 'YYYY-MM-DD'. The document does not specify how to find the exact dates available, but typically, an API provides an endpoint or documentation listing the available dates.

Download the Data: After getting the list of available files for your specified date, you can download them using the 'Download File' endpoint. The method for this endpoint is also GET, and its path is /api/public/map/downloads/downloadFile/{data_type}/{file_id}/{file_type}. You will need to specify the data_type (e.g., 'availability'), file_id (which you get from the list of available data downloads), and file_type (e.g., 'csv' or 'gis').

[FCC Broadband Map Data Details](https://us-fcc.app.box.com/v/bdc-data-downloads-output)

Broadband Summary by Geography Type: This file contains summary information about the fixed and mobile broadband data submitted
across all biannual submissions for a geography type in Comma Separated Value (CSV) format.
Variable of interest: t1_2_3_7_s3_r: This variable represents the calculated percentage of units for broadband serviceable locations with residential fixed broadband service using Copper, Cable, Fiber to the Premises, or Licensed Fixed Wireless technology at speeds of at least 25 / 3 Mbps