# School_District_Analysis

## Project Overview
Looking for performance trends and patterns related to school budgets and their students' test scores to inform discussion and strategic decisions at the school and district level. 

#### Resources:
 - Data Source: schools_complete.csv, students_complete.csv
 - Software: Python 3.7.13, Pandas 1.3.5, Numpy 1.21.5, jupyter notebook (notebook server 6.4.8, Ipython 7.31.1)

## Summary:
The data includes:
  - 39,000+ students, their grade years, 15 schools, budgets and test scores and no null/NaN values.
  - Students_df['student_name'][3] has a prefix that should not be there, these are high school kids not Doctor's. I needed to find and clean the names of improper prefixes and suffixes.

The anticipated performance summary tables:  
  - District Summary: An overall snapshot of all schools. (total students, budget, average test scores, % passing subjects, % passing overall)
  - School Type Summary: District Summary based on the type of school.
  - School Summary: District Summary that compares each school.
  - School Size Summary: Schools sorted according to their size, determined by the number of students.
  - Spending Summary: Schools sorted according to their budget per student.

# Results:
## District Performance Summary
![District Summary](/Resources/initial_district_summary.png)

 - Overall passing percentage is so much lower than the individual passing percentage for each subject.

## School Type Performance Summary
![Sorted by School Type](/Resources/initial_school_type_summary.png)
 - The charter schools are performing alot better than the district schools.

## School Performance Summary
#### Top 5 Best
![Top 5 best](/Resources/initial_top5_best_summary.png)
 - The best schools are all charter schools and have 90% of their students Passing.
#### Top 5 Worst
![Top 5 worst](/Resources/initial_top5_worst_summary.png) 
 - The worst schools are all district schools and have 53% of their students Passing.
 - The best performing schools have fewer students than the worst performing schools. I wonder if this is related to the student teacher ratio. Number of teachers per school is not in the data set.

## Performance Summary Sorted by School Size 
![Sorted by school size](/Resources/initial_school_size_summary.png)
 - The small and medium schools are doing so much better than the large and extra large schools, a drastic difference. it looks identical to the top 5 best/worst comparison.

## Performance Summary Sorted by Spending
![Sorted by spending per student](/Resources/initial_spending_summary.png)
 - Spending ranges shows the budget amount per student has an inverse correlation to the % Passing Overall. The problem is not "Not enough money".

### Ending Analysis:
 - The Charter schools are smaller than the District schools.
 - The Charter schools have a lower budget than the Distrct schools. 
 - The Charter schools are outperforming the District schools. 

# Challenge:
The PyCitySchools.ipynb notebook is an anlysis is as if all the data in the in the dataset is true. The PyCitySchools_Challenge_testing.ipynb notebook assumes that Thomas High School has some falsely reported math and reading scores for ninth graders in it, until that data can be verified it will not be used in the analysis. Those scores will be replaced with NaN values. How does this affect the analysis?

### Challenge Results:
Vary little actually changed. The removed data ended up being 461 students, or 1.17% of the total student population. The largest visible difference in the performance summary tables is the District Summary and the Top 5 Best Schools. 
![New District Summary](/Resources/challenge_district_summary.png)
 - The percent of overall passing students dropped by 0.3%, the percentage of students passing reading went down by 0.1%, and the average math score dropped by 0.1.
 - Thomas High school dropped from #2 ranking to #3.
   - 0.3% drop in overall passing students and passing reading
   - 0.2% drop in students passing math
   - 0.1 increase in average reading score
![Top 5 Best Schools](/Resources/challenge_top5_best_summary.png)
 - The 0.1% drop in overall passing students and those passing reading is also visible in the spending and school size Performance Summary Tables 
![New Spending Performance Summary](/Resources/challenge_spending_summary.png)
![New School Size Performance Summary](/Resources/challenge_school_size_summary.png)
