# Mental Health Survey Analysis - SQL & Python

This project conducts an exploratory data analysis (EDA) on a mental health survey dataset, utilizing SQL for data validation, manipulation, and exploration and Python for data visualization.

## Dataset Overview
This data is from Open Source Mental Illness (OSMI) using survey data from the years 2014, 2016, 2017, 2018 and 2019, comprising of 3 tables:

##### Survey: 
- Includes records for surveys conducted in the years 2014, 2016, 2017, 2018, and 2019.
- Serves as a reference table for identifying years & linking with the answers table.
##### Questions: 
- Includes 105 unique questions, covering various aspects of mental health in the workplace.
- Acts as a reference for mapping question IDs to the corresponding survey questions, aiding in interpreting survey responses stored in the answers table.
##### Answers:
- Stores all survey responses in a structured way, linking responses to questions, and survey years.

##### Key attributes include:
- **Age**: Respondent's age
- **Gender**: Respondent's gender
- **Country**: Respondent's country of residence
- **self_employed**: Self-employment status
- **family_history**: Family history of mental illness
- **treatment**: History of mental health treatment
- **work_interfere**: Impact of mental health on work
- **no_employees**: Number of employees in the company
- **remote_work**: Remote work status
- **tech_company**: Employment in a tech company
- **benefits**: Availability of mental health benefits
- **care_options**: Awareness of care options
- **wellness_program**: Availability of wellness programs
- **seek_help**: Provision of resources to seek help
- **anonymity**: Anonymity protection
- **mental_health_interview**: Willingness to discuss mental health in an interview

## Analysis Steps

1. **Data Loading**: Imported the dataset into a SQL database for efficient querying.

2. **Data Cleaning**:
   - **Handling Missing Values**: Identified and addressed missing values in critical columns.
   - **Standardizing Categorical Variables**: Standardized entries in the 'Gender' column to ensure consistency.
   - **Outlier Treatment**: Identified and handled outlies in the 'Age' column for efficient analysis.
      <img width="599" alt="image" src="https://github.com/user-attachments/assets/3b6a9903-6d65-4b5a-8d0c-8316db72acf1" />

3. **Exploratory Analysis**:
   - **Demographics**: Analyzed age and gender distributions.
   - 
      <img width="596" alt="image" src="https://github.com/user-attachments/assets/38634d34-5416-4272-8d95-270ad14fa633" />
      <img width="596" alt="image" src="https://github.com/user-attachments/assets/32c4ec23-07f4-4933-bb0f-ef2f3c6889c7" />
      
   - **Geographical Distribution**: Examined respondent distribution across countries.
   - 
      <img width="599" alt="image" src="https://github.com/user-attachments/assets/4676fc26-b9dc-479b-804c-6f103debdf9e" />
      <img width="598" alt="image" src="https://github.com/user-attachments/assets/c166cb62-ed66-41d4-9f4f-50d6a78fe05c" />
      
   - **Employment Factors**: Investigated the relationship between self-employment, company size, remote work, and mental health.
     
      <img width="595" alt="image" src="https://github.com/user-attachments/assets/dde7fa91-56a6-468c-8e8b-605261c05c09" />
      
   - **Mental Health Treatment**: Assessed the proportion of respondents who have sought treatment and the impact of family history.
     
      <img width="296" alt="image" src="https://github.com/user-attachments/assets/62b089b0-1f0d-4810-9402-6a54ef912490" />
      <img width="594" alt="image" src="https://github.com/user-attachments/assets/6354748b-2e99-44f9-9c18-4620846a36dd" />

4. **Visualization**: Utilized Python libraries to create visual representations of the findings, including bar charts, histograms, and pie charts. 

## Key Findings

- **Age Distribution**: Most respondents are between 25 and 35 years old.
- **Gender Representation**: Predominantly male respondents, with a smaller proportion of female and non-binary individuals.
- **Geographical Insights**: The highest number of responses was from the United States, followed by other countries.
- **Mental Health Treatment**: A significant portion has sought mental health treatment, with family history being a contributing factor.

## Conclusion

The analysis provides insights into mental health awareness and support within the tech industry. It highlights areas where organizations can improve resources and foster an environment encouraging open discussions about mental health.

## Repository Structure

- **`EDA Notebook.ipynb`**: Jupyter Notebook containing the detailed analysis and visualizations.
- **`mental_health.sqlite`**: SQLite database file with the survey data.
- **`README.md`**: Project overview and documentation.

## Requirements

- Python 3.x
- Jupyter Notebook
- SQLite
- Python libraries: pandas, matplotlib, seaborn, sqlite3

## References
- [Mental Health in Tech Survey Dataset](https://www.kaggle.com/datasets/anth7310/mental-health-in-the-tech-industry/data?select=mental_health.sqlite)
