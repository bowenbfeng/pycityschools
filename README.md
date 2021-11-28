# PyCitySchools: School District Analysis

## Overview of the school district analysis

> The school board has notified Maria and her supervisor that the file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Although the school board does not know the full extent of the academic dishonesty, they want to uphold state-testing standards. 

In this analysis, all the reading and math grades for Thomas High School ninth graders have been changed to NaNs. In addition, the number of Thomas High School ninth graders is deducted from the total number of students in Thomas High School so that a fair evaluation of the school's performance can be concluded. 

## Results

Below are the results after all the reading and math grades for Thomas High School ninth graders have been changed to NaNs. 

### The effect on district summary

As can be concluded, after the change, with excluding the reading and math scores for Thomas High School ninth graders, the average math score chagned from 79.0 to 78.9, while the average reading score slightly changed. The percentage of students passing reading tests changed from 86.0% to 85.7% while that of students passing math tests changed from 65.0% to 64.9%. 

Before, the district summary looked like the following. 

![](/Resources/district_summary_0.png)

After the change, the district summary looks like the following. 

![](/Resources/district_summary_1.png)

### The effect on school summary

After all the reading and math grades for Thomas High School ninth graders have been changed to NaNs, when calculating the average score or the percentage passing, those students are not excluded from the analysis. That's why we are seeing only 65.1% overall passing percentage for all the students of Thomas High School. 

![](/Resources/school_summary_0.png)

Therefore, we need to exclude those students of whom the grades have been changed to NaNs. After doing this process, we can see a 90.6% of overall passing percentage for all the students of Thomas High School, which is the correct way to calculate the average score and the percentage passing, which stops Thomas High School's performance being underrated. 

![](/Resources/school_summary_1.png)

### The effect on Thomas High School's performance

Initially, when the number of Thomas High School ninth graders were not excluded, the overall passing percentage was only 65.1%, which was way below average. After excluding the number of Thomas High School ninth graders, the overall passing percentage is increased to 90.6%, which is calculated based on the correct method. In this way, Thomas High School's performance is stopped from being underrated. 

### Other effects

Below are other minor effects brought by the change. 

* Math and reading scores by grade
  
  As can be see from the below two screenshots, the reading and math grades for Thomas High School ninth grades have been excluded and become null. 
  
  ![](/Resources/reading_by_grade.png)
  
  ![](/Resources/math_by_grade.png)

* Scores by school spending

  As the spending per student of Thomas High School is within the $630-644 range before and after the adjustment, the rest of the rows did not change after the adjustment. The change to the schools's performance within the $630-644 range of spending per student changed only slightly, with the overall passing percentage decreasing from 62.86% to 62.78% if we round off to 2 decimal places. 
  
  Below shows the data before the adjustment. 
  
  ![](/Resources/school_spending_0.png)
  
  Below shows the data after the adjustment. 
  
  ![](/Resources/school_spending_1.png)

* Scores by school size

  As the size of Thomas High School is medium (1000-2000) before and after the adjustment, the rest of the rows did not change after the adjustment. The change to the schools's performance of the medium size category changed only slightly, with the overall passing percentage decreasing from 90.62% to 90.56% if we round off to 2 decimal places. 
  
  Below shows the data before the adjustment. 
  
  ![](/Resources/school_size_0.png)
  
  Below shows the data after the adjustment. 
  
  ![](/Resources/school_size_1.png)

* Scores by school type
  
  As the type of Thomas High School is Charter, the District row did not change after the adjustment. The change to the schools's performance of the Charter category changed only slightly, with the overall passing percentage decreasing from 90.43% to 90.39% if we round off to 2 decimal places. 
  
  Below shows the data before the adjustment. 
  
  ![](/Resources/school_type_0.png)
  
  Below shows the data after the adjustment. 
  
  ![](/Resources/school_type_1.png)

## Summary

1. District: as can be concluded, after the change, with excluding the reading and math scores for Thomas High School ninth graders, the average math score chagned from 79.0 to 78.9, while the average reading score slightly changed. The percentage of students passing reading tests changed from 86.0% to 85.7% while that of students passing math tests changed from 65.0% to 64.9%. 
2. School: after all the reading and math grades for Thomas High School ninth graders have been changed to NaNs, when calculating the average score or the percentage passing, those students are not excluded from the analysis. That's why we are seeing only 65.1% overall passing percentage for all the students of Thomas High School. After excluding those students of whom the grades have been changed to NaNs, we can see a 90.6% of overall passing percentage for all the students of Thomas High School, which is the correct way to calculate the average score and the percentage passing, which stops Thomas High School's performance being underrated. 
3. The math and reading scores by grade: the math and reading scores of Thomas High School's ninth graders are all excluded and changed to null. 
4. Being the result of the above mentioned steps, there are slight changes (decreases) in scores by school spending, scores by school size, and scores by school type. 
