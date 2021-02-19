# Amazon_Vine_Analysis

## Summary

- Used knowlege of bid data to perform ETL on a dataset from Amazon. The purpose of the analysis was to determine if there were any positivity bias for in video game reviews in the Amazon Vine Program. The analysis was done using pythons pyspark library combined with an AWS relational database and a PostgreSQL database.

## Overview

### Performed ETL on Amazon Product Reviews

- Used knowledge of the cloud ETL process, created an AWS RDS database with tables in pgAdmin, picked a dataset from the Amazon Review datasets (Links to an external site.), and extracted the dataset into a DataFrame. Transformed the DataFrame into four separate DataFrames that match the table schema in pgAdmin. Then, uploaded the transformed data into the appropriate tables and run queries in pgAdmin to confirm that the data has been uploaded.

### Determined Bias of Vine Reviews

- Used knowledge of PySpark to determine if there is any bias towards reviews that were written as part of the Vine program. For this analysis, determined if having a paid Vine review makes a difference in the percentage of 5-star reviews.

## Results

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
  - There were 1,607 Vine reviews and 1,025,317 non-vine reviews 
- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
  - The percentage of Vine reviews was 0.156 % and the percentage non-vine reviews was 99.8 %
  ![Screen Shot 2021-02-02 at 8 11 59 PM](https://user-images.githubusercontent.com/16258584/106694109-7e68cb80-659d-11eb-8108-52b6ed3c0c63.png)
## Conclusion

- The analysis did not show a positivity bias for the Amazon Vine rating program. Less than one percent of five star reviews came from Vine members. The vast majority of reviews that were five stars were not part of the Amazon Vine program. Therefore there is not evidence for a positivity bias for reviews in the Amazon Vine program. An additional analysis that could be done to test bias would be to measure the different percentages in one star ratings. 
