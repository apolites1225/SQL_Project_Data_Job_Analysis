# Introduction
Dive into the data job market! Focusing on data analyst roles, this project explores top-paying jobs, in-demand skills, and where high demand meets high salary in data analytics.
SQL queries? Check them out here: [project_sql folder](/project_sql/).
# Background
Driven by a quest to navigate the data analyst 
# Tools I used
- **SQL:**
- **PostgreSQL:** The backbone of my analysis
- **Visual Studio Code:**
- **Git & GitHub:**
# The Analysis
Each query for this project aimed at investigating specific aspects of the data analyst job market. Here's how I approach each question.

### 1. Top Paying Data Analyst Jobs
To identitify the highest-paying roles...

```sql
SELECT
    job_id,
    job_title,
    job_location,
    job_schedule_type,
    salary_year_avg,
    job_posted_date,
    name AS company_name
FROM
    job_postings_fact
LEFT JOIN company_dim ON
    job_postings_fact.company_id = company_dim.company_id
WHERE
    job_title_short = 'Data Analyst' AND
    job_location = 'Anywhere' AND
    salary_year_avg IS NOT NULL
ORDER BY 
    salary_year_avg DESC
LIMIT 10
```
Here's the breakdown of the top data analyst jobs in 2023:
-- **Wide Salary Range:** \

![Top Paying Roles]()
# What I Learned
Throughout this adventure, I've turbocharged my SQL toolkit with some

# Conclusions
### Insights
1. Top 
2. Top
3. Top
4. Top
5. Top

### Closing Thoughts
This project enhanced. 