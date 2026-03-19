# Excel Data Analytics Project | Data Jobs Market Analysis

## Overview
This project examines a 2023 data jobs dataset to answer a practical market question: **which skills are most requested, which are associated with higher pay, and how salary patterns vary by role and region**.

Built in **Excel** with **Power Query, Power Pivot, DAX, PivotTables, and PivotCharts**, the project was designed as a compact analytical workflow rather than a static spreadsheet.

## What the project covers
The analysis focuses on four connected views:
- salary by role and number of skills required,
- salary comparison across regions,
- most common skills for selected roles,
- salary level versus skill prevalence.

## Dataset
The dataset captures **2023 job-posting signals for data roles**. It includes job title, salary, location, job ID, and required skills.

To make the analysis more robust, the source was structured into two linked tables:
- **data_jobs_all** — job-level records
- **data_jobs_skills** — skill-level records connected by `job_id`

This structure made it possible to move from flat reporting to relationship-based analysis.

## Analytical Workflow

### 1) Prepare the raw data
The first step was cleaning and shaping the source data in **Power Query**. This included organizing the records into a job table and a skill table so the later analysis would be consistent and scalable.

- data_jobs_all

<img width="1918" height="564" alt="power query" src="https://github.com/user-attachments/assets/0add3d2d-5351-482d-9ef6-bc6e5a130cb6" />

- data_jobs_skills

<img width="1903" height="595" alt="power query skills" src="https://github.com/user-attachments/assets/aa04a1c1-bef1-4210-96b2-9784123a0e27" />

### 2) Build the analytical model
After cleaning, both tables were loaded into the **Excel Data Model** and connected through `job_id`. This allowed salary analysis at the job level and skill analysis at the skill level without breaking the logic of the dataset.

<img width="810" height="702" alt="realtionship" src="https://github.com/user-attachments/assets/dd367c4c-1a97-42a6-a935-acfa81308c8b" />

### 3) Test whether broader skill requirements align with higher pay
The first analytical view compares **median salary** with the **average number of skills required per job**. This helps answer a simple but important question: do more demanding roles tend to pay more?

<img width="1155" height="429" alt="salaries vs skills" src="https://github.com/user-attachments/assets/49ff37bc-98f7-4fab-8f27-6b90fce30d3f" />

### 4) Compare market demand with market value
The final view compares **skill prevalence** with **median salary**. This separates skills that are merely common from skills that may carry stronger compensation signals.

<img width="1410" height="391" alt="skill salary analysis" src="https://github.com/user-attachments/assets/8bb8e97d-f365-4326-ac0e-b7d24e0d96fb" />

## Key Takeaways
- **SQL and Python** appear as foundational skills across data roles.
- Higher-paying roles often require a broader technical stack.
- Regional context matters: salary patterns differ materially across markets.
- Skill popularity and salary value are related, but they are not the same thing.
- Using **median salary** makes the analysis more resistant to outliers than a simple average.

## Why this project matters
This project was built to demonstrate more than spreadsheet usage. It shows a clear analytical chain:

**data preparation → data model → metric selection → insight generation**

That is the part of the work I want to emphasize as I transition into a Data Analyst role.

## Author

**Łukasz Filipek**  Aspiring Data Analyst with a background in project management and cost control.
