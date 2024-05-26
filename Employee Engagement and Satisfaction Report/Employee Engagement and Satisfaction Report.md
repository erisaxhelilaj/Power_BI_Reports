
# <p align="center" style="margin-top: 0px;">📊 Employee Engagement and Satisfaction Report 📊

This dashboard presents a detailed analysis of employee satisfaction. It visually displays survey results on job clarity, professional growth opportunities, break area accessibility, and overall office environment, all rated on a scale of 1 to 5.
It contains various charts and metrics related to employee responses, including pie charts, bar graphs, and numerical statistics.


## 📊 Overview Report 

<p align="center" style="margin-bottom: 0px !important;">
<img src="https://github.com/erisaxhelilaj/Power_BI_Reports/blob/master/Employee%20Engagement%20and%20Satisfaction%20Report/DataSets/Overview.PNG" width="900" height="550">



#### :arrow_right: Here's a breakdown of the visual elements:

**1.** **Responses by Age Group Pie Chart:** This chart shows the distribution of responses by age group. </p>
**2.** **Tenure Pie Chart:** This chart illustrates the tenure of the respondents </p>
**3.** **Employee Status Pie Chart:** It shows the employment status of the respondents </p>
**4.** **Team Collaboration Ratings by Employees Bar Graph:** This horizontal bar graph displays the ratings for team collaboration but does not show the number of responses for each rating. 
 The ratings are on a scale from 1 to 5, with 5 being the highest.  </p>
**5.** **Employee Satisfaction with Company-Organized Team Building Activities Bar Graph:** This horizontal bar graph shows the number of responses for each satisfaction level, ranging from 1 to 5, with 5 being the highest level of satisfaction.  </p>
**6.** **Numerical Statistics Boxes:**  </p>
  - Participation Rate :
  
```
participation_rate = COUNTROWS('form_responses') / 696

```

  - Average Score :
```
average_engagement_score = 
AVERAGEX(
    form_responses,
    (
        form_responses[role_clarity_score] +
        form_responses[growth_opportunity_rating] +
        form_responses[manager_effectiveness_of_communication] +
        form_responses[managers_openness_rating] +
        form_responses[department_teamwork_score] +
        form_responses[team_building_score] +
        form_responses[break_space_usability_score] +
        form_responses[workplace_environment_score]
    ) / 8
)
```

**7.** **Button Options:** On the top right, there are filter options for the visualization, which include buttons for **"Management"** and **"Work Culture."**


***
## 📊 Management & Work Culture 

<p align="center" style="margin-bottom: 0px !important;">
<img src="https://github.com/erisaxhelilaj/Power_BI_Reports/blob/master/Employee%20Engagement%20and%20Satisfaction%20Report/DataSets/Management%20%26%20Work%20Culture.PNG" width="900" height="550">


**"Management and Work Culture Report,"** divided into two sections: Management and Work Culture. </p>
#### :arrow_right: Here's a breakdown of the visual elements:

**1.** **Perceptions of Workplace Inclusivity:** This horizontal bar chart shows responses to how inclusive the workplace is perceived to be. The categories are "Inclusive," "Highly Inclusive," "Neutral," "Not Inclusive," and "Very Inclusive," with numerical values indicating the number of responses in each category. </p>
**2.** **Sense of Belonging at Company:** Below the first chart is a pie chart titled "Sense of Belonging at Company" with slices representing different sentiments: "Definitely, it's where I belong," "I'm still trying to figure that out," "No, I feel like I don't fit in at all," "Sometimes, but other times I f..." and "Yes, it feels like home." Each slice is accompanied by a number and percentage of responses. </p>
**3.** **Team and Department Communication Satisfaction:** This pie chart shows the level of satisfaction with team and department communication. The categories include "Neutral," "Satisfied," "Unsatisfied," "Very Satisfied," and "Very unsatisfied," each with corresponding response counts and percentages. </p>
**4.** **Employee Outlook for the Next 2 Years:** The last section on the right side of the image is a line graph with a dotted line showing employee outlook for the next two years. The x-axis has categories "Agree," "Disagree," "Neutral (neither agree nor disagree)," "Totally Agree," and "Totally disagree," but there are no numerical values or response counts provided on the y-axis. </p>



***
## 📊 Experience & Work Environment 

<p align="center" style="margin-bottom: 0px !important;">
<img src="https://github.com/erisaxhelilaj/Power_BI_Reports/blob/master/Employee%20Engagement%20and%20Satisfaction%20Report/DataSets/Experience%20%26%20Work%20Environment.PNG" width="900" height="550">


This report appears to be a graphical representation of survey results regarding employee satisfaction at a company. The report is divided into two main sections: **Employee Experience and Work Environment.** </p>
#### :arrow_right: Here's a breakdown of the visual elements:

**1.** A pie chart titled **"Recommending Company as a Workplace".** </p>
**2.** A bar chart titled **"Satisfaction with Clarity of Job Responsibilities":** displays responses on a scale from 1 to 5, with the majority of responses in category 3.  </p>
**3.** Another bar chart titled **"Satisfaction with Growth Opportunities:"** shows responses on a scale from 1 to 5, with the majority of responses in categories 3 and 4.  </p>
**4.** A bar chart titled **"Favorite Office Features"** lists features such as Open Spaces, Break Areas, Ergonomic Furniture, Interior Design, Natural Lighting, Private Workstations, and Recreation Areas, with Break Areas receiving the highest number of responses (45) and Ergonomic Furniture the lowest (7).  </p>
**5.** A pie chart titled **"Satisfaction with the Environment and Office:"** shows responses on a scale from 1 to 5, with the majority of responses in category 4 (97 responses, 34.52%).   </p>
**6.** A bar chart titled **"Satisfaction with Workplace Break Areas:"** shows responses on a scale from 1 to 5, with a relatively even distribution among the categories. </p>




