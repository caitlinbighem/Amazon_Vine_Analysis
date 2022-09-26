# Amazon Vine Analysis
 
Amazon Vine Analysis can be found here: https://github.com/caitlinbighem/Amazon_Vine_Analysis
 
## Objective
 
Similar to a large percentage of consumers, Amazon shoppers rely on reviews to inform their shopping and purchasing decisions.While Amazon’s vine review datasets are available to the public and can be found here (https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt), these vine reviews are fairly large and therefore may be too dense for the average unit to handle. With this in mind, Spark and AWS are being utilized in this analysis.
 
The first objective is to perform the ETL process entirely in the cloud and upload a DataFrame to an RDS instance. The second objective is to employ PySpark to generate a statistical analysis of the desired data. Other tools include AWS, RDS, S3, Python, PySpark and Google Colab Notebooks.
 
### Data
 
Music
https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Music_v1_00.tsv.gz

### Images

![Vine Greater than 50](https://github.com/caitlinbighem/Amazon_Vine_Analysis/blob/main/Resources/Screenshot%20.PNG)

## Results
 
For this analysis, we took the total number of reviews and applied a filter to the DataFrames to determine how many were either paid or unpaid. Out of the 4.75 million reviews contained in this dataset, this filter showed there was a grand total of seven that were paid reviews. Next, we determined the amount of 5-Star ratings associated with these reviews that were from unpaid sources. From this research, we were able to determine there were 67,580 5-Star ratings resulting from unpaid reviews. Finally, we calculated the percentage of 5-Star ratings which came to a total of 63.77% from unpaid sources.
