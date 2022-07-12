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
  



## Results:

## Challenge:
PyCitySchools.ipynb is the jupiter notebook I started the analysis in. 