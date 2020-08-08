# School District Analysis

## Overview of the School Data Analysis Project
Here is the list of deliverables for the analysis of the school district: 
- A high-level snapshot of the district's key metrics, presented in a table format
- An overview of the key metrics for each school, presented in a table format
- Tables presenting each of the following metrics:
	- Top 5 and bottom 5 performing schools, based on the overall passing rate
	- The average math score received by students in each grade level at each school
	- The average reading score received by students in each grade level at each school
	- School performance based on the budget per student
	- School performance based on the school size 
	- School performance based on the type of school

We have replaced all of Thomas High School's 9th grade scores with 'NaN' to reflect that there may have been dishonest alterations, effectively removing all of those scores from the underlying math of the report.

## Results
### How is the district summary affected?
- Overall, the district summary saw only very minor changes with the removal of Thomas High School's 9th grade reading and math scores.
	- Average Math Score decreased by 0.1%.
	- % Passing Math, % Passing Reading, and % Overall Passing all decreased by 1%.

The below images show these changes.

![District summary with THS](https://github.com/timbannock/school-district-analysis/blob/master/Resources/district_summary_w_THS.PNG)

![District summary without THS](https://github.com/timbannock/school-district-analysis/blob/master/Resources/district_summary_wo_THS.PNG)

### How is the school summary affected, and how does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
- Interestingly, when you sort the school summary by descending order of % Overall Passing, Thomas High School drops off the list of Top 5 schools. Originally, it held second place. This suggests a significant % of the 9th grade reading and math grades pushed into the passing criteria (70 or above for a grade), which is logical if there was some dishonesty with the aim of boosting some students' grades.

The below images show these changes.

![School summary with THS](https://github.com/timbannock/school-district-analysis/blob/master/Resources/school_summary_descending_w_THS.PNG)

![School summary without THS](https://github.com/timbannock/school-district-analysis/blob/master/Resources/school_summary_descending_wo_THS.PNG)

### Math and reading scores by grade
In this case, Thomas High simply shows 'NaN' on the table for the 9th grade scores in both math and reading; the average scores themselves remain the same in all other grades, of course.

### Scores by school spending
- Sorting the scores by school spending reveals that Thomas High School is in the $630-644 range, and the % passing math and reading drop by 6 (math) or 7 (reading) points.
	-- If there was dishonest alterations of the grades, they were kept relatively "realistic" since the drop is not terribly significant, but certainly enough to show up in these statstical analyses.

The below images show these changes.

![School spending with THS](https://github.com/timbannock/school-district-analysis/blob/master/Resources/school_spending_w_THS.PNG)

![School spending without THS](https://github.com/timbannock/school-district-analysis/blob/master/Resources/school_spending_wo_THS.PNG)

### Scores by school size
- We once again see where Thomas High School exists: it's a Medium school according to the ranges we set (1000-2000). Only the numbers in that range band are affected.

The below images show these changes.

![School size with THS](https://github.com/timbannock/school-district-analysis/blob/master/Resources/school_size_w_THS.PNG)

![School size without THS](https://github.com/timbannock/school-district-analysis/blob/master/Resources/school_size_wo_THS.PNG)

### Scores by school type
- We find here that Thomas High School is charter school, as only the numbers on that row have been affected by removing Thomas High School's 9th grade math and reading scores.

The below images show these changes.

![School type with THS](https://github.com/timbannock/school-district-analysis/blob/master/Resources/school_type_w_THS.png)

![School type without THS](https://github.com/timbannock/school-district-analysis/blob/master/Resources/school_type_wo_THS.png)
