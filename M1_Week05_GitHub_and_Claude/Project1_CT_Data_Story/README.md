# Project 1: A Connecticut Data Story

**OPIM 3510 · Module 1 · Team project · due end of Week 5**

## The job
Connecticut publishes a treasure trove of town-level data: housing, education, health, income, energy, crime. Your team picks **2–3 datasets, joins them by town, and tells a story** about Connecticut with tables, plots and a clear narrative. Pick something you'd be proud to show in a job interview, because it's going on your GitHub.

**Where to find data:**
* **Starter option:** [`data/ct_home_sales_2025.csv`](../../data/ct_home_sales_2025.csv) (27,000 home sales; summarize it by `town` first) plus the CTData town tables already in [`data/`](../../data) (median home value, educational attainment), the same ones from the Week 4 Long-to-Wide notebook.
* **Find your own:** [CTData by topic](https://www.ctdata.org/data-by-topic) · [data.ct.gov](https://data.ct.gov/browse). Look for datasets with a **`Town`** column so they join cleanly. (Remember: Connecticut has **169 towns**. Watch for a "Connecticut" statewide-total row hiding in town tables!)

Start here: [**Open the project template in Colab**](https://colab.research.google.com/github/drdave-teaching/OPIM3510-BDA1/blob/main/M1_Week05_GitHub_and_Claude/Project1_CT_Data_Story/Project1_CT_Data_Story.ipynb)

## Rubric
| Part | What | Points |
|---|---|---|
| **1. Motivation** | What question are you answering, and why should anyone care? At least 8 sentences; cite 3 sources (bullets). | 10 |
| **2. Join and clean** | Read 2–3 datasets **from your team repo**, reshape if needed, join on town, fix data types and missing values. Check row counts before and after every join. No duplicate or confusing columns. | 25 |
| **3. Three amazing tables** | Not just `describe()`. Use `groupby`, flags, percentiles, rankings. Each with a caption that says what it shows. | 20 |
| **4. Three amazing plots** | A mix of univariate and bivariate (a map is a great idea!). Titles, labels, legends, captions tied to your motivation. | 25 |
| **5. Conclusion** | 5 detailed bullets: what you found, what surprised you, what was hard, what you'd do next. | 10 |
| **GitHub process** | Team repo set up per the [guide](../1_GitHub_Portfolio_Guide.md#step-5-team-repos-for-projects-1-and-2): data uploaded to the repo, **≥5 meaningful commits** spread over the project, a README with team names and a 3-sentence summary. | 10 |
| | **Total** | **100** |

Your notebook must **Run All** with no errors. Sloppy code or missing captions lose points.

## AI on Project 1
Project 1 is your **Module 1 checkpoint**: **write the code yourselves.** You may use Claude as a *tutor* (to explain an error message or a concept), but not to write your code or text. If you used it, add one line to your README saying how. (Starting with Project 2, AI is expected, with a full AI log.)

## What to submit
In your team repo (`opim3510-project1-teamN`, with `drdave-teaching` added as a collaborator):
1. `Project1_CT_Data_Story.ipynb`: run top to bottom.
2. Your data files (CSV).
3. `README.md`: team names, 3-sentence summary, and how you used AI (if at all).

Submit the **repo link** in HuskyCT. **No NetIDs or student ID numbers anywhere in the repo.**
