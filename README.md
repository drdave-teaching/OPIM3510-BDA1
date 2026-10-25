![OPIM 3510 — Business Data Analytics I · Dr. Dave Wanik](opim3510_banner.svg)

# OPIM 3510 — Business Data Analytics I

**Dr. Dave Wanik · University of Connecticut · Spring 2027 (online, asynchronous)**

Everything for the course lives here: every notebook opens in **Google Colab** with one click, and every dataset loads straight from this repo, so there is nothing to install, download, or mount.

> 🚧 **Being rebuilt for Spring 2027.** Module 2 (forecasting) is the new version. Weeks 1–4 point to the Python Bootcamp, which is being refreshed. Module 3 still points to the previous version of the course.

## How to use this repo
1. Find the week below and click the notebook's **Colab** link.
2. In Colab, choose **File → Save a copy in Drive** (or, from Week 5 on, **Save a copy in GitHub**) so your changes are yours.
3. Run every cell, top to bottom. Read the markdown, not just the code.

## The semester at a glance

| Week | Module | Topic | Materials |
|---|---|---|---|
| 1 | **M1 Python Bootcamp** 🐍 | Welcome · Colab · Python basics | [Bootcamp: Data Wrangling](https://github.com/drdave-teaching/OPIM-Python-Bootcamp/tree/main/M1_1_DataWrangling) |
| 2 | M1 Python Bootcamp | pandas: tables, selecting, descriptive statistics | [Bootcamp: Data Wrangling](https://github.com/drdave-teaching/OPIM-Python-Bootcamp/tree/main/M1_1_DataWrangling) |
| 3 | M1 Python Bootcamp | Exploratory data analysis: plots that tell a story | [Bootcamp: Basic EDA](https://github.com/drdave-teaching/OPIM-Python-Bootcamp/tree/main/M1_2_BasicEDA) |
| 4 | M1 Python Bootcamp | Dirty data, missing values, joins | [Bootcamp: Dirty Data](https://github.com/drdave-teaching/OPIM-Python-Bootcamp/tree/main/M2_1_DirtyData) |
| 5 | **M1 Ship it** 🚀 | GitHub portfolio · meet Claude · Project 1 (EDA) | [`M1_Week05_GitHub_and_Claude`](M1_Week05_GitHub_and_Claude) *(coming soon)* |
| 6 | **M2 Forecasting** 📈 | Time-series data: Connecticut's electricity demand | [Open in Colab](https://colab.research.google.com/github/drdave-teaching/OPIM3510-BDA1/blob/main/M2_Forecasting/Week06_TimeSeriesData/1_CT_Electricity_Demand.ipynb) |
| 7 | M2 Forecasting | Baselines, moving averages, and how not to cheat | [Open in Colab](https://colab.research.google.com/github/drdave-teaching/OPIM3510-BDA1/blob/main/M2_Forecasting/Week07_Baselines_MovingAverages/1_CT_Baselines_and_Moving_Averages.ipynb) · bonus: [momentum trading](https://colab.research.google.com/github/drdave-teaching/OPIM3510-BDA1/blob/main/M2_Forecasting/Week07_Baselines_MovingAverages/bonus_MomentumTrading.ipynb) |
| 8 | M2 Forecasting | Exponential smoothing and Holt-Winters | [`Week08_ExponentialSmoothing`](M2_Forecasting/Week08_ExponentialSmoothing) *(coming soon)* |
| — | Spring break | | |
| 9 | M2 Forecasting | Project 2 | [`Week09_Project2`](M2_Forecasting/Week09_Project2) *(coming soon)* |
| 10 | **M3 Stats + Maps** 🗺️ | Distributions, sampling, the central limit theorem | [previous version](https://github.com/drdave-teaching/OPIM3510-notebooks/tree/master/Module3_Stats_Geospatial/1_Distributions) |
| 11 | M3 Stats + Maps | Confidence intervals and hypothesis tests | [previous version](https://github.com/drdave-teaching/OPIM3510-notebooks/tree/master/Module3_Stats_Geospatial/2_SamplingDistributions_CI) |
| 12 | M3 Stats + Maps | Geospatial data and maps | [previous version](https://github.com/drdave-teaching/OPIM3510-notebooks/tree/master/Module3_Stats_Geospatial/3_Geospatial) |
| 13 | M3 Stats + Maps | Joining Connecticut data to maps, census enrichment | [previous version](https://github.com/drdave-teaching/OPIM3510-notebooks/tree/master/Module3_Stats_Geospatial/3_Geospatial) |
| 14 | M3 Capstone | Project 3 and your portfolio repo | [previous version](https://github.com/drdave-teaching/OPIM3510-notebooks/tree/master/Module3_Stats_Geospatial/4_Putting_It_Together) |

## Module 2 in one sentence
One forecasting problem all module long, **forecasting Connecticut's daily electricity demand**, scored every week with the same `evaluate()` scorecard ([`M2_Forecasting/forecast_helpers.py`](M2_Forecasting/forecast_helpers.py)), where **error = predicted − actual** and every model has to beat the naive forecast.

## AI in this course
* **Weeks 1–4 (Python Bootcamp): no AI.** Learn to read and write basic Python yourself first.
* **Week 5 onward: AI is expected.** Claude Pro is required from Week 5. Disclose it, own every line, and verify everything you submit.
* Quizzes are always closed-AI.

## Data

| File | What it is |
|---|---|
| [`ct_demand_weather_hourly_2011_2021.csv`](data/ct_demand_weather_hourly_2011_2021.csv) | Hourly CT electricity demand (MWh) + Bradley Airport weather, 2011–2021 (raw, real-world problems left in on purpose) |
| [`ct_daily_demand_2011_2021.csv`](data/ct_daily_demand_2011_2021.csv) | The clean daily version built in Week 6 (GWh/day, average + max temperature) |
| [`ct_heating_oil_weekly_2019_2023.csv`](data/ct_heating_oil_weekly_2019_2023.csv) | Weekly CT retail heating oil prices, Oct 2019 – Oct 2023 |
| [`GLD.csv`](data/GLD.csv) | Daily prices for the GLD gold ETF, Nov 2004 – Oct 23, 2026 (saved from Yahoo Finance) |

## Previous version
The Spring 2024 materials are archived at [drdave-teaching/OPIM3510-notebooks](https://github.com/drdave-teaching/OPIM3510-notebooks).

— Dr. Dave Wanik · University of Connecticut
