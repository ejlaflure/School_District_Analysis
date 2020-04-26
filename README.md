# School_District_Analysis
Analysis of school district grades using Python, Pandas and Jupyter Notebook in order to organize the data more efficiently. 

## Project Overview
Deliverables requested for the analysis of the school district: 
- A high-level snapshot of the district's key metrics, presented in a table format
- An overview of the key metrics for each school, presented in a table format
- Tables presenting metrics for: 
  - Top 5 and bottom 5 performing schools:
    - Overall passing rate
    - The average scores received by students in each grade level at each school
  - School Performance
    - Budget per student
    - School size
    - Type of school

## Project Summary
- District's key metrics

![District's key metrics](https://github.com/ejlaflure/School_District_Analysis/blob/master/project_tables/District's%20key%20metrics.PNG)
- Key metrics for each school

![Key metrics for each school expanded](https://github.com/ejlaflure/School_District_Analysis/blob/master/project_tables/Key%20metrics%20for%20each%20school%20expanded.PNG)
- Top 5 performing schools, based on the overall passing rate 

![Top 5 performing schools, based on the overall passing rate](https://github.com/ejlaflure/School_District_Analysis/blob/master/project_tables/Top%205%20performing%20schools%2C%20based%20on%20the%20overall%20passing%20rate.PNG)
- Bottom 5 performing schools, based on the overall passing rate 

![Bottom 5 performing schools, based on the overall passing rate](https://github.com/ejlaflure/School_District_Analysis/blob/master/project_tables/Bottom%205%20performing%20schools%2C%20based%20on%20the%20overall%20passing%20rate.PNG)
- Top 5 average math score received by students in each grade level at each school 

![The average math score received by students in each grade level at top schools](https://github.com/ejlaflure/School_District_Analysis/blob/master/project_tables/The%20average%20math%20score%20received%20by%20students%20in%20each%20grade%20level%20at%20top%20schools.PNG)
- Bottom 5 average math score received by students in each grade level at each school 

![The average math score received by students in each grade level at bottom schools](https://github.com/ejlaflure/School_District_Analysis/blob/master/project_tables/The%20average%20math%20score%20received%20by%20students%20in%20each%20grade%20level%20at%20bottom%20schools.PNG)
- Top 5 average reading score received by students in each grade level at each school 

![The average reading score received by students in each grade level at top schools](https://github.com/ejlaflure/School_District_Analysis/blob/master/project_tables/The%20average%20reading%20score%20received%20by%20students%20in%20each%20grade%20level%20at%20top%20schools.PNG)
- Bottom 5 average reading score received by students in each grade level at each school 

![The average reading score received by students in each grade level at bottom schools](https://github.com/ejlaflure/School_District_Analysis/blob/master/project_tables/The%20average%20reading%20score%20received%20by%20students%20in%20each%20grade%20level%20at%20bottom%20schools.PNG)
- School performance based on the budget per student 

![School performance based on the budget per student](https://github.com/ejlaflure/School_District_Analysis/blob/master/project_tables/School%20performance%20based%20on%20the%20budget%20per%20student.PNG)  
- School performance based on the school size 

![School performance based on the school size](https://github.com/ejlaflure/School_District_Analysis/blob/master/project_tables/School%20performance%20based%20on%20the%20school%20size.PNG)  
- School performance based on the type of school 

![School performance based on the type of school](https://github.com/ejlaflure/School_District_Analysis/blob/master/project_tables/School%20performance%20based%20on%20the%20type%20of%20school.PNG)  

## Challenge Overview
The grades of the ninth graders at Thomas High School have been changed. After assessing the situation with the school superintendent and Maria, you decide the best approach is to:
- Replace the ninth-grade math and reading scores from Thomas High School.
- Keep all other data associated with the ninth-grade students and Thomas High School intact.

The goals of this challenge are for you to:
- Filter DataFrames using logical operators.
- Replace the incorrect values with NaN.
- Explain how your PyCitySchools analysis changes after you handle the incorrect data.  

## Challenge Summary
Post grade correction analysis:

- Effect on District Summary
  - Looking at a broad summary of data like this, only a slight change is noticeable.  The average math score went down 0.1, while all three percentages went down 1%. 
- Effect on School Summary
  - Since this table shows all the schools separately, the change from the score correction is much more dramatic. The average math score was only lowered by 0.06 and the reading score actually increased by 0.05. Since these are averages, the effected scores were removed from this calculation. This is why the averages are only effected very slightly. The passing percentages on the other hand are greatly affected. The reason for this is that every single ninth grader in Thomas High School has now failed reading and math. The overall passing percentage of the school decreased by 25.87%, while the passing percentages for math and reading decreased by 26.36% in math and 27.65% in reading. This lines up with about a fourth of the student population now failing because the whole grade’s scores are no longer valid. 
- Thomas High School’s performance relative to the other schools in district
  - Thomas High School’s performance in comparison to the other schools in the district was greatly affected, by the change in scores. Surprisingly, even with a whole grade failing, Thomas High School is not the worst performing school in the district. Thomas High School went from being the second best performing school in the district to being ranked eighth among the 15 schools. 
- Effect on Math and Reading Scores by Grade
  - Since only the ninth grade scores at Thomas High School were changed, the changes that occurred was Thomas High School 9th grade cell changed to NaN in both the math scores by grade table and reading scores by grade table.
- Effect on Scores by School Spending
  - Since Thomas High School is the $630-644 range of spending, only this budget range was affected by the change in data. The average math and reading scores were not affected by the change in data similar to those columns when the data was distributed by schools. Passing percentages, on the other hand, was greatly affected for this spending range. The $645-675 spending range still performs worse in Math and overall, but in reading the $630-644 spending range is now the worst performer. All three percentages is the spending bracket decreased by about 7% from the change. 
- Effect on Scores by School Size
  - Thomas High School is a medium sized school, so only this size of school was affected by the change in data. Just like with the school spending distribution, the average scores in the school size distribution was not affected by the change. The passing percentages for medium schools decreased by 6%. This takes medium schools from being the best performer out of the three school sizes. Small schools now perform the best while large schools still perform the worst.
- Effect on Scores by School Type
  - Similar to School spending and size, since Thomas High School is a Charter school, that type of school was affected. Just like with school spending and size, the average scores were not affected by the change in data. Percent passing in math and reading decreased by 4% while overall decreased by 3%. Charter school, even with this change, still perform vastly better then District schools. 
