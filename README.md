# Data Gathering & Warehousing 
## DSSA-5102 - Spring 2025
_Data Science and Strategic Analytics Graduate Program_ - [Stockton University]

### Languages & Environment:
- Python, SQL, Anaconda Navigator, Jupyter Notebook, Github, Spyder


The data for this project  was collected by the National Center for Immunization and Respiratory Diseases (NCIRD) and they own the dataset. Data was collected from the Pregnancy Risk Assessment Monitoring System (PRAMS) which is used at the state level for women who experienced a recent live birth. It was extracted from the **CDC** website as a CSV file and imported into a Jupyter notebook. 

Jupyter notebook and Python were used to clean the data and take all the necessary steps to remove dirty data. Most of the data contained in the file was clean, however a few steps were taken. All the column names were made lowercase, and all special characters were removed and replaced with an underscore sign to make it SQL friendly. One of the column was renamed completely to accurately represent the data- ‘survey_year_influenza_season’ to simply ‘year’. The column of dimensions which contained age and race and ethnicity was separated to include age in one column and race and ethnicity in another. All the columns were converted into Numpy arrays to increase accessibility for other libraries. The units for the vaccine column are types of vaccines which is similar for the category column of geography type as state or nation. Next, the geography column is names of US states, year is numerical value of perspective year. Estimate and 95% CI columns are another numerical percentage representing the estimated vaccine coverage and confidence interval, respectively. Sample size is the last column containing numbers portraying the sample size. 

Most of the columns remained the same but to split the dimension column an if and else loop was used to separate the contents. Data was validated to ensure consistency. It was checked both manually and through Python through various ways such as checking for missing or incomplete values, looking for all the unique values in each column for outliers and anomalies. The NCIRD also collects the data through state records ensuring validity and consistency of data. 

The columns in the dataset are as follows: 
**Vaccine**- The name of the vaccine (Tdap or Influenza) that women received is listed.  
**Geography Type**- Specifies whether the location is a US state or nationwide statistic. 
**Geography**- Lists the specific state or USA that the statistics represent. 
**Year**- Specifies the year the data was collected in for the specific state or nationwide. 
**Dimension type**- Specifies if the age or race and ethnicity is listed  
**Dimension**- includes the actual age or race and ethnicity of the women that are included in this dataset.
**Estimate (%)**- Lists the estimated women who got vaccinated for the specific vaccine within a certain age group or race and ethnicity. 
**95% CI** Lists the confidence interval range for the estimated vaccine coverage for the specific age or ethnicity. 
**Sample Size**- States the sample of women who were included. 

There is no strict regulation to use the data. It is  available publicly for use for anyone presented by the CDC. CDC has many datasets that are available for the public. The website used to gather the data and other information are listed below- 
Vaccination Coverage among Pregnant Women | Data | Centers for Disease Control and Prevention
Vaccination Coverage among Pregnant Women | HealthData.gov



### Assignments:
- *Assignment #1* - Locating a Dataset
    - Importing data and initial dataset exploration (Master dataset not available on repository). 
- *Assignment #2* - Cleaning the Dataset
    - Preparing our dataset for our future class database (Master dataset not available on repository).
- *Assignment #3* - Metadata
    - Creating a metadata file with all necessary components
- *Assingment #4* - Only Murders in the Database (SQL Murder Mystery)
    - Learn to use SQL queries to find the murderer within the database.  
- *Assignment #5* - Only Murders in the Database Continued (SQL Murder Mystery)
    -   Build on the work from assignment 2 and work on more queries to strengthen SQL skills. 
