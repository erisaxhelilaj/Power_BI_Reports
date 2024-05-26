
# <p align="center" style="margin-top: 0px;">📊 Employee Engagement and Satisfaction Report 📊

Dashboard Link : [https://app.powerbi.com/groups/me/reports/384d017e-e935-44dc-9e7d-1626c1a36de1/ReportSection](https://app.powerbi.com/view?r=eyJrIjoiNTE5MzYyZGItYjI1Zi00MWE2LWE1YmEtMDlhMjBmNWRlYzcyIiwidCI6ImNhOWY5NDcwLWIxZjctNGI2NC1hNjM2LWUzOWYwMDE3NGQxOCIsImMiOjl9)


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













