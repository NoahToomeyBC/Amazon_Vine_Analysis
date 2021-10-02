# Amazon Vine Program Analysis

## Purpose
Using a dataset containing video game review metrics, we examined the validity and effectiveness of Amazon's "Vine" review program and whether or not paid reviews would create a notable bias. We pulled data from an S3 bucket and preformed transformations on the data using PySpark and Google CoLabs to clean our data and ready it to be imported to a local machine in order to preform analysis on the most important data which we had output to a new dataset labeled vine_table.csv. From there, we were able to further seperate the data into two sets: the reviews completed using the Vine program and the organic reviews.

## Results

The following information was found through the use of Pandas to preform aggregations and filtering on our Vine and Organic datasets

### Vine Program Results

![Vine_Program_Figures](https://user-images.githubusercontent.com/85508764/135726699-e7e595ff-2c14-4f87-80f7-ad36f0032175.png)

### Organic Review Results

![Unpaid_review_figures](https://user-images.githubusercontent.com/85508764/135726712-b1d72506-de7a-4eef-acf6-164e4f6e76f2.png)

# Findings and Conclusions

### Positivity Bias

In this dataset, we find that the number of five star reviews represent a very small portion of the overall vote count. While there is more of a positivity bias found in the Vine program it only is about .1 percent more (.0082) than that of the organic reviews (.0069). A more effective analysis would be to look at the average star rating  of Vine reviews compared to the average star rating for organic reviews. This would give us a much broader look at the data and allow for further analysis to be done. In addition, this analysis could be reproduced for all of the star ratings (4 stars, 3 stars, etc.) to further examine the presence of positivity bias in the data.
