# Data Professional Survey Breakdown: Power BI Dashboard

An interactive Power BI dashboard that summarizes a survey of 630 data professionals: what they earn, which programming languages they prefer, how satisfied they are, and how hard it was to break into the field.

## The questions

- Which data roles earn the most, and where do data analysts fall?
- Which programming languages do data professionals prefer?
- How satisfied are data professionals with their salary and work/life balance?
- How difficult do people find it to break into data?

## Dataset

- **Source:** survey of data professionals conducted by Alex the Analyst in 2022
- **Size:** 630 respondents
- **Fields used:** profession, salary, age, country, favorite programming language, salary satisfaction, work/life balance, and difficulty breaking into data

## Tools

Power BI Desktop

## What the dashboard shows

| Visual | What it shows |
|---|---|
| KPI cards | Total survey takers (630) and average age (29.87) |
| Gauges | Average salary satisfaction and work/life balance, each out of 10 |
| Treemap | Where respondents live, by country |
| Stacked column chart | Favorite programming language, split by profession |
| Donut chart | How hard respondents say it was to break into data |
| Bar chart | Average salary by profession |

## Data preparation

Before building the visuals, I cleaned the survey data so the charts would be accurate:

1. **Cleaned columns:** tidied the fields used in the dashboard so each held consistent, usable values.
2. **Standardized categories:** grouped inconsistent or rarely used responses, such as job titles and programming languages, into a single **Other** category so the charts were readable.
3. **Fixed values:** corrected inconsistent or incorrectly formatted entries, so measures like average salary and average age were calculated correctly.

## Key findings

- **Data scientists earn the most.** The average salary is **$94K**, compared with **$65K** for data engineers, **$64K** for data architects, and **$55K** for data analysts, about **$39K** less than data scientists.
- **Python is the clear favorite.** Roughly 420 of the 630 respondents, about two-thirds, chose it, far ahead of R (about 100) and "Other" (about 95).
- **Salary satisfaction is low.** Respondents rated it **4.27 out of 10**, while work/life balance scored higher at **5.74 out of 10**.
- **Breaking into data is seen as neither easy nor hard by most.** **42.7%** (269 people) chose neutral, **31.7%** found it difficult or very difficult, and **25.6%** found it easy or very easy.
- **Entry-level roles pay the least.** Respondents who are students, job seekers, or in no role averaged **$27K**, and database developers averaged **$33K**.

## Limitations

- The survey is self-reported and voluntary, so respondents may not represent all data professionals.
- Salaries are averages, so a few high earners can pull a group's average up, especially in small groups.
- Country counts are shown as a treemap without labeled values, so the exact split is not displayed.

## What I learned

- Building a multi-visual dashboard in Power BI Desktop and arranging it for readability
- Choosing the right visual for each question: gauges for ratings, a donut for proportions, bars for comparisons
- Turning a dashboard into plain-language findings for a non-technical audience

## Next steps

- Add slicers so viewers can filter by country, profession, and gender
- Explore salary by country and years of experience
- Rebuild the same analysis in SQL or Python to cross-check the results
