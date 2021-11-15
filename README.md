# School District Analysis

## Overview
As a result of possible altered reading and math grades belonging to the 9th graders at Thomas High School, I have repeated the original analysis I conducted for schools in the district, but this time around I have nullified the math and reading scores for the 9th graders at Thomas High.  I will then determine how the new scores have affected the original results by comparing the data frames in this analysis to the original data frames.

## Results

[Modified Analysis](https://github.com/MaxV6ft4/School_District_Analysis/blob/main/PyCitySchools_Challenge.ipynb)

- The District Summaries were near identical.  Only the average math score changed, dropping by 0.1 from 79.0 to 78.9.
- The School Summaries, however, contained greater changes in values pertaining to Thomas High.
  - the average math score went down by 0.067412
  - the average reading score went up by 0.047152
  - the percentage of students passing math went down by 0.086481%
  - despite the average reading score increasing, the percentage of students passing reading went down by 0.29013%
  - finally, the overall passing percentage went down by 0.317688%
- Despite all values decreasing, save the average reading score, Thomas High School remains in second place for the total number of students passing both reading and math in the school district.
- By removing the 9th grade reading and math grades at Thomas High, its score becomes null (nan means "not a number") in the 9th grade column of the scores per grade data frame.  Otherwise, the data frame does not change.
- Thomas High School spends $638 per student.  The values that changed in the data frame for school spending are therefore located in the $630-$644 index.  
  - Before formatting to display the number with a single decimal point, the average math score went down by 0.016853 and the average reading score went up by 0.011788.  After formatting, the average scores remained at 78.5 and 81.6, respectively.
  - Before formatting to display a whole number, the percentage of students passing math went down by 0.02162%, the percentage of students passing reading went down by 0.072532%, and the overall student passing percentage went down by 0.079423%.  After formatting, the percentages remained at 73%, 84% and 63%, respectively.
- Thomas High School has a total of 1635 students.  Therefore, the values that changed in the school size data frame are located in the Medium(1000-2000) index.
  - Before formatting to display the number with a single decmial point, the average math score went down by 0.013483 and the average reading score went up by 0.009431.  After formatting, the average scores remained at 83.4 and 83.9, respectively.
  - Before formatting to display a whole number, the percentage of students passing math went down by 0.017297%, the percentage of students passing reading went down by 0.058026%, and the overall passing percentage went down by 0.063538%.  After formatting, the percentages remained at 94%, 97%, and 91%, respectively.
- Thomas High School is a charter school.  Therefore, the values that changed in the school type data frame are located in the Charter index.
  - Before formatting to display the number with a single decimal point, the average math score went down by 0.008427 and the average reading score went up by 0.005894.  After formatting, the average scores remained at 83.5 and 83.9, respectively.
  - Before formatting to display a whole number, the percentage of students passing math went down by 0.01081%, the percentage of students passing reading went down by 0.036266%, and the overall passing percentage went down by 0.039711%.  After formatting, the percentages remained at 94%, 97%, and 90%, respectively.

## Summary
After replacing the 9th grade reading and math scores at Thomas High with NaNs, I have observed a few changes in the data frames.  The average math score has decreased at Thomas High, which in turn has decreased the average math score for the entire district.  Also, the average reading score has increased at Thomas High, which in turn has increased the average reading score for schools that spend between $630-$644 per student, schools that contain between 1000-2000 students and schools that are charter schools. The overall percentage of students passing both math and reading decreased at Thomas High, resulting in a decrease in the district passing percentage for the same three categories ($630-644 per student, 1000-2000 students attending and schools of the charter type).  Finally, Thomas High School remains in the second-highest position amongst all schools in the district for students passing both math and reading, despite the decrease in percentage.

Most importantly, however, I noticed that once the data had been formatted in the frames displaying results based on school spending, school size and school type, the above changes in both average scores and percentages of students passing math and reading were erased.  It is only when the numbers contain many decimal points that a difference in scores and percentages is visible.
