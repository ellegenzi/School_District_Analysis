# PyCity Schools: School District Analysis

## Overview of Project

### Background and Purpose

Maria is a chief data scientist for the PyCity school district. She has been tasked with preparing all standardized test data for analysis and creating a presentation to provide insights about performance trends and patterns, which will aid the school board and superintendent in making strategic decisions. Maria is requesting help with analyzing this data, especially with updating the data now that it's been revealed there may be evidence of academic dishonesty with the test scores for the 9th graders at Thomas High School.

### Resources

- Data Source: schools_complete.csv, students_complete.csv
- Software: Anaconda 4.13, Python 3.7.6, Visual Studio Code 1.68.1

## Results

### How is the district summary affected?

As shown in Figures 1 and 2, after cleaning up the data to remove the scores from the 9th graders at Thomas High School, the following metrics are affected:

+ The average math score decreases from 79.0 to 78.9.
+ The average reading score does not change and remains at 81.9.
+ The percentage of students passing math decreases from 75.0% to 74.8%.
+ The percentage of students passing reading decreases from 86.0% to 85.7%.
+ The overall percentage of students passing math and reading decreases from 65.0% to 64.9%.

*Figure 1: District Summary Before Cleaning Up Data*
![DistrictSummary_Original](https://user-images.githubusercontent.com/106830513/178169309-330ed3f2-971a-4918-ac18-355f6e667ffe.png)

*Figure 2: District Summary After Cleaning Up Data*
![DistrictSummary_After](https://user-images.githubusercontent.com/106830513/178169406-1c0ec4b8-8732-48f6-8611-a5237c880d6c.png)

### How is the school summary affected?

As shown in Figures 3 and 4 below, the school summary for Thomas High School changes just slightly after cleaning up the data, with the following metrics being affected:

+ The average math score decreases from 83.42 to 83.35.
+ The average reading score increases from 83.85 to 83.9.
+ The percentage of students passing math decreases from 93.23% to 93.19%.
+ The percentage of students passing reading decreases from 97.31% to 97.02%.
+ The overall percentage of students passing math and reading decreases from 90.95% to 90.63%.

*Figure 3: THS Rank Before Cleaning Up Data*
![THSrank_Original](https://user-images.githubusercontent.com/106830513/178170811-4c09ca4d-4450-41fe-939b-342ba147de5b.png)

*Figure 4: THS Rank After Cleaning Up Data*
![THSrank_After](https://user-images.githubusercontent.com/106830513/178170823-5823134e-ff6a-49c1-bebe-b5162fd7e64e.png)

### How does replacing the ninth graders' math and reading scores affect Thomas High School's performance relative to the other schools?

As shown in Figures 3 and 4 above, replacing the 9th graders' math and reading scores only minorly affects Thomas High School's performance. Prior to removing the scores, Thomas High School ranked 2nd in performance compared to the other schools. After removing the scores, Thomas High School remains in 2nd, but by a much smaller margin. They were 0.35% ahead of the 3rd place school, but now are only roughly 0.03% ahead after cleaning the data.

### How does replacing the ninth-grade scores affect the following:
+ Math and reading scores by grade: As shown in Figures 5 through 8, the math and reading scores for THS 9th graders now show "nan." If you averaged the scores for all 9th graders in the district before replacing the scores for THS, the average for math scores was 80.35 and after replacing the scores, the average falls to 80.12. The average reading score for all 9th graders in the district was 82.51 before replacing the scores for THS and after replacing the scores, it falls to 82.43.

*Figure 5: THS Math Scores Before Cleaning Up Data*
![THSmath_Original](https://user-images.githubusercontent.com/106830513/178169659-aec89dfb-b23f-48be-9458-ac2a4604d68b.png)

*Figure 6: THS Math Scores After Cleaning Up Data*
![THSmath_After](https://user-images.githubusercontent.com/106830513/178169669-b4d53748-1d0b-458a-ac13-f328835aebb5.png)

*Figure 7: THS Reading Scores Before Cleaning Up Data*
![THSreading_Original](https://user-images.githubusercontent.com/106830513/178169674-68b13544-10f0-493d-9562-b5826c1d0255.png)

*Figure 8: THS Reading Scores After Cleaning Up Data*
![THSreading_After](https://user-images.githubusercontent.com/106830513/178169684-e3dd9077-0bf3-48cb-8508-bfe705eb651b.png)

+ Scores by school spending: THS is in the spending range of $631-645 per student. As shown in Figures 9 and 10, When rounding to whole numbers, there is no difference in the scores by school spending for this bin. However, as shown in Figures 11 and 12, when expanding out to one decimal place, the % passing reading drops from 84.4% to 84.3% and the % overall passing drops from 62.9% to 62.8%.

*Figure 9: School Spending Before Cleaning Up Data*
![SchoolSpending_Original](https://user-images.githubusercontent.com/106830513/178171598-07831046-26b6-4d8b-a566-c04ac92bafc7.png)

*Figure 10: School Spending After Cleaning Up Data*
![SchoolSpending_After](https://user-images.githubusercontent.com/106830513/178171630-a56ca568-28f0-4b8d-b120-08b89e627c0c.png)

*Figure 11: School Spending Before Cleaning Up Data - Expanded*
![SchoolSpending_Originalpoint1](https://user-images.githubusercontent.com/106830513/178171617-d5d2c99b-903e-4846-9701-a87b1117d893.png)

*Figure 12: School Spending After Cleaning Up Data - Expanded*
![SchoolSpending_Afterpoint1](https://user-images.githubusercontent.com/106830513/178171642-a6a72a7f-ae85-49c5-9de5-ec0048ee8309.png)

+ Scores by school size: THS is in the medium school size bin. As shown in Figures 13 and 14, when rounding to whole numbers, there is no difference in the scores by school size for this bin. However, as shown in Figures 15 and 16, when expanding out to one decimal place, the % passing reading drops from 96.8% to 96.7%.

*Figure 13: School Size Before Cleaning Up Data*
![SchoolSize_Original](https://user-images.githubusercontent.com/106830513/178171805-6365d5c0-7489-4b27-8835-2d786b37758b.png)

*Figure 14: School Size After Cleaning Up Data*
![SchoolSize_After](https://user-images.githubusercontent.com/106830513/178171841-8ec35dc2-f437-4bcd-ad3d-dc0d82682711.png)

*Figure 15: School Size Before Cleaning Up Data - Expanded*
![SchoolSize_Originalpoint1](https://user-images.githubusercontent.com/106830513/178171823-4a0a0c9f-4d5a-405b-a2b6-6485f3b5ffdb.png)

*Figure 16: School Size After Cleaning Up Data - Expanded*
![SchoolSize_Afterpoint1](https://user-images.githubusercontent.com/106830513/178171853-2a22a907-3e9a-4404-b904-10ff0b0b39cb.png)

+ Scores by school type: THS is a charter school. As shown in Figures 17 and 18, there is no difference in the scores by school type for this bin.

*Figure 17: School Type Before Cleaning Up Data*
![SchoolType_Original](https://user-images.githubusercontent.com/106830513/178171865-84aad780-32c6-4377-a8fa-063672041d82.png)

*Figure 18: School Type After Cleaning Up Data*
![SchoolType_After](https://user-images.githubusercontent.com/106830513/178171878-b10a7a13-bfdb-4ed0-9791-c6714c67426d.png)

## Summary
In summary, replacing the scores for the 9th graders at Thomas High School did change the averages, but only by a very small amount. The largest change was the drop in overall passing percentage, which decreased by 0.32%, and was mostly due to the decrease in the passing reading percentage from 97.31% to 97.02%. However, these decreases did not affect Thomas High School's overall standings by performance and they remain in 2nd. Otherwise, the miniscule decreases in average scores for math and reading and their corresponding percentages can be seen throughout the analysis, but these didn't make an impact on the overall bin comparisons for school spending, school size, and school type. This tells us that, in general, Thomas High School students perform similarly in all grades. When the scores for one grade are removed, the averages remain about the same.
