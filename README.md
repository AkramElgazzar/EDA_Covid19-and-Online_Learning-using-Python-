# EDA_Covid19-and-Online_Learning-using-Python

This project explores how COVID-19 has impacted student and teacher engagement and performance across US districts using LearnPlatform data.

I used a dataset from a Kaggle for my analysis.
Here is the link to the data:[ https://www.kaggle.com/competitions/learnplatform-covid19-impact-on-digital-learning/data]

# Project Goals:
- Analyze LearnPlatform data on COVID-19's impact on digital learning.
- Gain insights into demographics, expenditure, time, products & services, access, and engagement index.
- Draw conclusions about COVID-19's influence on digital learning adoption and usage.

# Data Description:
The data consists of three files:
1- districts_info.csv: contains information about the districts, such as the state, locale, and per-pupil expenditure.
2- products_info.csv: contains information about the products, such as the product id, sector, and primary essential function.
3- engagement_data: contains engagement data of students and teachers for each product and district, such as the time, lp id, pct_access, and engagement_index.

The data covers the period from January 2020 to December 2020, and includes 233 districts and 372 products.

# the data cleaning and analysis steps:

**Data Cleaning:**

1. **Import Libraries:** numpy, pandas, matplotlib
2. **Read Data:** Load districts, products, engagement datasets
3. **Clean Districts Data:**
    - Change district_id to string
    - Delete records with high missing values
    - Replace NaN in last 4 columns with mean
4. **Clean Products Data:**
    - Change id to string
    - Replace NaN with mode
    - Derive categories and sectors columns
    - Rename LP ID to lp_id
5. **Clean Engagement Data:**
    - Change time to datetime
    - Change lp_id to string
    - Impute pct_access and engagement_index with median
    - Remove ".csv" from district_id

**Data Analysis:**

1. Merging the three data frames into one final data frame
2. Save Final DataFrame:** As "final_Covid19_df.csv"
3. Clean the "final_Covid19_df" Data
4. Explore and Variables
5. Explore Relationships between variables
6. Create Visualizations
7. Extract Insights
   

# Key Findings:

**Demographics**:
- The most common state in which students reside is Connecticut followed by Utah & Illinois. while the least common one is North Dakota.
- The locale where most students exist is the suburb and the area where we have the fewest number of students is the town


**Expenditure**:
- The local and federal expenditure is between 14000-16000 for the majority of students. While very few minorities recieve a high total expenditure of 32000-34000.
- The 3 states that spend the most expenditure per pupil in total are Utah, Illinois, and Massachusetts. The least spending state is Minnesota with a total of 15463
- The government spends the most expenditure on students from the suburbs and the least on town students.

**Time**:
The data has been extracted from ist January 2020 to 1 January 2021. The highest amount of data was extracted from September to Decerhber 2020

**Products & Services**:
- The most used products in general are all developed by Google.
- The top provider of learning products is Google followed by Microsoft and XL Learning.
- The most prevalent education sector is PreK-12 which includes students aging 5 to 18 years old. The least common sectors are the Higher Education and corporate.
- The majority of products and services are digital learning platforms. While the least prevalent type of services provided are Sites, Resources & References.

- **Access**:
- The state with the highest average percentage of access is North Dakota. The least average access goes to Ohio.
- The product with the highest average percentage of access is Google Classroom. The least average access goes to Zoom.
- The highest average percentage of access was noticed between September and October. The least was in the middle of August.

**Engagement Index**:
- The highest average engagement index was noticed at the beginning of October. The least at the beginning of January.
- The state with the highest average engagement index is Arizona. While the least engagement is noticed in Tennessee.
- The highest average engagement is noticed in rural areas while the least is in the city.
- The product with the highest average engagement index is Google Docs. The least engagement goes to Google Sheets.
- The sector with the highest average engagement is The PreK-12; Higher Ed;Corporate. The least engagement is noticed in the Higher Ed; Corporate sector.
- The provider that has the highest average engagement index is Instructure,inc. While the least engagement goes to MIND Research Institute.


# Finally:
• It has been reported that Covid-19 arrived in the United states on 13 January 2020, which coincides with the nearly the same they started collecting this dataset. 
  From the chart we notice that the there wasn't much engagement at the beginning because the virus wasn't so fierce then. yet, the average access was very high.

• This confirms that by the arrival of Covid-19 in the United States, there was a noticeable transformation to digital learning especially by the PreK-12 sector and Google products were the most used services at that time especially digital learning platforms which replaced gradually classrooms in schools
