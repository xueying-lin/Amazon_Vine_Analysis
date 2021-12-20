# Amazon_Vine_Analysis

## Overview
 I am working on a project which is analyzing Amazon reviews written by memebers of the paid Amazon Vine program. There will be approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wirless products. I will pick *the reviews of music instruments* and use PySpark to extract and transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin.
 - Purpose: Determine whether there is **any bias** toward favorable reviews from **Vine members** in the dataset.
 
## Results
1. There are **60 total Vine reviews** and **14477 total non-Vine reviews.**
-![Total reviews comparison](https://github.com/xueying-lin/Amazon_Vine_Analysis/blob/65ad20fa024b0edc70246e773684253ac1a6ce9e/challenges/total%20views.PNG)

2. There are **34 Vine 5-star reviews** and **8212 non-Vine 5-star reviews**.
-![5-star reviews comparison](https://github.com/xueying-lin/Amazon_Vine_Analysis/blob/65ad20fa024b0edc70246e773684253ac1a6ce9e/challenges/5-star.PNG)

3. Around **56.67% of Vine reviews** were 5 stars and **56.72% of non-Vine reviews** were 5-star
-![5-star reviews percentage comparison](https://github.com/xueying-lin/Amazon_Vine_Analysis/blob/65ad20fa024b0edc70246e773684253ac1a6ce9e/challenges/percentage.PNG)


## Summary
Since the difference between the 5-star percentage of vine and non-vine reviews is only 0.05%, there is **no noticable positivity bias** for reviews in the Vine program.
The other way to support this statement is comparing the positivity of vine and non-vine customers through analyzing their review_body. The **NLP technique** could be applied to make a ML module , identifying the positivity of each review. And then count the positive reviews of each group and make the comparison of the percentage of positive reviews. 
