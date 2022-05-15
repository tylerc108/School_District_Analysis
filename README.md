# School_District_Analysis

## Overview 

In this module, we assisted a data analyst named Maria in conducting analysis on a variety of schools in a school district. We looked at several variables relating to each school, such as the funding each school is provided and the average grades of students in the school. With the analysis that we produced in this module, the school board will be better equiped to make decisions for how to manage these schools. The analysis we provided can help the school boards understand which schools are scoring the lowest on certain subjects and therefore which schools need more assistance to ensure better outcomes for all students. We also looked at how funding can affect the average grades of students at each school, which will help the school boards understand which schools require more funding and whether or not increasing funding can directly improve student outcomes.

## Results:
### District Summary
Below is the original district summary:
<img width="927" alt="Screen Shot 2022-05-14 at 12 50 35 PM" src="https://user-images.githubusercontent.com/103055666/168441199-2432bccc-fcc5-4def-9982-f8d9fad88c95.png">

Below is the new district summary, after dropping the 9th graders of Thomas High School from the data:
<img width="928" alt="Screen Shot 2022-05-14 at 1 11 35 PM" src="https://user-images.githubusercontent.com/103055666/168441869-1f8cf550-0262-45fb-819f-7099d25a7e3d.png">


* Looking at the two tables above, we can see that dropping the 9th graders form the data altered the outcome in the district summary slightly. Originally, the overall passing percentage was 65.2%. After dropping the 9th graders from the data, it was 64.9%. The Average Math Score changed from 79.0 to 78.9, the Average Reading Score was unchanged, % Passing Math changed from 75.0 to 74.8, and % Passing Reading changed from 85.8 to 85.7. Overall, there were only slight changes to the school district data frame after dropping the 9th graders of Thomas High School from the data set.

### School Summary

Below is the original school summary:
<img width="993" alt="Screen Shot 2022-05-14 at 1 17 36 PM" src="https://user-images.githubusercontent.com/103055666/168442044-e621a1a7-06e8-4ffb-8476-bed8179c7183.png">


Below is the row of the new school summary with the data from Thomas High School:
<img width="830" alt="Screen Shot 2022-05-14 at 1 13 40 PM" src="https://user-images.githubusercontent.com/103055666/168441924-aac15f9f-18e8-4842-afbe-3662a801f47d.png">


* Per the above images, the only change that dropping the 9th graders of Thomas High School from the data set created was in the row of the data frame holding the values for Thomas High School. In this row, the Avg. Math Score and Avg. Reading Score were unchanged, the % Passing Math went from 66.91% to 97.02%, % Passing Reading went from 69.66% to 97.02%, and % Overall Passing went from 65.08% to 90.63%.

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
* Replacing the 9th graders scores greatly imporved Thomas High School's performance. After the change was made to drop the 9th graders grades, Thomas High School was the #2 performing school in the district.
### How does replacing the ninth-grade scores affect the following?:
  * Math and reading scores by grade
    * Replacing the ninth grade scores with NaN does not affect scores by grade for 10th, 11th, and 12th grade math and reading scores. However, it does affect 9th grade scores in the "reading_scores_by_grade" and "math_scores_by_grade" data frames, because in the updated data frames the values are replaced with "NaN".
  * Scores by school spending
    * The "spending_summary_df" is affected by dropping the scores because it improves the scores and percentage passing for the $631-$645 range, as this is the bin that Thomas High School is in.
  * Scores by school size
    * The "size_summary_df" is affected by dropping the scores because it improves the scores and percentage passing rates for the "Medium" size category, which is the category that Thomas High School falls in.
  * Scores by school type
    * The "type_summary_df" is affected by dropping the scores because it improves the scores and percentage passing rates for the "Charter" size category, which is the category that Thomas High School falls in.

## Summary: 

In summary, dropping the Thomas High School 9th graders' scores improved Thomas High School's status on the school district analysis data frame. This includes the following four changes: 

1. Thomas High School's scores by school spending improved.
2. Thomas High School's scores by school size improved.
3. Thomas High School's scores by school type improved.
4. Thomas High School's % Overall Passing improved.
