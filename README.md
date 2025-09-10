# SAT Performance Analysis in New York City Public Schools

![schoolbus](https://github.com/user-attachments/assets/1d867bbe-9c2f-45d8-8a04-b695b600c9fa)

## An Analysis of NYC High School SAT Performance

Standardized tests like the SAT are a cornerstone of the American education system, providing a uniform measure of literacy, numeracy, and writing skills for high school students. With each of the three sections, reading, math, and writing, carrying a maximum of 800 points, these scores are critical for college admissions. This report analyzes SAT performance across New York City's public schools to identify key trends and top-performing institutions.

### Data and Key Questions

The analysis is based on the `schools.csv` dataset, which contains SAT performance data for various high schools across NYC's boroughs. The investigation focuses on answering three primary questions:

1.  Which schools are the top performers in mathematics?
2.  What are the top 10 schools based on combined SAT scores?
3.  Which borough has the largest variation in school performance?
   
## Analysis and Results

### Top Performing Schools in Math

To identify schools with outstanding math performance, we filtered for those with an **average math score of at least 640**, which is 80% of the maximum possible score. The resulting list, `best_math_schools`, highlights the elite schools that excel in this subject, sorted from highest to lowest score.

### Top 10 Schools by Total SAT Score

For a holistic view of performance, a `total_SAT` score was calculated for each school by summing the `average_math`, `average_reading`, and `average_writing` scores. The schools were then ranked by this combined score to identify the overall top 10 performers in NYC. This produced the `top_10_schools` DataFrame.

### Borough with the Largest Spread in Scores

To understand performance diversity, the data was grouped by borough. We calculated the number of schools, the average SAT score, and the standard deviation of SAT scores for each borough. The **standard deviation** is a key metric here, as a higher value indicates a greater disparity between the highest and lowest-scoring schools within a borough.

The analysis identified that **Manhattan** has the largest standard deviation in SAT scores (230), indicating the most significant performance gap between its schools. The full result is stored in the `largest_std_dev` DataFrame.

## Conclusion

This analysis successfully identified key performance metrics within the NYC public school system. We pinpointed the schools with the highest achievement in mathematics, ranked the top 10 schools based on their combined SAT scores, and determined that Manhattan is the borough with the most varied academic performance among its high schools.

## Tools Used

  * **Python**
  * **Pandas**
