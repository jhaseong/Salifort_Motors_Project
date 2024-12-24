Salifort Motors Project

Overview
To reduce employee turnover and improve satisfaction, Salifort Motors has commissioned this project to analyze HR data and build a predictive model.

Business Understanding

Two distinct groups of departing employees were identified: (A) those who worked significantly fewer hours than peers with similar project loads, and 
(B) those who worked substantially more. Group (A) may include employees who were terminated or those with pending departures assigned reduced hours. 
Group (B) likely resigned, potentially after making significant contributions to their projects.

Data Understanding

Notably, all employees assigned seven projects left the company. Analysis of monthly working hours revealed that the interquartile range for this 
group and those with six projects was approximately 255-295 hours, considerably higher than any other group. The low attrition rate among employees 
with 3-4 projects suggests this as a more optimal workload. Based on a standard 40-hour workweek and two weeks of vacation, the expected monthly 
working hours are 166.67. However, with the exception of those with two projects, all groups, including retained employees, worked substantially 
more, indicating a potential pattern of overwork.

![image](https://github.com/user-attachments/assets/c863bf4f-d61c-464a-840d-8a27578c66a3)

Modeling and Evaluation

Evaluation on the test set revealed the following performance metrics for the logistic regression model: precision (80%), recall (83%), 
F1-score (80%, weighted average), and accuracy (83%). Subsequent feature engineering led to substantial improvements in the decision tree model's 
performance, with an AUC of 93.8%, precision of 87.0%, recall of 90.4%, F1-score of 88.7%, and accuracy of 96.2%. The random forest model demonstrated 
a marginal improvement over the enhanced decision tree.

![image](https://github.com/user-attachments/assets/c3c33fba-84c0-48d0-92d6-6780daabb444)

![image](https://github.com/user-attachments/assets/1183a76b-d1bd-43d9-b60f-c17a2f8cf73e)

Conclusion

Analysis of the models and extracted feature importances provides strong evidence of employee overwork. To address this and improve retention, we 
recommend the following actions for stakeholders:

1) Project Load Management: Implement a formal policy limiting the number of projects assigned to each employee concurrently. This will help prevent
unsustainable workloads.
2) Tenure and Promotion: Review promotion practices for employees with four or more years of service, as this group appears to be particularly dissatisfied.
Further investigation is warranted to understand the root causes of this dissatisfaction.
3) Overtime Policy: Re-evaluate the company's approach to overtime. If long hours are necessary, ensure appropriate compensation is provided. Alternatively,
explore strategies to reduce the reliance on overtime.
4) Communication and Transparency: Ensure that all employees are fully aware of the company's overtime pay policies. Clearly define expectations regarding
workload, time off, and work-life balance.
5) Culture Assessment and Dialogue: Conduct company-wide and team-specific discussions to identify and address issues related to work culture, workload
management, and employee well-being.
6) Performance Evaluation: Revise performance evaluation metrics to avoid incentivizing excessive working hours (200+ hours/month). Implement a more
balanced system that recognizes contributions, effort, and overall performance, rather than simply rewarding time spent at work.
