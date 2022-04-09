# School_District_Analysis
Analysis of school math and reading testing was done to clean data and analyze overall scores by school, school type, and budget per student.

##**Resources**
Data Sources: students_complete.csv, schools_complete.csv
Software: Python 3.9.7, Jupyter Notebook 6.4.0

##**Overview**
Standardized test data from 15 schools was collected for math and reading for analysis of performace trends. Trends identified would be used for discussion of factors influencing test schools such as school budget and budget per student alloted and factored into future budget allotments. The data was cleaned for improper names and falsified test scores which were found in the data for Thomas High Schools 9th grade students. This data was removed to prevent skewing of overall results of analysis. DataFrames within Pandas were then created to show relation between passing percentages and grade, school type, overall budget, and budget per student. Bins were created to depict which range of budget per student performed best. Data was analyzed in accordance wit FERPA to protect students identities and scoring results.  
##**Results**
- District Summary
  -The 9th grade students were removed from total student count due to altered test scores, thus lowering the total number of students in the district summary as shown below. Since the passing math, reading, and overall is calculated based on the total number of students these amounts would increase since the total number of students decreased. Total schools and school budgets remained unaffected.
  
  
![District_summary](https://user-images.githubusercontent.com/100040705/162583871-9dc5e2a3-a5ef-40be-8fea-922520d71bfe.png)

- School Summary
  - With removal of 9th grade Thomas High School students scores the school summary information for this school changed, but other remained the same. Thomas High Schools passing percentages for math, reading, and overall greatly increased with the removal of innaccurate 9th grade scores. The increase for Thomas High school scores is as follows:
    - % Passing Math increased from 66.9% to 93.1%
    - % Passing Reading increased from 66.7% to 97.0%
    - % Overall Passing increased from 65.1% to 90.6%
Results for final school summary data is shown below:


![School_summary](https://user-images.githubusercontent.com/100040705/162584139-14f6d635-51c7-4f8b-904f-263058fd6212.png)

- Replacing 9th graders' math and reading scores increased Thomas High School's performance overall, and its performance relative to other schools. With percent passing above 90% in all catefories it outscores all district schools and is similar to passing percentages of other charter schools analyzed. With the replaced scores Thomas High School ranks second in scores overall, as shown below.


![top_schools](https://user-images.githubusercontent.com/100040705/162584284-3dcfddcf-007e-460b-ace8-a689a0f9734d.png)

- Replacement of Thomas High School 9th grade scores affected the following:
  - Math and reading scores by grade were affected by replacement of 9th grade scores by "NaN" to communicate a lack of scores in this area without affecting other data with deletion. Other grades were unaffected as they were not editted. Results for math and reading scores by grade are as follows:
Math scores by grade:

![math_scores_by_grade](https://user-images.githubusercontent.com/100040705/162584713-a65231f6-f3d2-41fa-bf8d-b0bec88be629.png)

Reading scores by grade:

![reading_scores_by_grade](https://user-images.githubusercontent.com/100040705/162584721-d5fcaf94-fc1e-48c2-a35b-0a19ed916ea3.png)

  - Scores by school spending was affected only in the $646-675 spending range as Thomas High School has a budget of $683 per student putting them in this category. As Thomas High Schools percentage passing for math, reading, and overall was raised by the removal of the 9th grade skewed data, this spending ranges passing percentages were also raised with the increased scores. Results for scores by school spending are as shown below:


![school_scores_by_spending](https://user-images.githubusercontent.com/100040705/162584821-fc85b4cb-e75f-4be0-8eb2-0a2ff5de62cc.png)

  - Scores by school size was affected only in the medium (1,000-1,999) school size range as Thomas High School has 1,635 students. The passing percentage for math, reading, and overall was raised by the removal of Thomas High School 9th graders because these percentages were raised for Thomas High School with the removal, therefore raising the average of this range. Results for scores by school size are as follows:


![scores_by_school_size](https://user-images.githubusercontent.com/100040705/162585070-4fcff912-f491-4477-a51d-51acf013d13c.png)


  - Scores by school type was similarly affected as described above. Since Thomas High School is a Charter school the percentage passing math, reading, and overall was raised by the removal of 9th grade Thomas High School students has this raised those scores for Thomas High School itself which lies within this category. Results for scores by school type are depicted below:


![scores_by_school_type](https://user-images.githubusercontent.com/100040705/162585014-0e9e6a11-7072-4566-8a63-5ca5fc4c1df5.png)

##**Summary**
After the school district analysis was updated by replacement of inaccurate scores for 9th grade students at Thomas High School with NaNs, four major changes can be identified. The first being the drastic increase (around 30% for each) in Thomas High Schools passing percentage for reading, math, and overall(passing of both). Second, this then affected analysis of scores by school type, with charter schools passing percentages increasing due to Thomas High School falling within this category. Third, scores by school size were additionally affected as Thomas High School falls within the medium scores size and its increasing in passing percentages increased the passing percentages within this range. And lastly the scores by school spending was affected as Thomas High School falls within the largest spending category, $646-675, increading the passing percentages within this range. Additionally the school ranking were affected as the refined school district data placed Thomas High School second overall out of all schools analyzed by overall poassing percentages. The cleaned data and refined results will allow for the most accurate results to be analyzed and thus the best conclusions to be made about future budget allotments and the best school conditions for high passing percentage results. 
