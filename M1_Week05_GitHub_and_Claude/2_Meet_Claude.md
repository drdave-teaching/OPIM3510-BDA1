# Meet Claude: your pair programmer from Week 5 on

For four weeks you wrote every line yourself. That was on purpose: **you can only check AI-written code if you can read code.** Now you can. From here on, Claude is expected in this course: as a tutor when you're stuck, and as a pair programmer on projects.

## Get set up
* Sign up at **claude.ai** and subscribe to **Claude Pro** (required from Week 5; about \$20/month, and you can cancel after finals). If the cost is a hardship, email Dr. Dave and we'll work something out.
* Use it in your browser next to Colab: two windows side by side, or your second monitor.

## What Claude is good at (and not)
| 👍 Great at | 👎 Watch out for |
|---|---|
| Explaining an error message in plain English | Sounding confident when it's wrong |
| Explaining what a line of code does | Code that *runs* but quietly answers a different question |
| Suggesting a plot or a `groupby` for your question | Mixing up column names it hasn't seen |
| Turning your rough idea into working pandas | Time-series traps: forgetting `shift(1)`, using the test year |
| Rewording your memo for a non-technical boss | Making up facts or sources about your data |

## Two ways to use it
**1. Tutor: "help me understand"** (use this the most)
> *I'm learning pandas. This line gives `KeyError: 'Sale Price'`. Here's `df.columns`: [...]. What does the error mean and how do I find the right name?*

> *Explain this line to me like I'm new to Python: `daily['adjustment'] = daily['weekday'].map(weekday_avg)`*

**2. Pair programmer: "help me build"**
Give it **context**: what you're trying to do, what your data looks like, and what you already tried.
> *I have a pandas DataFrame `daily` with a datetime index and columns `Demand_GWh` and `Temp_avg` (daily, 2011–2021). I want a 1-day-ahead forecast that only uses information from before each day. Write code for a 3-day moving average forecast, and explain how it avoids using the future.*

Paste `df.head()` and `df.dtypes` (or `df.info()`) into your prompt so it knows your real column names.

## Always verify (this is the skill we grade)
Before you trust anything Claude gives you:
1. **Run it.** Does it work on *your* data?
2. **Check a few rows by hand.** Pick 3 rows and do the math yourself, or in Excel.
3. **Check the shape.** Did you lose or gain rows? (`df.shape` before and after.)
4. **Check for peeking.** Does any forecast use the same day's (or a future) value?
5. **Read every line.** If you can't explain a line, ask Claude to explain it, then check that explanation against the pandas docs.

## The rules (from the syllabus)
* **Disclose:** when AI materially shaped your work, say so in your AI log or commit message: which tool, and what it did.
* **Own it:** you must be able to explain every line you submit. Project walk-through videos ask you to explain code Dr. Dave picks. "The AI wrote it" isn't an answer.
* **Verify:** never submit AI output you haven't run and checked.
* **Your voice:** reflections and memos are written by you.
* **Quizzes are always closed-AI.**

## Keep these out of any AI chat
* Passwords, API keys, NetIDs, student ID numbers.
* Anyone else's personal information.
* Quiz questions.

## Your AI log
Every project from Project 2 on includes an **AI log** ([template](../M2_Forecasting/Week09_Project2/AI_LOG_template.md)): a few entries of *what you asked → what it gave you → was it right → how you checked*. Fill it in as you go, not the night before. You'll practice one entry in this week's notebook.
