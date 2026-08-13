# IT Incident Analytics

An interactive Power BI dashboard designed to monitor IT support operations, incident trends, SLA compliance, MTTR, application performance, and workforce utilization through actionable visual analytics.

## Business Issue

IT support teams manage thousands of incidents across multiple applications, priorities, assignment groups, and environments. Without centralized reporting, monitoring SLA compliance, MTTR, incident backlog, and workforce utilization becomes time-consuming and makes it difficult to identify operational bottlenecks

## Resolution

Developed a multi-page Power BI solution using Power Query, DAX, and star-schema data modeling to consolidate ITSM incident data into an interactive reporting platform. The dashboard provides executive, application, workforce, and drill-through views to monitor operational KPIs, SLA performance, and incident trends.

## Business Impact

The solution enables support managers to monitor SLA compliance, MTTR, incident backlog, application health, and engineer workload from a single dashboard, helping prioritize operational improvements and identify service risks more efficiently.

## Business Questions Answered

The dashboard helps answer critical operational questions such as:
1. Which applications generate the highest number of incidents?
2. Are SLA targets being achieved?
3. How is MTTR changing over time?
4. Which engineers or assignment groups handle the highest workload?
5. Which priorities contribute to most SLA breaches?
6. Which environments (Production/UAT/Development) generate more incidents?

## Data Model

The report follows a Star Schema design.

**Fact Table**
- Incidents

**Dimension Tables**
- Dim_Date_table
- Dim_Applications
- Dim_Requesters

<img width="1043" height="511" alt="Model view" src="https://github.com/user-attachments/assets/4f4e473e-2bae-44a7-ba21-77e1f277917a" />

## Data Preparation (Power Query)
**Data Preparation (Power Query)**
- Standardized data types
- Cleaned null and blank values
- Removed duplicates
- Standardized categorical values
- Created calculated and conditional columns
- Prepared fact and dimension tables
- Created a dedicated Date table for time intelligence


**DAX Highlights**
- KPI Measures (Total, Open & Closed Incidents)
- SLA Compliance & Breach Analysis
- MTTR Analysis
- MTD, YTD & MoM Trend Analysis
- Dynamic Measures using CALCULATE and DIVIDE
- Time Intelligence using DATEADD
- Relationship-based Analysis using USERELATIONSHIP
- Dynamic Insight Cards


## Dashboard Pages

### Executive Dashboard

Provides a high-level overview of IT support performance for management.

Key Metrics:
1. Total Incidents
2. Open Incidents
3. Closed Incidents
4. SLA Compliance
5. MTTR
6. Escalation Rate

**Visuals**

1. Monthly Incident Trend
2. MTTR Trend
3. Priority Distribution
4. SLA Breach Analysis
5. Incident Volume by Environment
6. Executive Insight Cards

<img width="906" height="512" alt="Executive" src="https://github.com/user-attachments/assets/55aada8f-4dbe-40f6-914c-3b3a0171a3d0" />

---

### Application Dashboard

Provides application-level operational analysis.

Key Metrics:
1. Active Reopened Incidents
2. P1 Incidents
3. P2 Incidents
4. Open Production Incidents
5. Total Requesters

**Visuals**

1. Incident Volume by Application
2. Assignment Group Workload
3. Application MTTR Analysis
4. Priority Distribution
5. Application Insight Cards

<img width="906" height="511" alt="Application" src="https://github.com/user-attachments/assets/3fc4b6f8-934b-46d0-ab33-f82e5dc70c5b" />

---

### Workforce Dashboard

Monitors workload distribution and engineer performance.

**Key Metrics**

1. Total Engineers
2. Average MTTR per Engineer
3. Average Backlog per Engineer
4. Average Reopened Incidents

**Visuals**

1. Engineer Workload
2. Assignment Group Distribution
3. Engineer Performance
4. Escalation vs MTTR
5. Workforce Insight Cards

<img width="902" height="510" alt="Workforce" src="https://github.com/user-attachments/assets/da7a5e55-2158-428a-9d49-8dbddeba1642" />

---

### Incident Details (Drill-through)

Interactive drill-through page allowing users to investigate detailed incident records filtered by:

1. Application
2. Engineer
3. Assignment Group
4. Priority

<img width="906" height="511" alt="Drill through" src="https://github.com/user-attachments/assets/609082b2-366e-4302-b34f-1504caabee2a" />


**Drill-through Navigation**

<img width="899" height="505" alt="Executive drill through" src="https://github.com/user-attachments/assets/1c44b94b-031e-43a3-9779-3277567d521c" />

<img width="905" height="507" alt="Application Drill through" src="https://github.com/user-attachments/assets/c6c08837-17c5-4319-9cc6-9fc84f1b29cd" />

<img width="903" height="509" alt="Workforce drill through" src="https://github.com/user-attachments/assets/bdaf620f-d95a-4709-9f18-749b30cddda1" />


---

## Key Features

1. Multi-page interactive dashboard
2. Executive, Application, and Workforce reporting
3. Drill-through navigation
4. Dynamic KPI cards
5. Interactive slicers
6. Conditional formatting
7. Dynamic insight text
8. Operational reporting
9. Star schema data model
10. Dedicated Date table for time intelligence

---

## Technologies Used

1. Power BI Desktop
2. Power Query
3. DAX
4. Microsoft Excel (CSV)






