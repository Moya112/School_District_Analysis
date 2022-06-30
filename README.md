# School_District_Analysis

## Project Overview
A school board has requested a data analysis of a school district based on funding and student grades. This analysis would be to learn new insights and visually provide precise results on each school's performance. 

1. Calulate average math score received by students in each grade level at each school.
2. Determine the top 5 and bottom 5 performing schools, based on the overall passing rate.
3. Caluclate the average reading score received by students in each grade level at each school.
4. Determine the school performance based on the budget per student, school size, and type of school.

## Resources
- Data Source: PyCitySchools.ipynb
- Software: Python 3.10.5, Jupyter Notebook


## Challenge Overview
 Due to potential academic dishonesty, specifically in reading and math, grades for Thomas High School ninth-graders appear to have been altered. Therefore, to uphold state-testing standards, the school board requested Maria's team to conduct a second analysis of the data by replacing the reading and math scores for Thomas High School with NaNs while keeping the rest of the data intact.
 
 
 ## Resources
- Data Source: PyCitySchools_Challenge.ipynb
- Software: Python 3.10.5, Jupyter Notebook

## Results
The first trial of this analysis includes the complete set of student data. In the second trial of this analysis, the ninth-grade students of Thomas High School had their scores omitted from the calculations. Therefore, the entire ninth-grade class of Thomas High School has had their scores replaced with NaN.
<img width="922" alt="district_overview" src="https://user-images.githubusercontent.com/105765150/176584110-31a72f1c-61c2-4197-bf4c-2fc5baa7b746.png">

The following changes occurred for Thomas High School after replacing the ninth graders' math and reading scores with NaN:
1. The overall passing percentage for Thomas High School fell to 65%.
2. The overall passing percentage for the entire district fell to 64.9%.
3. Thomas High School was no longer included on the list of top five schools.

When the ninth graders' of Thomas High School had their scores omitted from the calculations, the following changes occured:
1. The overall passing percentages of Thomas High School decreased by 0.11%.
2. The average scores of Thomas High School for math and reading increased by 0.06.
3. For the spending range of $630-644 per student, the overall passing percentage decreased by 0.1%.
4. School rankings are unchanged. Thomas High School is still the second best performing school in the district with an overall passing rate of 90.63% among their tenth through twelfth graders.

## Effects of the School Budget and School Size

The  Average Scores and Passing Percentages do not increase as spending per student increases. For example, Cabera High School, the top-performing school in the entire school district, received $68 less per student than Johnson High School, the lowest-performing school, implying that more relevant factors than funding decide average student scores.
<img width="842" alt="school_budget_per_student_df" src="https://user-images.githubusercontent.com/105765150/176585776-88657685-0820-42df-a4be-0cd25575a7c7.png">

Considering the size of a school, larger schools with over 2,000 students have the lowest average scores and passing percentages. However, the difference in performance between small and medium-size schools is imperceptible at approximately 1%. Fort this dataset, the district schools Large, which suggested that students in this district learn and perform better in smaller, more intimate settings.
<img width="767" alt="school_size_df" src="https://user-images.githubusercontent.com/105765150/176586362-9d2da473-65c1-4aa2-be6e-f5bfdf24cedd.png">

## Charter Schools vs. District Schools
The analysis suggested that charter schools performed better than district schools. The top five schools with the highest overall passing percentages are Charter schools, whereas the bottom five are all District Schools. Charter schools have a 36% higher overall passing rate than district schools. 
.<img width="719" alt="school_type_df" src="https://user-images.githubusercontent.com/105765150/176586657-b38f09b8-43c1-4110-875c-9a7d9ab5e514.png">

## Summary
It is unfeasible to determine the extent of the potential academic dishonesty or identify specific individuals to exclude from the dataset. As a result, the entire ninth grade of students from Thomas High School has had their scores excluded from the results. Replacing the ninth graders' scores with NaN caused Thomas High School's overall passing percentages and average scores to decrease. As a result, the district has had its average math, and reading scores plummet, as well as the overall passing rate for students. In addition, Thomas High School lost its placement as a top-five school within the district. However, Thomas High School's average scores improved and retained its position as the number two school in the district after updating the total student counts and removing their scores from the dataset. 
