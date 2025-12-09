# Help Desk Performance Monitoring Dashboard for SAAS Medical Insurance 

### Executive Summary

An interactive dashboard was designed to monitor the performance of the Help Desk over a monthly period. The report reflects a total of 1,120 tickets, showing a 7.4% decrease compared to the previous month. Workload is evenly split between Requests (50%) and Issues (50%).
Although the resolution rate improved to 13.9%, the majority of tickets (71.7%) remain open, with a backlog reaching 55.7% of open tickets and an average age of 19.3 days. User satisfaction is concentrated in “Satisfied” and “Highly Satisfied” categories; however, 43% of responses are marked as “Unknown”, limiting the ability to accurately assess true customer experience.
The project enables the identification of bottlenecks, prioritization by severity and technical area, and data-driven decision-making to reduce backlog, shorten resolution times, and increase end-user satisfaction.

### Business Problem
   
The IT Support / Help Desk area needed clear answers to the following key questions:

Are we resolving tickets fast enough?

A high percentage of open tickets (71.7%) and a backlog representing 55.7% of open tickets indicate accumulation and potential SLA breaches.

What types of incidents are driving the highest demand?

Tickets are distributed across Systems, Software, Hardware, and Access/Login, with Systems and Hardware being the most frequent categories.

How satisfied are our end users?

Only 47% of users report being “Satisfied” or “Highly Satisfied,” while 11% are dissatisfied and a significant 43% of responses remain “Unknown,” severely limiting visibility into the true customer experience.

Which technical teams are under the heaviest workload?

Owner groups such as Hardware, Networking, and Security & Governance handle a substantial portion of tickets, creating potential bottlenecks and resource imbalances.

Project Objective
Reduce backlog and resolution times, improve end-user experience, and optimize resource allocation across support teams through data-driven insights and actionable KPIs.
 
Order completion for chart (Marjorie Quintero)

To build a clear, business-aligned dashboard, the visuals were designed and arranged in the following logical sequence:

<img width="591" height="541" alt="Captura de pantalla 2025-12-03 172545" src="https://github.com/user-attachments/assets/4e82ff33-afda-47e8-a0e0-22cfa0cce35c" />

This layout allows the dashboard to be read like a funnel:
volume → status → customer perception → root cause → priority → responsible team.

#### Methodology

##### CRISP-DM Methodology

Business Understanding:

Meetings with the Support team to define objectives: reduce backlog, understand ticket severity distribution, and improve user satisfaction.

Data Understanding:

Review of ticket tables: fields such as date, type, status, severity, owner group, satisfaction, etc.

Data Preparation:

Handling of null values (especially in satisfaction and severity columns).
Normalization of categories ( standardizing status names).
Creation of calculated fields: days open, backlog indicator, creation month.

Modeling:

Development of a star-schema data model:
Fact table: Tickets
Dimension tables: Date, Type, Status, Severity, Issue, Owner Group, Customer

Definition of key measures (KPIs) using SQL and/or DAX.

Evaluation:

Validation with the Support team: comparison of dashboard results against previous reports and operational reality.

Deployment:

Publication of the interactive dashboard in a Power BI tool .
Short training session for supervisors on how to interpret and use the dashboard effectively.

#### Skills:

SQL (MySQL / SQL Server / PostgreSQL)
Data extraction from ticket tables.
Creation of aggregated views by month, severity, status, and owner group.

Data Modeling
Design and implementation of a star-schema model with proper relationships between fact and dimension tables.

Power BI 
Development of bar charts, KPI cards, line charts, donut charts, and interactive slicers/filters.

Excel / Google Sheets
Support for initial data exploration, validation, and quick calculations.

Basic Statistics
Calculation of percentages, month-over-month variations, and trend analysis.

Data Storytelling
Visual flow design following a logical funnel (volume → status → customer perception → root cause → priority → responsible team) and prioritization of key metrics for fast decision-making.

### Results & Business Recommendations:

<img width="904" height="489" alt="image" src="https://github.com/user-attachments/assets/613730c5-fe1b-4110-9372-7863703a17b6" />

#### Results

Slight reduction in total ticket volume:

1,120 tickets vs 1,210 the previous month (–7.4%), indicating a modest relief in workload.

Improved resolution rate:

13.9% resolved vs 12.1% the previous month (+6.8%), reflecting higher resolution efficiency.

Persistent high percentage of open tickets:

71.7% still open, feeding a backlog of 55.7% of open tickets with an average age of 19.3 days.

User satisfaction distribution:

47% Satisfied or Highly Satisfied
11% Unsatisfied
43% Unknown/no response → clear gap in feedback collection.

Severity & team workload insights:

17% High severity tickets and 32% Unassigned severity, hindering proper prioritization.
Hardware, Networking, and Security & Governance teams carry a significant share of the workload.

#### Business Recommendations

Reduce backlog and average days open:

Define strict SLAs by severity (e.g., High ≤ 3 days).
Run weekly “backlog sprints” focused exclusively on closing aged tickets.

Improve satisfaction feedback capture:

Make a short survey mandatory upon ticket closure.
Automate survey reminder emails.

Enforce mandatory severity assignment:

Prevent ticket creation/submission without a severity level.
Train agents to quickly classify tickets based on impact and urgency.

Balance workload across teams:

Review capacity of Hardware, Networking, and Security & Governance groups.
Consider reallocating staff or enhancing self-service tools for the most frequent incident types.

Promote self-service and knowledge base:

For recurring categories (Access/Login, common Software issues), develop self-service guides and a robust FAQ section to reduce new ticket creation.

(Ready
