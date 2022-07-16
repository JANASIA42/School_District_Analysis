# School_District_Analysis

## Overview
The purpose of this analysis was to improve the integrity of the school district analysis, after discovering that Thomas Highschool's ninth graders' math and reading scores may have been compromised/altered, by removing those scores and replacing them with non-numbers.  We then used the "clean" data to repeat the analysis and improve it's accuracy.


## Results
### How is the district summary affected?
- The Average Math Score in the updated district summary dropped by 0.1 point.
- The Average Reading Score was unchanged.
- The percentage of students who passed math dropped by 0.2%.
- The percentage of students who passed reading dropped by 0.1%.
- The overall percentage of passing students dropped by 0.3%.

Unscrubbed district summary:
![image](https://user-images.githubusercontent.com/106359572/179361398-b7d9b222-5afe-434e-9e95-a7d4c635c07e.png)

Scrubbed district summary:
![image](https://user-images.githubusercontent.com/106359572/179361476-9a05f9cd-60ef-40cc-b739-89e567a336d6.png)


### How is the school summary affected?
The only changes to the school summary were for Thomas High School.  Their average reading and math scores did not change significantly (by less than a percentage point), but their percentages for passing math and reading scores plummeted from 93.27% to 66.91%, and from 97.31% to 69.66%, respectively.  Their overall percentage of students who passed both math and reading fell from 90.95% to 65.08%.

Unscrubbed school summary:
![image](https://user-images.githubusercontent.com/106359572/179361972-3c843a92-ecff-4335-b752-228c71dfbaf7.png)

Scrubbed school summary:
![image](https://user-images.githubusercontent.com/106359572/179361625-cec2c17c-7ea5-4759-81c4-f3148c5d2fef.png)

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
In the school summary created with the inaccurate ninth grade scores, Thomas Highschool placed second-best in Overall passing percentage (at approximately 91%).
The analysis that took into account and excluded the false scores shows Thomas as placing 8th (so, the median), with their updated Overall passing percentage of 65.08.

### How does replacing the ninth-grade scores affect the following:
- Math and reading scores by grade:

Math and reading scores by grade were removed from the 9th grade column for Thomas High School and were therefore not included in the analysis results.

![image](https://user-images.githubusercontent.com/106359572/179367012-03d3d750-0de1-46ae-b3ed-28f2f4494ed1.png)
![image](https://user-images.githubusercontent.com/106359572/179367065-41051257-3c3d-45cb-a8c7-0b8a8b667b76.png)

- Scores by school spending:

Scores by school spending were not significantly impacted (less than a tenth of a percent in each metric):

Unscrubbed scores by spending DataFrame:

![image](https://user-images.githubusercontent.com/106359572/179367645-7668aefe-5e97-46b5-8c80-5af03486a5e2.png)

Scrubbed scores by spending DataFrame:
![image](https://user-images.githubusercontent.com/106359572/179367668-650a1540-ab26-438b-b1c0-42b411bd0cbd.png)

- Scores by school size:

Impact on scores by school size was about as insignificant as scores by spending (again, less than a tenth of a percent difference).  The only impact was to the mid-size category (between 1,000 and 1,999 students), as Thomas is in this size category and their data was the only school data that changed.

Unscrubbed scores by school size:
![image](https://user-images.githubusercontent.com/106359572/179367973-11df5da7-a265-4715-bdd7-c31cae67b0e6.png)

Scrubbed scores by school size:
![image](https://user-images.githubusercontent.com/106359572/179368018-a6b8e7ec-b98c-4430-9fad-b4fad2148201.png)

- Scores by school type

As with the scores by spending and size, impact to scores by school type was also not significant.

Unscrubbed scores by school type:
![image](https://user-images.githubusercontent.com/106359572/179368127-e156ee24-7a44-43f7-a863-72b57cb701a0.png)

Scrubbed scores by school type:
![image](https://user-images.githubusercontent.com/106359572/179368195-f3d8f77c-9428-404e-ae5d-e27432d03a9d.png)


## Summary 
### Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

1. The biggest change after Thomas High school ninth grade math and reading scores were removed was to their placement in overall performance relative to the other schools, which went from being in the top two, to just average (8th place out of 15 schools).

2. The other major change was to Thomas High School's overall passing score, which dropped sharply from around 91% to approximately 65%.

3. The school summary now no longer includes the potentially falsified Thomas High School ninth grade math and reading scores.

4. The least significant change was to the outcome of the analysis; none of the scores by type, size or spending categories changed noticeably as a result of removing the ninth grade THS scores.



