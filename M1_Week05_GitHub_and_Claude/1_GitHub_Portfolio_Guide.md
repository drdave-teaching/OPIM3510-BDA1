# Your GitHub Portfolio (browser + Colab, nothing to install)

## Why bother? (read this first)
* **Your GitHub profile is proof.** Anyone can write "Python, pandas, data visualization" on a résumé. A recruiter who clicks your GitHub link sees the actual notebooks: your Connecticut home sales EDA, your electricity forecast that beat naive by 40%. That's the difference between *saying* you can do it and *showing* it.
* **No more `Project1_final_v3_REALLYFINAL.ipynb`.** GitHub keeps every version you save, with a note about what changed. Broke something? Go back to yesterday's version.
* **It's how real teams work.** Analytics teams share code in repositories like this, and so do AI coding tools like Claude Code. You'll use it the same way for your team projects.

By the end of this guide you'll have **a portfolio repo with your first notebook in it**, and you'll know how to set up a **team repo** for Projects 1 and 2.

---

## Step 1. Make an account (5 minutes)
1. Go to **github.com** and sign up.
2. Use your **personal email**, not your UConn email. This account should outlive your NetID, and your portfolio follows you to your first job.
3. Pick a **professional username**: `jane-smith`, `jsmith-data`. Not `xXbballfanXx`.
4. Add a profile photo and your name. (*Settings → Public profile*)

## Step 2. Create your portfolio repo
1. Click **+** (top right) → **New repository**.
2. **Repository name:** `opim3510-portfolio`
3. **Public** (it's a portfolio, so people should see it).
4. Check **Add a README file**.
5. Click **Create repository**.

Now edit the README (click the ✏️ pencil on `README.md`). Replace the text with a short intro, then click **Commit changes**:

```markdown
# Jane Smith · Data Analytics Portfolio
Business analytics student at UConn. Python, pandas, forecasting, and maps.

| Project | What I did |
|---|---|
| Your town in 10 lines | A quick look at home sales in my hometown |
```

🎉 That was your first **commit**: a saved version with a message.

## Step 3. Save a notebook from Colab straight to GitHub
1. Open the [Week 5 practice notebook](https://colab.research.google.com/github/drdave-teaching/OPIM3510-BDA1/blob/main/M1_Week05_GitHub_and_Claude/3_Week5_Practice_Your_Town.ipynb) in Colab and run it.
2. In Colab: **File → Save a copy in GitHub**.
3. The first time, Colab asks to **authorize GitHub**. Click through and allow it. (If you'll ever save to a *private* repo, check **Include private repos**.)
4. Pick **Repository:** `your-username/opim3510-portfolio`, **Branch:** `main`.
5. **File path:** `your_town.ipynb`
6. **Commit message:** something useful, like `Add home-sales snapshot for my town`.
7. Leave **Include a link to Colab** checked, then click **OK**.

Go to your repo on github.com and refresh. Your notebook is there, plots and all, with an **Open in Colab** badge at the top.

> **Opening it again later:** in Colab, **File → Open notebook → GitHub** tab → search your username → pick the notebook. When you're done, **Save a copy in GitHub** again. Every save is a new commit.

## Step 4. Write good commit messages
A commit message says *what changed and why*, in a few words.

| ❌ Not useful | ✅ Useful |
|---|---|
| `update` | `Add weekday-adjusted naive forecast` |
| `asdf` | `Fix shift so forecasts don't peek at the future` |
| `final` | `Add leaderboard and business memo` |

**Commit early, commit often.** Projects in this course require at least **5 meaningful commits spread over the project window**. Your history *is* your process: it shows how your work grew. One giant commit at 11:58 PM on the due date loses those points.

## Step 5. Team repos for Projects 1 and 2
One teammate does this, once per project:
1. Create a repo named like `opim3510-project1-team3`. Make it **Private** for now (you can make it public after grades are in, if your whole team agrees).
2. Check **Add a README file**.
3. **Settings → Collaborators → Add people:** add each teammate **and Dr. Dave (`drdave-teaching`)**. Everyone must accept the email invite.
4. **Upload data:** **Add file → Upload files** → drag in your CSVs → commit.
5. **Read data in Colab straight from the repo.** Open the CSV on github.com, click **Raw**, and copy that URL into `pd.read_csv(...)`.

> ⚠️ Raw links to **private** repos don't work from Colab. For a private team repo, keep the data in a **public** data repo, or upload the CSV to the Colab session (*Files panel → Upload*). For Projects 1 and 2, the course data is already public in this repo.

**Taking turns:** two people saving the *same notebook* at the same time can overwrite each other. Split the work into separate notebooks (`part1_cleaning.ipynb`, `part2_tables.ipynb`), or agree on whose turn it is.

## Step 6. Polish your profile (10 minutes, do it after Project 2)
* **Pin your best repos:** your profile → **Customize your pins** → pick your portfolio and projects. ([how](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/pinning-items-to-your-profile))
* **Profile README:** make a public repo named exactly like your username. Its README shows on your profile page. ([how](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme))
* Add the GitHub link to your résumé and LinkedIn.

## Never put these in a repo
* **Passwords, API keys, tokens.** Bots scan GitHub for them within minutes.
* **NetIDs, student ID numbers, grades,** or anyone's personal information.
* Big files (over about 50 MB). Ask Dr. Dave if your data is huge.
