# School_District_Analysis
Week 4 Module 4 PyCitySchools with Pandas

## Overview of the school district analysis:
The purpose of this analysis was to replace the altered data for Thomas High School and re-run the original analysis looking at the different schools in PyCity. This included looking at overall passing for reading and math by a few different splits such as by grade, school size, school budget, and school type to see if there were any patterns that can help determine where students would be most successful and where there was need for improvement. 


### How is the district summary affected?
After Thomas High School was removed, most of the average scores fell by 0.1 - 0.3 percentage points with the biggest impact to the overall passing percentage that went from 65.2% to 64.9%.  Also, we know from running the student data count that there was over 39,000 students in all of the schools for the PyCity School data  with only 461 students from Thomas High School 9th grade that were removed. If we divide the Thomas High School 9th graders (461) by the total number of students in all schools (39,170), that works out to 1.17% which is why the scores didn’t change by much. If Thomas High School 9th graders made up a larger proportion of the students, the removal of their data would have caused a larger fluctuation.  

**Original District Summary:**
![image_name](Resources/school_summary_sorted_original.png)




**Revised District Summary:**
![image_name](Resources/school_summary_sorted_challenge.png)

### How is the school summary affected?
While overall the removed Thomas High School data did not have much impact, it did on the individual school level. Originally, Thomas High School was the second highest overall passing school in the original data frame, but once the 9th graders were removed, the school fell to the 8th highest overall passing, falling from 90.95% to 65.08%. The removal of the 9th graders scores heavily impacted Thomas High School’s passing rate, but not enough to send them to the very bottom of the list which means that even without 9th grade’s inflated scores, Thomas’s high school students’ are not less likely to get a passing grade. 

**Original School Summary:**
![image_name](Resources/school_summary_sorted_original.png)

**Revised School Summary:**
![image_name](Resources/school_summary_sorted_challenge.png)


### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
**Math Scores by Grade** <br />
In the original data frame, Thomas High School was third highest school among 9th graders. After the 9th graders were removed and the score was replaced with NaN, they lost their position.  As expected no other grades were impacted for Thomas High School. While they do not have the very highest average for math scores by grade, they tend to be a school close to the median scores for each grade with the 12th graders being highest compared to the other schools, but the average math score for Thomas High School’s 11th and 12th graders are nearly identical at 83.5 for both grades. <br />
  
 
   * Math Score by Grade Original <br />
    ![image_name](Resources/Math_Score_by_Grade_Original.png)  <br />
   * Math Score by Grade Challenge <br />
  ![image_name](Resources/Math_Score_by_Grade_Challenge.png)  <br />
    



  **Reading Score by grade**  <br />
  
Thomas High School 9th graders had the fourth highest average among the schools before their data was cleaned out. Similar to the Math score averages, the other grades were not affected after the 9th grade data clean for Thomas. Thomas High School is tied with Caberera High School for the average reading score for 10th graders, but has the seventh highest average reading score for their 11th and 12th graders. This tells us that even though the Thomas High School 9th graders were helping increase Thomas’s overall position compared to other schools, their 10th grade reading scores are also contributing. 

   * Reading Score by Grade Original <br />
    ![image_name](Resources/Reading_Scores_by_Grade_Original.png)  <br />
   * Reading Score by Grade Challenge <br />
  ![image_name](Resources/Reading_Score_by_Grade_Challenge.png) <br />

  
 **Scores by school spending**  <br />
 
 Although Thomas High School 9th graders were removed, the spending buckets included were large enough that the impact was minimal at best, affecting the hundreths of a decimal place.  Re-running the dataframe looked identical unless looking at unformatted data to spot the differences. I can confidentally say at a topline level that removing Thomas High School's 9th graders did not affect the scores by school spending. What I can tell from looking at the school by spend is that  Thomas High School was in the $630-644 range since that was the only row to show the hundredth decimal place changes. 
 
   * Original Scores by Spend <br />
     ![image_name](Resources/Scores_by_Spending_Original.png) <br />
   * Challenge Scores by Spend <br />
     ![image_name](Resources/Scores_by_Spend_Challenge.png) <br />

  **Scores by school size**  <br />
  
  A slight decrease in the range from 0.01 - 0.07 with the largests impacts to percentage passing reading by (-0.06) and the percentage of overall passing by (-0.07) for the Medium (1000 - 2000) school size. Medium schools continue to have the highest overall passing rate at 91%, but small schools are just slightly behind at 90% overall passing rate. Medium school sizes edge small schools for passing rate due to their higher reading scores, 97% comapred to 96% with math scores identical at 94%. Larger schools have the lowest overall passing rate at 58% with also the lowest reading score passing rate (83%) and lowest math score passing rate (70%). 
  
   * Original Scores by Size <br />
     ![image_name](Resources/Scores_by_Size_Original.png) <br />
   * Challenge Scores by Size <br />
     ![image_name](Resources/Scores_by_School_Size_Challenge.png) <br />
     
  **Scores by school type**  <br />
  
  Charter schools have a higher passing rate than District schools for all passing rates, but the difference is most prevlant in math scores where Charter has a 94% passing rate compared to District schools' 64% passing rate. The removal of Thomas High School 9th Graders had no impact on the dominating performance of Charter over District schools in all categories.

   * Original Scores by Type <br />
     ![image_name](Resources/Schools_by_Type_Original.png) <br />
   * Challenge Scores by Type <br />
     ![image_name](Resources/Scores_by_Type_Challenge.png) <br />

## Summary: 
Overall, a student has the best chance of passing reading and math if they are in a medium-small sized student population, where per student spending is less than $584, and is a Charter school. Holden High School's 12th graders have the highest chance of passing reading at 84.7% and their 11th graders have the best chance to pass math with an 85% math pass rate. Consistent with the previous school district analysis including the Thomas High School 9th grader reading and math scores the overall analysis was not impacted. While on an individual school analysis the removed scores dropped Thomas High School from a top to bottom perfomerer.

