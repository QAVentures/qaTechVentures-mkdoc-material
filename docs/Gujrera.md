
## Real e-state analysis of Gujrera Data
Market sizing for all construction projects in Gujrarat.

### 1. Introduction
- **Project Overview** :
    - The project aims to analyze the construction projects in Gujrarat and provide insights into the market size, profit margin etc. The data is extracted from the Gujrera website and transformed into a format that can be used for analysis.
- **Objectives** :
    - Demand Forecasting for constructions projects in Gujrarat.
- **Scope and Limitations** : 
    - The scope of this project is to analyze the construction projects in Gujrarat and provide insights into the market size, profit margin etc.

### 2. Methodology
- **Data Collection Methods**
   - Data source (Web scaraping): [Gujrera](https://gujrera.gujarat.gov.in/)

- **Data Extract**
    - Data is extracted from the Gujrera website using Python and Beautiful Soup library. The data is extracted  and stored in a CSV file. 
    - The data includes project details such as project name, project type, project status, project location, project size, project cost, and project completion date etc. json files are stored in google cloud Bucket for the trasformation process.

- **Data Transformation and Data load pipeline**
    - ETL pipeline is used to extract data from the source, transform it into a format that can be used for analysis, and load it into a data warehouse. 
    - The data is transformed using Python from google cloud bucket and loaded into a Big Query Database. The data is then queried using SQL to generate insights and visualizations.
    

- **Airflow DAG Creation**
    - Airflow is used to automate the ETL process. A DAG (Directed Acyclic Graph) is created to schedule the ETL process at regular intervals. 
    - The DAG is created using Python and the Airflow UI is used to monitor the ETL process.
    [Github](https://github.com/QAVentures/Gujrera-ETL.git)


### 3. Market Analysis

- **Profit Margin analysis**
     The profit margin is calculated for CENTRUM HEIGHTS,MAGNATE SQUARE,Rudram Icon,SHLOK INFINITY and the average profit margin is calculated. 
     - The profit margin is used to determine the most profitable project type. The profit margin is also used to determine the average profit margin for each project type.
    [profit Margin](https://docs.google.com/spreadsheets/d/1iOyhlXYo3G5Kh2om8exP8Ma--Jo9QZfiimtGlQMjGOk/edit?usp=sharing)


- **Underdevelopement project analysis**
    - The underdeveloped projects are identified by filtering the data by project status. 
    - The underdeveloped projects are then grouped by project type and the total number of underdeveloped projects for each project type is calculated.
    [Underdevelopment](https://docs.google.com/spreadsheets/d/1kuQrR_E996tftl4r4in-7fk_-G1dh57rR4bU9ckeL1c/edit?usp=sharing)

- **Gift city constructions analysis**
    - The data is filtered by project location to identify the projects in Gift city. 
    - The projects are then grouped by project type and the total number of projects for each project type is calculated.
    [Gift City](https://docs.google.com/spreadsheets/d/1GivZBFlTMx0hIRdcI0ttp6YpqWgKwDtUQBVN8dC7h9Y/edit?usp=sharing)


### 4. Dashboard for Gujrera Analysis
- **Dashboard**
    - A dashboard is created using Streamlit to visualize the insights generated from the data.
    - The dashboard is made dynamic and deployed on streamlit cloud. 
    [Dashboard](https://gujera-analysis.streamlit.app/)
 




