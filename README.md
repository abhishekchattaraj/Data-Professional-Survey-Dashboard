# Data Professional Survey Breakdown

**Interactive Power BI dashboard analyzing demographics, salaries, skills, and satisfaction of data professionals.**

---

## Overview
This repository contains a **Power BI dashboard** that explores a **global survey of data professionals**.  
It shows:

- Where respondents are located  
- How salaries vary by role and gender  
- Which programming languages are most popular  
- How satisfied professionals are with work–life balance and pay  

Use this repo to **preview the project**, review methodology, and open the dashboard locally.

---

## Tech Stack
- **Power BI Desktop**
- **Data:** Excel, cleaned in **Power Query:** Yes
- **Optional preprocessing:** N/A

---

## Data Source
- **Source:** `https://github.com/AlexTheAnalyst/Power-BI/tree/main`
- **Sample size (unique respondents):** `504`
- **Survey period:** `October/2022 – December/2022`
- **Notes/assumptions:** All salaries converted to USD. Shortened the different job titles that were not primary focus to "Other" category.

---

## Business Problem and Goal
**Problem:**  
Organizations and aspiring professionals often lack clear, consolidated insights into the current state of the data industry.  
Understanding salary benchmarks, regional trends, popular skills, and job satisfaction levels is crucial for making informed career and hiring decisions.  
However, this information is often scattered across different sources and not presented in an interactive, easy-to-digest format.

**Goal:**  
Deliver a concise, interactive dashboard answering:
- Where respondents are based  
- What they earn by role and gender  
- Which languages they use  
- How satisfied they are

---

## Key Questions
1. Which countries do respondents come from?
2. What is the average salary by job title?
3. Which programming languages are most popular, and how does usage vary by role?
4. What is the average salary by gender?
5. How many people took the survey, and what is their average age?
6. How satisfied are respondents with work–life balance and current salary?

---

## Dashboard Features and Visuals

### Respondents by Country (Treemap)
- **Categories:** United States, United Kingdom, India, Canada, Others  
- **Configuration:** `Category = Country; Values = Country (count)`  
- **Insight:** Top country = `United States` with `219` respondents (`43% of total`)

### Average Salary by Job Title (Stacked Bar Chart)
- **Y-axis:** Job Title (Data Scientist, Data Engineer, Data Analyst, Data Architect, Database Developer, Student/Looking/None, Other)  
- **X-axis:** Average Salary  
- **Legend:** Job Title  
- **Insight:** Highest average salary = `Data Scientist` at `$94,000`; Lowest = `Student/Looking/None` at `$28,000`

### Favorite Programming Language by Role (Stacked Column Chart)
- **X-axis:** Programming Language (Python, R, C/C++, JavaScript, Java, Other)  
- **Y-axis:** Count of Unique ID (respondents)  
- **Legend:** Job Title  
- **Insight:** Most popular language overall = `Python` with `331` users (`65% of respondents`)

### Average Salary by Gender (Donut Chart)
- **Legend:** Gender (Male, Female)  
- **Values:** Average of Salary  
- **Insight:** Avg salary — Male: `$54,000`, Female: `$57,000`  
  *(Difference: USD 2,000 / 3.7%)*

### KPI Cards
- **Count of Survey Takers:** `504`  
- **Average Age:** `29` years

### Satisfaction Gauges (1–10 scale)
- **Work–Life Balance:** Avg = `5.72`, Min = `1`, Max = `10`  
- **Current Salary Satisfaction:** Avg = `4.26`, Min = `1`, Max = `10`  
- **Insight:** WLB avg = `5.72`; Pay satisfaction avg = `4.26`

---

## How to Use
1. Install **Power BI Desktop** (`Version: 2.1.x or later`).
2. Clone or download this repository.
3. Open `Data Professional Survey Breakdown.pbit`.
4. Refresh the data: **Home → Refresh**.

---

## Data Connections
- **Local file:** `Data Professional Survey Data.xlsx` 
- **Parameters:**  
  - `Currency = USD`

---

## Methodology and Cleaning
- **Deduplication:** Unique respondents identified by `UniqueID`.
- **Salary handling:** Currency normalized to `USD($)`.
- **Role categories:** Standardized to listed roles; “Other” groups low-frequency titles.
- **Country grouping:** Top countries shown; remaining grouped as “Others”.
- **Age:** Validated within `<18-100>` bounds.

---

## Key Insights
- **Geography:** `43% of survey respondents were from the United States, followed by "Other" countries and India.`  
- **Roles and pay:** `Data Scientist has highest avg salary at $94,000; Student/Looking lowest at $28,000.`  
- **Skills:** `Python dominates across roles.`  
- **Gender gap:** `Avg difference of $2,000 (female salaries ~3.7% higher).`  
- **Satisfaction:** `WLB 5.7/10 vs Pay 4.2/10.`  
- **Demographics:** `Average age 29.`

---

## Image Preview
![Dashboard Overview](Data%20Professional%20Survey%20Breakdown%20Image.jpg)

---

## Getting Started Quickly
- **Prerequisites:** Power BI Desktop `2.1.x or later`
- **Estimated setup time:** `5 minutes`
- **Test data sample included:** `Yes`.

---

## License
`No license`

---

**Author:** `Abhishek Chattaraj` — [Email](mailto:abhishekchattarajj@gmail.com) — [LinkedIn](https://www.linkedin.com/in/abhishek-chattaraj-b25a78125) — [GitHub](https://github.com/abhishekchattaraj)
