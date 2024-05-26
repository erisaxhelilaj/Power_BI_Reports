# <p align="center" style="margin-top: 0px;">📊 Recruiting Report - Performance 📊

This dashboard used to track the efficiency and outcomes of a recruitment process over a specified period. It provides insights into the recruitment process, including interview distribution, candidate progression through stages, and the effectiveness of various recruitment sources. The report highlights important data points like the average number of interviews, total hires, and the size of the candidate pool. Overall, it offers a visual representation of recruitment activities and outcomes within the specified timeframe.


## 📊 Overview Report 

<p align="center" style="margin-bottom: 0px !important;">
<img src="https://github.com/erisaxhelilaj/Power_BI_Reports/blob/master/Recruiting%20Report%20-%20Performance/DataSets/Recruiting.PNG" width="900" height="550">



#### :arrow_right: Here's a breakdown of the visual elements:

**1.** **Interviews per position:** This section lists different job positions and the number of interviews conducted for each. The position with the highest number of interviews is "Promoter Push" with 948 interviews, followed by "Operatore Smart Agent..." with 463, and so on. </p>
**2.** **Candidates per stages:** It shows the number of candidates at different stages of the recruitment process, such as "Screening" with 9,695 candidates, "Refused" with 6,113, and various other stages like "Da Ricontattare," "Setting," "Department Interview," etc.  </p>
**3.** **Interviews & hired per recruiter:** This part of the infographic seems to compare the number of interviews conducted to the number of candidates hired by each recruiter </p>
**4.** **Numerical Statistics Boxes:**  </p>
  - Job Positions: 
  
```
b_positions = 
 DISTINCTCOUNT(main_table[job_position] )
```

  - Interviews:
```
b_interview = 
 CALCULATE(
    COUNT( main_table[transformed_stage_name]),
    FILTER(
        main_table, main_table[transformed_stage_name] = "In person/HR Interview"
    )
 )
```


 - Avg Interviews: 
  
```
b_avg_interview = 
 DIVIDE(
    [b_interview], [worked_days]
 )
```

- Worked Days: 
  
```
worked_days = 
 NETWORKDAYS(
     MIN( calendar_table[Date] ),
     MAX( calendar_table[Date] ),
     2)
```

- Hired: 
  
```
b_hired = 
 CALCULATE(
    COUNT(main_table[stage_name] ),
    FILTER(
        main_table, main_table[stage_name] = "Hired"
    )
 )
```

- Pool: 
  
```
b_pool = 
 CALCULATE(
    COUNT(main_table[stage_name] ),
    FILTER(
        main_table, main_table[stage_name] = "Stand by"
    )
 )
```






