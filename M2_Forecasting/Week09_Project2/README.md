# Project 2: Forecast Connecticut's Electricity Demand

**OPIM 3510 · Module 2 · Team project**

## The job
You're the forecasting team at a grid operator. Every morning you forecast **tomorrow's total electricity demand for Connecticut**. Your boss has one question: **can you beat the simple forecast we use today?**

* **Data:** [`data/ct_daily_demand_2011_2021.csv`](../../data/ct_daily_demand_2011_2021.csv): daily demand (GWh) and Bradley Airport temperature, 2011–2021.
* **Train:** 2011–2019. Use these years for *every* choice you make.
* **Test:** **2020**. Touch it once, at the end. (Yes, that's the COVID year. Part of your job is explaining what it did to your forecasts.)
* **Horizon:** 1 day ahead.

Start here: [**Open the starter notebook in Colab**](https://colab.research.google.com/github/drdave-teaching/OPIM3510-BDA1/blob/main/M2_Forecasting/Week09_Project2/Project2_Forecasting_CT_Demand.ipynb)

## What to do
| Part | What | Points |
|---|---|---|
| **A. Honest baselines** | Split by time. Build **naive**, **weekday-adjusted naive**, one **moving average** and one **exponential smoothing / Holt-Winters** model. Choose every setting (window, alpha) on 2011–2019 only. Score everything on 2020 with `evaluate()` and make a **leaderboard**. | 25 |
| **B. Beat it** | Try at least **one new idea** to beat your best baseline (ideas are in the notebook: weather, holidays, blending). Choices made on training years only. Report **skill vs. naive**. Grading is on an honest, well-explained attempt, not only on winning. | 25 |
| **C. Diagnose** | Plot your best model's errors over 2020. List the 10 worst days and explain them (COVID shutdown? holidays? heat waves?). | 15 |
| **D. Business memo** | 5 bullet points for a non-technical manager: which model, how accurate (in GWh *and* %), when it fails, and what you'd do next. | 10 |
| **Process** | **≥5 meaningful commits** in your team repo over the project window (5) · **AI log** (10) · **walk-through videos** (10). See below. | 25 |
| | **Total** | **100** |

## The rules (break one and the model doesn't count)
1. **Never peek at the future.** Every forecast for day *t* uses only data through day *t − 1*: use `shift(1)`.
2. **Choose on train, score on test.** No setting may be picked by looking at 2020.
3. **Weather is a special case.** You *may* use day *t*'s temperature **only if you say so** and call it what it is: *"assuming a perfect weather forecast."* Real day-ahead temperature forecasts miss by a few degrees, so your real-world accuracy would be a bit worse.
4. **Always report skill vs. naive.**

## What to submit
Push these to your **team's GitHub repo** and submit the repo link in HuskyCT:
1. `Project2_Forecasting_CT_Demand.ipynb`: run top to bottom, with headers, comments and plots.
2. `AI_LOG.md`: copy [the template](AI_LOG_template.md) and fill it in as you go, not the night before.
3. `README.md`: team names, one-paragraph summary of your best model, and links to each member's video.

## Walk-through videos (every team member)
After you submit, **Dr. Dave will email each of you a section of your notebook** (for example, *"cell 23: your weekday adjustment"*). Record a **3–5 minute** video (Kaltura or unlisted YouTube) explaining:
* what that code does, line by line,
* why it doesn't peek at the future,
* what would change if you changed one setting (a window, an alpha, a cutoff).

You may use AI to help write code. You may **not** use it to answer the video. If you can explain it, you own it.

## Grading notes
* A model that "beats" naive by peeking at the future gets **zero** for that model, so check your `shift()`s.
* A tidy loss is worth more than a messy win.
* Commits all made at 11:58 PM on the due date lose the process points.
