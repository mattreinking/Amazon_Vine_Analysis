# Amazon_Vine_Analysis

## Overview
Jennifer has asked me to take on a large project. I have been tasked with analyzing Amazon reviews written by members of the paid Amazon Vine program. Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. I will be using a dataset on video game reviews and using PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, I will be using PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset. Then, you’ll write a summary of the analysis for Jennifer to submit to the SellBy stakeholders.


## Results  
  
- How many Vine reviews and non-Vine reviews were there?  
![image](https://user-images.githubusercontent.com/86776606/199834031-eda56d28-11f8-430a-b79a-7c9fa3474dbe.png)
  - There were 94 Vine reviews
  - There were 40,471 non_vine reviews  

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?  
![image](https://user-images.githubusercontent.com/86776606/199834202-516dc104-0482-4e3b-b517-68d0bc5e8237.png)
  - There were 48 5-star Vine reviews
  - There were 15,663 5-star non-Vine reviews  

- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?  
![image](https://user-images.githubusercontent.com/86776606/199826329-b5c4311c-504b-4eff-9263-2ab308fd4f18.png)
  - 38% of Vine reviews were 5 stars
  - 39% of non-Vine reviews were 5 stars  

## Summary
The data above shows there is no positivity bias for reviews in the Vine program in terms of 5-star reviews. Out of the total 5-star reviews, only 1% more of reviews were non-Vine in comparison to Vine reviews. However, the sample sizes were extremely imbalanced. Only less than 100 reviews were from Vine out of over 40,000. Our results are inconclusive on bias. An additional analysis we could perform would be to gather data on 1-star reviews. Being able to calculate the statistics on negative reviews would help give better insight into any review bias there might be. It is quite possible that while Vine members may not be skewing reviews with positivity bias, there is a chance they may be compelled to minimize negativity bias. A lower percentage of negative reviews could still help products keep business afloat.
