# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 1: Standardized Test Analysis


The SAT and ACT are standardized tests that many colleges and universities in the United States require for their admissions process. This score is used along with other materials such as grade point average (GPA) and essay responses to determine whether or not a potential student will be accepted to the university.

The SAT has two sections of the test: Evidence-Based Reading and Writing and Math (source). The ACT has 4 sections: English, Mathematics, Reading, and Science, with an additional optional writing section (source). They have different score ranges, which you can read more about on their websites or additional outside sources (a quick Google search will help you understand the scores for each test):

-SAT
-ACT

Standardized tests have long been a controversial topic for students, administrators, and legislators. Since the 1940's, an increasing number of colleges have been using scores from sudents' performances on tests like the SAT and the ACT as a measure for college readiness and aptitude (source). Supporters of these tests argue that these scores can be used as an objective measure to determine college admittance. Opponents of these tests claim that these tests are not accurate measures of students potential or ability and serve as an inequitable barrier to entry. Lately, more and more schools are opting to drop the SAT/ACT requirement for their Fall 2021 applications (read more about this here).

### Problem Statement 

As an employee of College Board, I am in a team that analyzes that trends and insights from the data we gathered each year to provide to our executive board. Since this is year 2020, we would like to evaluate the last 3 years SAT score by state and by intended college major to see if there are any key insights we can use to leverage and improve our test.

### Choose your Data

sat_2017.csv: 2017 SAT Scores by State
sat_2018.csv: 2018 SAT Scores by State
sat_2019.csv: 2019 SAT Scores by State
sat_2019_by_intended_college_major.csv: 2019 SAT Scores by Intended College Major


### Data Dictionary for sat_3years dataset
 
|Feature|Type|Dataset|Description|
|---|---|---|---|
|state|object|sat_3years|List of states in the United States| 
|participation_sat2017|float|sat_3years|Percentage of students who took SAT test in 2017|
|total_sat2017|int|sat_3years|Average total SAT score in 2017, range between 400 and 1600| 
|verbal_sat2017|int|sat_3years|Average SAT verbal score in 2017, range between 200 and 800| 
|math_sat2017|int|sat_3years|Average SAT math score in 2017, range between 200 and 800| 
|participation_sat2018|float|sat_3years|Percentage of students who took SAT test in 2018|
|total_sat2018|int|sat_3years|Average total SAT score in 2018, range between 400 and 1600| 
|verbal_sat2018|int|sat_3years|Average SAT verbal score in 2018, range between 200 and 800| 
|math_sat2018|int|sat_3years|Average SAT math score in 2018, range between 200 and 800| 
|participation_sat2019|float|sat_3years|Percentage of students who took SAT test in 2019|
|total_sat2019|int|sat_3years|Average total SAT score in 2019, range between 400 and 1600| 
|verbal_sat2019|int|sat_3years|Average SAT verbal score in 2019, range between 200 and 800| 
|math_sat2019|int|sat_3years|Average SAT math score in 2019, range between 200 and 800| 

### Data Dictionary for sat_major dataset

|Feature|Type|Dataset|Description|
|---|---|---|---|
|intended_major|object|sat_major|Intended college major of the students who took SAT test in 2019|
|participation|float|sat_major|Percentage of students who took SAT test in 2019|
|total|int|sat_major|Average Total SAT score in 2019, range between 400 and 1600| 
|verbal|int|sat_major|Average SAT verbal score in 2019, range between 200 and 800| 
|math|int|sat_major|Average SAT math score in 2019, range between 200 and 800| 


### Conclusion and Recommendations
From our analysis, our SAT test is gaining more participation rate throughout the country. We can observe more positive trends towards SAT participation rate from the histogram as there is an increasing number of states that receive 100% participation scores and many states with low partipation scores show higher percentage in the last two years.

There are 22 states with more than 50% SAT participation rate in all 3 years. However, District of Columbia is the only state among the 4 states with 100% participation rate in 2017 to have negative growth in the following year. Connecticut, Delaware, and Michigan have shown no change in participation rate year-to-year from 2017 to 2019.

In terms of total score by state, Minnesota has earned the highest average total score for year 2017-2019 in the range of 1284-1298. Meanwhile, District of Columbia earns the lowest average total score for year 2017-2018 in the range of 950-977 and West Virginia has the lowest average total score of 943 in year 2019. The scatter plots of Average total SAT scores for 2017 vs 2018 and 2018 vs 2019 show strong positive relationship, indicating no significant changes of average scores for each state between years. Additionally, the Heat map shows that verbal score is positively correlated with math score for each respective year while participation rate is negatively correlated with total score for each respective year.

When looking into the total scores by intended college major (2019 only), we find that the intended college majors with highest SAT scores are those science-related majors such as Mathematics and Statistics, Physical Science, and Social Science. On the other hand, the intended college majors with lowest SAT scores are Mechanic and Repair Technologies/Technicians, Construction Trades, and Personal and Culinary Services. When comparing the total SAT score by state and total SAT score by intended college major, students who want to major in Mathematics are more likely to come from Minnesota and Wisconsin. There's a chance that these states have more students who want to pursue math majors.

Recommendations:

Gather more information on the causes of students performance in SAT in District of Columbia and West Virginia. Deep dive into the resources allocation, school district as such to find a way to improve scores of these states.
Find out the drop in participation rate for District of Columbia. Not only that this state earns low average total score, but it also shows decrease in participation rate over years.
Gather intended college major data by state in order to find out whether there is any correlation between states and intended college major.


