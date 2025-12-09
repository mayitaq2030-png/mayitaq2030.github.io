# Help Desk Performance Monitoring Dashboard for SAAS Medical Insurance 

### Executive Summary:

<p align ="justify"> Using SQL, Python, and Power BI, I analyzed RWFD’s Help Desk performance to identify service gaps, ticket resolution delays, and workload patterns affecting operational efficiency. The dashboard highlights rising backlog levels, decreasing resolution rates, and consistent login/access-related issues. These insights reveal immediate opportunities to optimize ticket handling, improve agent productivity, and reduce customer dissatisfaction.</p>

Key areas of improvement:

- Reduce backlog by optimizing triage and prioritization workflows.

- Strengthen ticket ownership accountability across engineering groups.

- Improve response and resolution times through automation and SLA monitoring.

### Business Problem:
   
<p align ="justify"> The Help Desk is managing a rising volume of tickets, but metrics show declining performance. According to the dashboard, total ticket volume reached 1120, with a 13.9% resolution rate decreasing from the prior month and 71.7% of tickets remaining open, indicating operational bottlenecks .The backlog represents 55.7% of open tickets, reflecting limited capacity, slow triage processes, and inconsistent ownership across teams such as Networking, Architecture, Hardware, and Security & Governance.
Furthermore, ticket satisfaction data reveals that 38% of responses fall into Unsatisfied or Unknown, and Access/Login issues represent a major portion of problems, suggesting systemic authentication or permission inconsistencies. These gaps reduce service quality, increase customer friction, and delay business productivity. </p>
 
Order completion for chart 

<img width="1470" height="771" alt="FlowChart" src="https://github.com/user-attachments/assets/8bc3beeb-c6b7-4f2e-bb9a-2bfb24fefcdb" />

#### Methodology:

- Data Extraction: SQL queries to pull ticket history, issue types, severity, owner group, and satisfaction logs.
- Data Processing: Python (Pandas, Numpy) for cleaning, categorization, outlier detection, and aggregation.
- Visualization: Power BI dashboard with KPIs for ticket status, severity, backlog, satisfaction, and category trends.
- Comparative Analysis: Month-over-month change, ticket aging distribution, resolution vs. open ratios, and severity load.


#### Skills:

- SQL: Filtering, joins, aggregations, SLA calculations.

- Python: Data cleaning, categorization, KPI computation.

- Power BI: DAX, relationships, advanced visuals (donuts, bar charts, trend lines).

- Analytics: Ticket aging analysis, workload trends, customer satisfaction insights.

- BI Storytelling: Translating operational data into actionable improvements.

### Results & Business Recommendations:

<p align ="justify"> The dashboard reveals high ticket volume (1120) with a large share of open cases (71.7%) and a declining resolution rate. Backlog increased to 55.7%, indicating capacity and workflow inefficiencies. Satisfaction levels are mixed, with 38% of users either unsatisfied or providing no feedback. Access/Login and Hardware issues represent the highest incident categories. Reducing backlog by 10% could significantly improve resolution times and customer satisfaction. Automating triage and enforcing SLA-driven prioritization are recommended as immediate actions.</p>

<img width="710" height="394" alt="image" src="https://github.com/user-attachments/assets/832c3337-eff1-41bf-ae68-0a2be7edbf91" />

🎯 Total tickets: 1120, down -7.4% vs PM.

🎯 Resolved: 13.9%, slight improvement vs PM.

🎯 Open: 71.7%, still critically high.

🎯 Avg. days open: 19.3, above SLA expectations.

🎯 Satisfaction: 34% Highly Satisfied, 28% Satisfied, 29% Unknown, 9% Unsatisfied.

🎯 Most common issues: Hardware (29%), Software (22%), Access/Login (32%).

🎯 Most open tickets belong to: Security & Governance (22%), Networking (22%), Architecture (21%).

Because the strongest opportunities to improve Help Desk performance come from reducing backlog, increasing resolution rate, and improving cross-team ownership, I recommend:

Automate ticket triage and categorization to reduce manual routing time and ensure high-severity cases are addressed first.

Strengthen ownership enforcement across Architecture, Networking, Hardware, and Security teams to reduce the high volume of “Unassigned” tickets.

Improve Access/Login reliability by addressing root causes of authentication failures, which represent one of the largest ticket categories.

Implement SLA-driven alerts and dashboards to reduce aging tickets and improve agent accountability.

Enhance customer communication workflows to decrease “Unknown” satisfaction responses and increase feedback rates.

### Next Steps:

📌 Introduce predictive analytics to forecast ticket surges and staffing needs.

📌 Build automated SLA alerts for overdue or high-severity cases.

📌 Integrate Help Desk data with monitoring systems to correlate issues with outages.

📌 Conduct root-cause analysis on the most frequent issues (Hardware, Access/Login).

📌 Build a monthly performance report for leadership to track progress.
