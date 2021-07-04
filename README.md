# School_District_Analysis
*School Analysis*

## Overview of the Project
The project is to utilize rough raw data from two csv files of School and Student data and produce meaningul measures for decision making.  

### Purpose 
The purpose of this analysis is to show trends in school performance, the analysis focuses on the following: 
1)  The **district summary**
2)  The **school summary**
3)  The **top 5 and bottom 5 performing schools** based on the overall passsing rate 
4)  The **average math and reading scores for each grade level** (9th, 10th, 11th, 12th)
5)  The **math and reading scores grouped** by the following:
    - Spending ranges per student
    - School Size
    - School Type
The analysis will be used by the school board and superintendent in making decisions regarding school budets and priorities.   

### Background 
The data is gathered in two different csv files 1) School Data 2) Student Data.  This is raw data that has to be transformed to develop meaningful charts and reports.  
The steps performed is called "data wrangling" and includes loading, reading, inspecting, & cleaning the data.    
After the data is clean we merged datasets and performed calculations to create tables.  Formatting was applied with sorting and grouping to display a   
comprehensive story.

### Resources
- Data Source: 
  - [schools_complete.csv](Resources/schools_complete.csv)
  - [students_complete.csv](Resources/students_complete.csv)

## Results 
The first analysis exercise utlized an original set of data for all the high schools. Many summaries were developed.  
The primary tools were 2 data frames shown below using the info() function 

 ![Student_Data_df](https://github.com/mjrotter4445/School_District_Analysis/blob/main/Graphics/student%20data%20df%20info.png)



 ![School_Data_df](https://github.com/mjrotter4445/School_District_Analysis/blob/main/Graphics/school%20data%20df%20info.png)


Early on, we were able to provide many useful summaries like overall summaries of the 15 schools with average score infomation and more:  

 
![overall summary](https://user-images.githubusercontent.com/84689107/124357382-66db5080-dbd8-11eb-99a6-3e934706aba2.png)
 
 

Later in the process of development and analysis, it was realized that the Thomas High School 9th grade scores were tampered with.  We used the programming
(loc) method to isolate Thomas High School 9th grades scores in both math and reading and we replaced these scores with no value or Nans. 
This change significantly changed the passing scores and percentages results and summaries.  



School Summary Before and After 

![School Summary before and after](https://github.com/mjrotter4445/School_District_Analysis/blob/main/Graphics/school%20summary%20before%20and%20after.png)


District Summary Before and After 
![District Summary before and after](https://github.com/mjrotter4445/School_District_Analysis/blob/main/Graphics/district%20summary%20before%20and%20after.png)

  
  
For further analysis, we provided statistics about the 5 top and bottom performing schools.  

![top](https://github.com/mjrotter4445/School_District_Analysis/blob/main/Graphics/top%205%20perf%20school.png)

 
 
 
 
![bottom](https://github.com/mjrotter4445/School_District_Analysis/blob/main/Graphics/bottom%205%20perf%20school.png) 
 
 
 
 
 
 
 In addition, budgetary information was also reported.  For example, the spending ranges per student provided helpful information.  
 We used "bins" and "spending ranges" to determine school spending per student by school.  Below is an example of a summary. 
 
 ![spending ranges by school](https://github.com/mjrotter4445/School_District_Analysis/blob/main/Graphics/spending%20ranges%20per%20student.png) 
 
 In addition, budgetary information was also reported.  For example, the spending ranges per student provided helpful information.   
 
 ![avg score by school type](https://github.com/mjrotter4445/School_District_Analysis/blob/main/Graphics/avg%20scores%20by%20school%20type.png)  
 
 
 
 
## Summary 
Overall, the amount of useful information that could be summized from the 2 data files we received was amazing.    The flexibility of working with Data Frames was the 
primary key to this exercise.    The early analysis was helpful, but, once the news about the Thomas High School 9th grade scores came in, we could quickly adjust. 
By replacing the scores with the loc() method, we could quickly refresh the reporting and see the impacts.   
 
Thomas High School math and reading grades for 9th graders were replaced with Nans, there are some unfortunate shifts in the reporting and the story.    
The changes include: 

   - 9th grade data is Nans 
   - overall passing % dropped from 91% to 65%, 
   - the passing math % dropped from 93% to 67%
   - the reading passing % dropped from 97% to 70%
   - overall passing % dropped from 91% to 65%

The score deletions at Thomas High School were also impactful to the District statistics.   
The changes include: 
   - the passing math % dropped from 75% to 74%
   - the reading passing % dropped from 86% to 85%
   - the overall passing % dropped from 65% to 64% 
