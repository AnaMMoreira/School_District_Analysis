# School_District_Analysis
## Module4 Challenge


## Overview of the school district analysis: Explain the purpose of this analysis

Maria, the chief data scientist for the City School System, has been tasked to organize, analyze and summarize standardized testing results in order to present performance trends and patterns.  The findings will be used by the School Board and Superintendent to make decisions and plan strategies for school district management of school budgets and priorities.

After cleaning and organizing all the testing results data into an all inclusive dataframe, multiple filtering and calculations were performed based on the District Overall performance as seen in the table bellow

![[terminal output image]](https://github.com/AnaMMoreira/School_District_Analysis/blob/main/Resources/All_Data_DistrictSummary_Fig1.png)

It should be noted that the Overall passing is 65.2 % for the District, with a 75% and 85.8 % passing for Math and Reading correspondingly.  A 65.2% overall passing value is not necessarily a great performance for the District.  However it can be deduced that Overall performance of each school is NOT solely dependent on the School Budget and Budget-per-student amounts.

Further analysis of all the testing results data for each individual school and the corresponding school information such as budgets  and  school size can be viewed in the following table displaying all calculated parameters.  It can be observed that there is no obvious or distinguishing pattern that can be associated to performance.  Take note of the highlighted max values in each column.  It can however be deducted 

![insert table All_data_PERschool_summary_Fig2](https://github.com/AnaMMoreira/School_District_Analysis/blob/main/Resources/All_data_PERschool_summary_Fig2.png)

Sorting the data by Overall % Passing as a measure of performance discloses which schools are at the Top 5 ranking and the lower bottom 5 ranking schools.  See table AllData_top_n_bottom_schools_Fig3

![insert AllData_top_n_bottom_schools_Fig3](https://github.com/AnaMMoreira/School_District_Analysis/blob/main/Resources/AllData_top_n_bottom_schools_Fig3.png)

Furthermore, when sub setting the math and reading scores by grade for each school also demonstrates very little variance across grades.  Each grade seems to perform equally for Each school ranking. See summary tables in Figure 4a and Figure 4b

![Insert AllData_MathScoresbyGradeFig4a](https://github.com/AnaMMoreira/School_District_Analysis/blob/main/Resources/AllData_MathScoresbyGradeFig4a.png)
	
![AllData_ReadingScoresbyGradeFig4b](https://github.com/AnaMMoreira/School_District_Analysis/blob/main/Resources/AllData_ReadingScoresbyGradeFig4b.png)

Interestingly and counter intuitive is the inverse relationship displayed between Spending Ranges per student and performance as seen in figure 5.  The table shows that the lower spending per student schools are actually the ones with the higher performance.

![AllData_SpendingSummary_Fig5](https://github.com/AnaMMoreira/School_District_Analysis/blob/main/Resources/AllData_SpendingSummary_Fig5.png)


Further analysis of the data however did start to display a correlation between school size and performance.  The bigger the student counts the lower the performance and overall grades and percent passing numbers. Figure All_datal_PERsizesummary_Fig6

![insert All_datal_PERsizesummary_Fig6](https://github.com/AnaMMoreira/School_District_Analysis/blob/main/Resources/All_datal_PERsizesummary_Fig6.png)

Lastly,  the largest and most obvious correlation between the type and school and performance is displayed in table figure 7  where it can be seen that Charter schools outperform the district run schools by 36% MORE based on overall percent passing numbers, and 16% and 27% for reading and math percent passing correspondingly.  Even though, the average scores for the 2 school types were not that different.  There results are summarized bellow in figure 7

![insert All_datal_PERtypesummary_Fig7](https://github.com/AnaMMoreira/School_District_Analysis/blob/main/Resources/All_datal_PERtypeSummary_Fig7.png)

 
Due to the suspicion of academic dishonesty regarding reading and math grades for Thomas High School ninth graders, the school board has requested a comparison analysis.  The following analysis results excludes the testing results reported for the 9th grade students in the Thomas High School (THS).  This was accomplished by replacing the 9th grade math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. Percentages therefore were calculated by excluding these students from the total counts.
The following report describes how these changes affected the overall analysis presented above.

# Results: For Comparison Analysis Excluding Data Under Question 
## Omission of Thomas High School 9th Grade Standardized testing Results.

## How is the district summary affected?

In the following District Summary table Figure 8 it can be seen that the exclusion of the THS 9th grade test results resulted in a very small change in the Overall Percent passing value.  Its should be noted however that if the performance passing grade for the district is based on for example a 65% Overall passing result, this small and apparently insignificant 0.3% change could be the difference between a "passing" or "failing" status for the district. 

![insert noTHS9TH_DistrictSummary_Fig8](https://github.com/AnaMMoreira/School_District_Analysis/blob/main/Resources/noTHS9TH_DistrictSummary_Fig8.png)

## How is the school summary affected?

In the school summary table figure 9 it can be seen that removing the 9th grade scores lowered the percent passing numbers by approximately 0.3%, 0.1%, and 0.1%, for Overall, math and reading % passing results correspondingly. 

[insert noTHS9th_meansPERschool_Fig9](https://github.com/AnaMMoreira/School_District_Analysis/blob/main/Resources/noTHS9th_meansPERschool_Fig9.png)

## How does replacing the ninth graders??? math and reading scores affect Thomas High School???s performance relative to the other schools?

Excluding the 9th grade test scores did not affect the overall placement or ranking of Thomas High School.  See Figure 10 for reference.

[insert top_n_bottom_schools_noTHS9thFig10](https://github.com/AnaMMoreira/School_District_Analysis/blob/main/Resources/top_n_bottom_schools_noTHS9thFig10.png)

## How does replacing the ninth-grade scores affect the following:
## Math and reading scores by grade

Grade averages by grade do not change because no values are affected by the THS 9th grade results.  The 9th grade THS results however are just displayed as NaN

![Insert noTHS9th_MathScoresbyGradeFig11a](https://github.com/AnaMMoreira/School_District_Analysis/blob/main/Resources/noTHS9th_MathScoresbyGradeFig11a.png)

![noTHS9th_ReadingScoresbyGradeFig11b](https://github.com/AnaMMoreira/School_District_Analysis/blob/main/Resources/noTHS9th_ReadingScoresbyGradeFig11b.png)

## Scores by school spending

The Analysis results based on spending-per-student remained unchanged.

![noTHS9th_SpendingSummaryFig12](https://github.com/AnaMMoreira/School_District_Analysis/blob/main/Resources/noTHS9th_SpendingSummaryFig12.png)

## Scores by school size
## Scores by school type

Both the analysis based on school size and school type remained unaffected by the exclusion of the data in question.

![noTHS9th_SizeSummaryFig13](https://github.com/AnaMMoreira/School_District_Analysis/blob/main/Resources/noTHS9th_SizeSummaryFig13.png)

![noTHS9th_TypeSummaryFig14](https://github.com/AnaMMoreira/School_District_Analysis/blob/main/Resources/noTHS9th_TypeSummaryFig14.png)

## Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

 In summary changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs, have very little effect in the overall district based analysis.  However it was noted that the 0.3% might have been sufficient to get the District performance to a benchmark of 65% overall passing proficiency.
In the school summary table figure 9 it can be seen that removing the 9th grade scores lowered the percent passing numbers by approximately 0.3%, 0.1%, and 0.1%, for Overall, math and reading % passing results correspondingly. 
Although Thomas High School did not change its ranking within the district and in comparison with other schools in the district the numbers did change sightly.  The other analysis results remained unchanged.  
