# pandas-challenge
Contributor: Cassia Yoon  

-Assignment:
You are the new Chief Data Scientist for your city's school district. In this capacity, you'll be helping the school boardand mayor make strategic decisions regarding future school budgets and priorities.
As a first task, you've been asked to analyze the district-wide standardized test results. You'll be given access to everystudent's math and reading scores, as well as various information on the schools they attend. Your task is to aggregatethe data to showcase obvious trends in school performance. In this assignment, you’ll create and manipulate Pandas DataFrames to analyze school and standardized test data.

The Analysis:  
My script analyzes budget and standardized test scores from various high schools within a district. From the raw test score data, it calculates additional metrics including average scores and student passing percentages (broken down by math, reading, and overall score). From the raw budget data, it calculates per capita budget. Then, the data and calculations are filtered/grouped and sorted in various configurations to facilitate analysis; the configurations include: summary of all data from the whole school district,  summary by school, top and bottom 5 performing schools based on % overall passing scores, math and reading scores grouped by school grade (grades 9 - 12), summary of scores by school spending ranges, scores by school size, scores by school type (charter vs district).  

Conclusions:  
Students from charter schools score higher on standardized tests based on three different analysis tables. The top 5 performing schools are all charter schools (see dataframe <top_schools>). The bottom 5 performing schools are all district schools, none are charter schools (see dataframe <bottom_schools>). The table comparing scores by school type (see dataframe <type_summary>) show that the average test scores and passing rates from charter schools are higher than the averages and percentages from district schools in all categories.

Passing rates may be correlated with school size. Based on the summary of scores by school size  (see dataframe <size_summary>), the average test scores and passing percentages were highest in medium sized schools (1000-2000) except for in average math score, which was slightly higher in small sized schools (by around 0.5). Overall, the average scores and passing rates from small schools were slightly lower than those from medium sized schools. The scores and passing rates from large size schools (2000-5000) were lower than their smaller counterparts all across the board. Upon closer inspection of the table of all the schools' scores by school size  (see dataframe <per_school_summary>), all large schools except for one have an overall passing rate in the low 50s. In contrast, the passing rates from small and medium sized schools were between 89 to 92 percents. However, the table also shows that all small and medium sized schools are all charter schools. In addition, the one outlier large school, the only large school that had a high passing rate, is also a charter school. All the other large schools were district schools and had a low overall passing rate. 

It is also difficult to determine whether the school size affects passing rates due to a large difference in sample sizes; there are only two small sized schools and more than half the schools are large sized. This decreases how meaningful the results from the small to medium sized schools are. In contrast, the sample sizes of school types (8 charter schools vs 7 district schools) are more comparable, making the correlation between school type and passing rates more reliable. Further consideration should be made for expanding the analysis to include multiple districts and obtaining more comparable sample sizes of different school sizes.

Resources:
- https://stackoverflow.com/questions/32464280/converting-currency-with-to-numbers-in-python-pandas
- https://stackoverflow.com/questions/34338374/pandas-control-new-column-names-when-merging-two-dataframes
- https://www.appsloveworld.com/pandas/100/196/how-do-i-remove-square-brackets-from-my-dataframe
- https://stackoverflow.com/questions/29765548/remove-index-name-in-pandas
- https://gitlab.com/farzadkhatoonabadi/PyCitySchools/-/blob/master/PyCitySchools.ipynb?ref_type=heads


Thank you to my bootcamp instructors, TAs, and classmates.