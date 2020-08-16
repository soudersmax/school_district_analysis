# School District Analysis

## Overview

The purpose of this analysis is to provide support to the School District in decision-making and evaluation of school performance and budget across the district. During the analysis, some evidence of academic dishonesty was found, so the analysis was completed again, excluding both math and reading scores of Thomas High School 9th graders. 

## Results

- The district summary doesn't show great change when the academic dishonesty adjustments were made. There is one fewer student "passing" math/reading/overall and the average math grade is slightly lower. 

- When looking at the school summary, Thomas High School drastically changes. As shown below, the percentage of students passing math and reading is greatly decreased, because, while no 9th graders are being counted in these scores, they are still included in the total students count. The average math score decreases slightly, and the average reading score increases slightly. 

  <img src="Resources\school_summary.png" style="zoom:50%;" />

- Replacing the 9th graders scores with "NaN" makes it appear that Thomas High School has a much lower performance and success rate than many of the other schools. Previous to the replacement, Thomas was second in the district, but they are pushed much farther down with the exclusion of the 9th graders.  

- Replacing the ninth-grade scores affects the following:
  - Math and reading scores by grade - The value for Thomas High School's 9th grade math and reading scores has been replaced by "nan" as seen in the figure below (example shows math scores only). 
  
    <img src="Resources\math_by_grade.png" style="zoom:80%;" />
  
  - Scores by school spending - The "bin" containing Thomas High School ($630 - 644) shows drastic changes in the passing percentages
  
    <img src="Resources\per_capita.png" style="zoom: 67%;" />
  
  - Scores by school size - The "bin" containing Thomas High School (Medium (1000 - 2000)) continues to show a decrease in passing percentages, though the value differs due to differing "bin" composition.
  
    <img src="Resources\school_size.png" style="zoom:67%;" />
  
  - Scores by school type - The "bin" containing Thomas High School (Charter) continues to show a decrease in passing percentages, though these appear to be the least drastic of our examples, due again to group composition. 
  
    <img src="Resources\school_type.png" alt="school_type" style="zoom:67%;" />

## Summary

1. Passing Math, reading, and overall percentage decrease by a good amount in every measure

2. Thomas High School is no longer in the Top 5 performing schools in the district

3. Even though it's not visible in most of our tightly formatted DataFrames, Thomas High School's average score for math decreased and average score for reading increased very slightly when looking at more precise measurements. 

4. Thomas High School's 9th grade reading and math scores have been replaced with "nan".

