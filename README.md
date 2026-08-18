# Data Jobs Dashboard with Power BI
![Power BI Data Jobs Dashboard](./Images/1_Jobs_Dashboard_Overview.gif)

## Project Overview

I built this interactive Power BI report to help job seekers explore the 2024 data job market from one central dashboard. The report brings together information about job titles, salaries, posting trends, locations, work-from-home availability, degree requirements, health insurance, employment schedules, and hiring platforms.

The finished report includes a high-level market dashboard and a drill-through page for investigating individual job titles in greater detail.

### Dashboard File

Download the completed Power BI report:

**[1_Jobs_Dashboard.pbix](./1_Jobs_Dashboard.pbix)**

> Open the file in Power BI Desktop to use its interactive filters, navigation, and drill-through features.

## Questions Explored

This dashboard was designed to help answer the following questions:

1. Which data roles offer the highest salaries?
2. How does demand for data jobs change throughout 2024?
3. How do yearly and hourly salaries compare across job titles?
4. Which countries contain the most data job opportunities?
5. What percentage of postings offer remote work, mention no degree requirement, or include health insurance?
6. Which employment schedules are most common?
7. Which platforms list the most jobs for a selected role?

## Power BI Skills Demonstrated

- **Power Query and ETL:** Imported, cleaned, transformed, and prepared job-posting data for analysis
- **Data modeling:** Organized the report model around the primary job-postings table and supporting visual tables
- **Implicit measures:** Aggregated salary and job-count fields to create report-level KPIs
- **Calculated fields:** Created additional fields, including a salary star rating, to support dashboard interpretation
- **Interactive filtering:** Added job-title slicers that update the report based on the user's selection
- **Drill-through analysis:** Connected the market overview to a detailed page for individual job titles
- **Navigation design:** Used buttons and a page navigator to create a guided report experience
- **Core visualizations:** Built bar, column, line, area, scatter, donut, treemap, waterfall, funnel, and ribbon charts
- **Geospatial analysis:** Used map, filled-map, and ArcGIS visuals to analyze job locations
- **KPI reporting:** Used cards, gauges, KPI visuals, tables, matrices, and sparklines to summarize performance
- **Dashboard design:** Structured visuals into a consistent, readable, and user-focused interface

## Dashboard Pages

### Page 1: Data Jobs Dashboard

The main dashboard gives users a high-level view of the data job market and allows them to filter the entire page by job title.

![Data Jobs Dashboard Main Page](./Images/1_Jobs_Dashboard_Main_Page.gif)


### Main Dashboard Features

- Job-title slicer for interactive filtering
- Selected job-title summary card
- Salary star-rating card
- Yearly and hourly salary cards
- Monthly job-posting trend chart
- Salary comparison by data role
- Hourly-versus-yearly salary scatter plot
- Detailed matrix with job titles, salaries, quarterly data, and monthly sparklines
- Navigation button to access additional report pages

### Why This Page Matters

This page gives job seekers a quick way to compare data careers and understand how compensation and demand change across different roles. Instead of searching through individual postings, users can view the broader market from a single interface.

---

### Page 2: Job Title Drill Through

The drill-through page provides a focused analysis of one selected job title. Users can move from the main dashboard into this page while preserving the context of their selection.

![Job Title Drill-Through Page](./Images/1_Jobs_Dashboard_Drill_Through.gif)


### Drill-Through Features

- Selected job-title header
- Median yearly salary gauge
- Median hourly salary gauge
- Work-from-home percentage
- Percentage of postings that do not mention a degree
- Percentage of postings that include health insurance
- Global map of job-posting locations
- Employment schedule treemap
- Top job-posting platforms
- Back button for returning to the main dashboard

### Why This Page Matters

The drill-through page converts a broad market overview into a role-specific career profile. It allows users to examine compensation, flexibility, benefits, location, employment type, and hiring sources for the job that interests them most.

## Data Model

The report uses a primary `job_postings_flat` table containing the job-market data. 

The primary dataset contains fields related to:
- Job titles
- Annual and hourly salaries
- Countries and posting locations
- Posting dates
- Work-from-home availability
- Degree requirements
- Health-insurance information
- Employment schedules
- Job-posting platforms

## Analytical Approach

1. Imported the 2024 job-posting dataset into Power BI.
2. Prepared and transformed the data using Power Query.
3. Reviewed different visual types across dedicated development pages.
4. Created summary metrics for salaries, job counts, and job-posting characteristics.
5. Built a high-level dashboard with interactive job-title filtering.
6. Created a drill-through page for role-specific analysis.
7. Added navigation elements to make the report easier to explore.
8. Organized the visuals into a consistent two-page portfolio dashboard.

## What I Learned

This project strengthened my ability to:

- Transform raw job-posting data into an interactive business-intelligence report
- Select visualizations based on the analytical question being answered
- Build report interactions with slicers, buttons, navigation, and drill-through
- Compare compensation, demand, benefits, and geographic trends across job roles
- Use cards, gauges, matrices, and sparklines to communicate KPIs at different levels of detail
- Organize multiple visuals into a clear and consistent dashboard experience
- Design a report for both high-level exploration and detailed analysis

## Limitations

- The dataset represents job postings from 2024 and may not reflect current market conditions.
- Salary information is not available for every posting.
- Job-posting data may contain duplicate, expired, or inconsistently categorized listings.
- Salary differences may also be influenced by seniority, industry, company size, and location.
- The report identifies patterns and associations within the available data; it does not establish causation.

## How to Use the Dashboard

1. Download [`1_Jobs_Dashboard.pbix`](./1_Jobs_Dashboard.pbix).
2. Open the file in Power BI Desktop.
3. Use the Home page or navigation controls to explore the report.
4. Open the **Data Jobs Dashboard** page.
5. Select a role from the job-title slicer to update the dashboard.
6. Use drill-through on a job title to open the detailed analysis page.
7. Use the back button to return to the main dashboard.

## Repository Structure

```text
PowerBI_Data_Jobs_Dashboard/
│── Data/
│   ├── job_postings_flat.csv
│   └──README.md
├── Images/
│   ├── 1_Jobs_Dashboard_Overview.gif
│   ├── 1_Jobs_Dashboard_Main_Page.gif
│   └── 1_Jobs_Dashboard_Drill_Through.gif
├── 1_Jobs_Dashboard.pbix
└── README.md
```

## Conclusion

This project demonstrates how Power BI can turn a large job-posting dataset into an accessible career-analysis tool. By combining data transformation, interactive filtering, KPI reporting, multiple visualization types, navigation, and drill-through functionality, I created a report that supports both broad market exploration and detailed job-title analysis.

## Acknowledgment

The dataset provided through [Luke Barousse's Power BI Data Analytics course](https://github.com/lukebarousse/PowerBI_Data_Analytics_Course). I used the course materials to develop and document my own Power BI report.
