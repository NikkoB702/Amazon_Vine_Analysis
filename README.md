# Amazon_Vine_Analysis

## Overview

The question was asked after the launch of Amazon Vine, is there a presence of bias leaning towards positive reviews from reviewers who are receiving monetary gains from their participation? With many options to choose from, today we will focus on reviews concerning groceries. 


##### Resources

Data Source: [Amazon Review Dataset; US Grocery Review Dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)

Software: Google Colab, PySpark, AWS


## Results

Our results are filtered with this criterion in mind; reviews needed at least 20 votes to qualify and 50% or more of those votes need to be considered helpful by the user. From there we created two data frames: Vine program reviews and non-Vine program reviews. 

* How many Vine reviews and non-Vine reviews were there?

![paid_total_reviews](https://user-images.githubusercontent.com/80132877/211380542-ae67255d-9ce0-4546-b9d1-2bb4fe1bf494.png)

![unpaid_total_reviews](https://user-images.githubusercontent.com/80132877/211380573-697871f8-9494-43e6-8ce5-cec06acb2dfa.png)

* How many Vine reviews were five stars? How many non-Vine reviews were five stars?

![paid_5_star_reviews](https://user-images.githubusercontent.com/80132877/211380687-3d94abd4-c1f9-49dc-bd1e-e80835b3d0b3.png)

![unpaid_5_star_reviews](https://user-images.githubusercontent.com/80132877/211380711-0b9595f4-d62a-4011-b028-e4ac206f405f.png)

* What percentage of Vine reviews were five stars? What percentage of non-Vine reviews were five stars?

![paid_5_star_percentage](https://user-images.githubusercontent.com/80132877/211380795-0b1943a2-f403-43f1-b3dd-611d693edd53.png)

![unpaid_5_star_percentage](https://user-images.githubusercontent.com/80132877/211380827-ec6cfb47-1ccd-4d49-a509-b349c758eb9f.png)


## Summary

![paid_unpaid_splits](https://user-images.githubusercontent.com/80132877/211380932-37ad78f2-f473-4008-abf3-27e96893d56b.png)

Based on our calculations it appears that positive bias doesn’t exist when analyzing the percentages of five-star reviews between Vine and non-Vine reviewers. As we examine our splits; five-star ratings by Vine program reviewers happen roughly 35% of the time while 5-star non-Vine reviews occur roughly 69% of the time. With this in mind, we can categorize reviews by their respective star ratings and use our formulas to provide more insight into any correlation between 5-star ratings and their respective counterparts. Additionally, I would suggest lowering the criterion of 20 votes to qualify down to 10 votes. That would increase the overall number of reviews to analyze.
