# School_District_Analysis
Week 4 Module 4 PyCitySchools with Pandas

## Overview of the school district analysis:
The purpose of this analysis was to replace the altered datat for Thomas High School and re-run the original analysis looking at the different schools in PyCity. This including looking at overall passing for reading and math by a few different splits such as by grade, school size, school budget, and school type to see if there were any patterns that can help determine where students would be most successful and where there was need for improvemnt. 


### How is the district summary affected?
After Thomas High School was removed, most of the average scores fell by 0.1 - 0.3 percentage points with the biggest impact to the overall passing percentage that went from 65.2% to 64.9%.  Although both codes look identical, after Thomas High School was removed (Revised District Summary), it was simpler to reuse the previous code that already existed to re-run the data frame and reformat, but that the display of the data frame is slightly different confirms that there was a change in the data.  Also, we know from running the student data count that there was over 39,000 students in all of the schools for the PyCity School data  with only 461 students affected for Thomas High School 9th grade. If we divide the Thomas High School 9th graders (461) by the total number of students in all schools (39,170), that works out to 1.17% which is why the scores didn’t change by much. If Thomas High School 9th graders made up a larger proportion of the students, the removal of their data would have caused a larger fluctuation.  

Original District Summary:
![image_name](Resources/school_summary_sorted_original.png)




Revised District Summary:
![image_name](Resources/school_summary_sorted_challenge.png)

### How is the school summary affected?
type analysis here

Original School Summary:
![image_name](Resources/school_summary_sorted_original.png)

Revised District Summary:
![image_name](Resources/school_summary_sorted_challenge.png)


### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
  - Math and reading scores by grade
  - Scores by school spending
  - Scores by school size
  - Scores by school type

## Summary: Summarize four major changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
