# School_District_Analysis
**PyCitySchools with Pandas**

## Main Objective
1. Open Jupyter Notebook files from local directories using a development environment.
2. Read an external CSV file into a DataFrame.
3. Format a DataFrame column.
4. Determine data types of row values in a DataFrame.
5. Retrieve data from specific columns of a DataFrame.
6. Merge, filter, slice, and sort a DataFrame.
7. Apply the groupby() function to a DataFrame.
8. Use multiple methods to perform a function on a DataFrame.
9. Perform mathematical calculations on columns of a DataFrame or Series.


## Purpose
A school district asked for a snapshot of several key metrics by each school campus and by the district level.  The main analysis focused on the performance of math and reading scores disaggregated several ways in preparation for a board meeting.  However, after the school board reviewed the data, it was determined that the data from Thomas High School's 9th grade class was suspect of cheating.  The school board asked for the data to be removed and analyzed again for a comparison. 

## Results

### How is the district summary affected?

Original Data:
<img width="700" alt="1_dist_origin" src="https://user-images.githubusercontent.com/68654746/196312645-0c0e7fbc-ba0c-4403-8e42-555208ab6db5.png">

In the challenge work, I updated the district summary by changing the testing data of *461* 9th graders at Thomas High School into null data. Next, I recalculated the total student count by subtracting the number of ninth-grade students in Thomas High School from the total student count, and then recalculate the passing math and passing reading percentages. The overall passing percentage was then recalculated with the total student count.

Adjusted Data:
<img width="699" alt="2_dist_adjusted" src="https://user-images.githubusercontent.com/68654746/196313923-a444cb47-aedb-41d3-b56e-a6843c62ec27.png">

**Findings...**
Comparing the original and adjusted summaries, the results were not significant after removing 461 test scores on the 39,170 student data set. There is less than a 1% difference in the overall percent passing rate and indifferent when rounding the results to the same whole number.

### How is the school summary affected?

Original Data:
<img width="748" alt="2_school_origin" src="https://user-images.githubusercontent.com/68654746/196315131-319c3f8f-8dc1-4b63-83f7-18396e686304.png">

In the challenge work, I updated the school summary of the 10th-12th graders from Thomas High School after the testing data was adjusted above.

Adjusted Data:
<img width="753" alt="2_school_adjusted" src="https://user-images.githubusercontent.com/68654746/196315472-c3478ba7-e593-49be-b7e1-698e87cda5b4.png">

**Findings...**
In the new findings, removing the 9th grade students performance from the dataset caused a significant change in the overall percent passing rate, dropping from 91% to 65%.

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

Original Data:
<img width="748" alt="3_top_5_schools" src="https://user-images.githubusercontent.com/68654746/196315889-049f41fb-e933-4229-ab76-8a701d18ce44.png">

Adjusted Data:
<img width="748" alt="3_top_5_schools" src="https://user-images.githubusercontent.com/68654746/196315979-96225370-c515-4d55-bbeb-e2ca83f21ad5.png">

**Findings...**
In the original analysis, Thomas High School ranked 2nd in the district. But after adjusting the 9th grade data, Thomas High School ranked in the exact middle of 15 campuses at 8th from the bottom. 

### How does replacing the ninth-grade scores affect the following:
*Math and reading scores by grade:*

![4_avgs_origin](https://user-images.githubusercontent.com/68654746/196317840-33d17015-67bc-4cef-9199-1fabb2267669.jpg)

In the original analysis, 9th graders at Thomas High School had 83.4 math average and 83.8 reading average. In the new analysis, I replaced the 9th grade scores with null values as NaN.

Adjusted Average Math Scores     //     Adjusted Average Reading Scores:

<img width="228" alt="4_avgs_adjusted" src="https://user-images.githubusercontent.com/68654746/196318054-c51f0d64-4116-4b12-977b-c290b0c3b2c0.png"><img width="236" alt="4_avgs_adjusted2" src="https://user-images.githubusercontent.com/68654746/196318177-cd44a45c-626c-4315-b6cd-0ff5fbae4749.png">

*Scores by school spending:*

*Scores by school size:*

*Scores by school type:*


## Summary: Summarize four major changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

1. The overall passing rate for Thomas High School changed dramatically from 91% to 65%. 

2. Thomas High School's ranking dropped from 2nd to 8th in the district of 15 campuses. 

3. Data at the grade level will now show as "NaN" in reports for the 9th grade students at Thomas High School  

4. In addition to the overall passing rate, the campus math and reading averages and passing percentages all saw shifts.  

The major changes will be seen at the lower views of the disaggregated data with minor impact to the larger data views.
