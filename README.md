# Amazon_Vine_Analysis

## Overview of the analysis

Since your work with Jennifer on the SellBy project was so successful, you’ve been tasked with another, larger project: analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, you’ll have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. You’ll need to pick one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, you’ll use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset. Then, you’ll write a summary of the analysis for Jennifer to submit to the SellBy stakeholders.

## Results

- How many Vine reviews and non-Vine reviews were there?

For the Furniture product review file, there were 2,775 Vine reviews (0.4%) and 789,338 non-Vine reviews (99.6%) for a total of 792,113 reviews:

![image](https://user-images.githubusercontent.com/76754655/120937158-c2411e00-c6c0-11eb-8535-3b54d6911970.png)

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

There were 1,356 Vine reviews with 5 stars (0.3%) and 446,360 non-Vine reviews with 5 stars (99.7%) for a total of 447,716 5 star reviews:

![image](https://user-images.githubusercontent.com/76754655/120937264-7642a900-c6c1-11eb-8124-494209a02a2f.png)

- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

There were 1,356 Vine reviews that were 5 stars (48.9%) and 1,419 remaining Vine reviews (51.1%) for a total of 2,775 Vine reviews. In addition, there were 446,360 non-Vine reviews that were 5 stars (56.5%) and 342,978 remaining non-Vine reviews (43.5%) for a total of 789,338 non-Vine reviews:

![image](https://user-images.githubusercontent.com/76754655/120937394-0bde3880-c6c2-11eb-896f-c21bf7f1b867.png)

## Summary

In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.

In summary, there appears to not be positivity bias for reviews in the Vine program given that there is a higher percentage of non-Vine reviews that were 5 stars (56.5%) compared to the percentage of Vine reviews that were 5 stars (48.9%). One additional analysis that can be done with the dataset to support this would be to determine the skew of Vine and non-Vine reviews across 1-5 stars to see if there is any positivity bias for reviews in the Vine program.
