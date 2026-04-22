# Stephen Data Pivot — 12-Week AI Co-Work Curriculum

Author: Muse (Claude) for Jon Hayles / 247 Group
Date: 2026-04-21
Target learner: Stephen Branch (Treasury / Accounting → Data Analyst)
Philosophy: "It's 2026. We have to use the AI that will replace us."

---

## JOB 1 — URL Verification Report (verified 2026-04-21/22)

All checks run live. GitHub repos queried via `gh api`. Non-GitHub URLs verified via WebFetch, WebSearch, and curl HEAD where WebFetch was blocked. Reported fields: STATUS → last activity → license → fit judgment.

| # | URL | Status | Last Activity | License | Fit |
|---|---|---|---|---|---|
| 1 | https://github.com/microsoft/Data-Science-For-Beginners | LIVE | pushed 2026-04-14, 34.9k stars | MIT (confirmed) | KEEP — 10-week structure, MIT means we can fork whole-cloth |
| 2 | https://github.com/microsoft/ML-For-Beginners | LIVE | pushed 2026-04-20, 85.4k stars | MIT (confirmed) | KEEP — use as stretch content in weeks 10-12 |
| 3 | https://github.com/DataTalksClub/data-engineering-zoomcamp | LIVE | pushed 2026-04-20, 40.2k stars | NOASSERTION on license file (repo states Apache 2.0 in course body per prior agent; GitHub API returns null — INVESTIGATE for relicensing, but content is public and free to study) | INVESTIGATE license on a specific clone; KEEP for week 2 SQL content as reference only, don't redistribute wholesale |
| 4 | https://www.kaggle.com/learn/intro-to-sql | LIVE (confirmed via search) | Actively listed in Kaggle Learn 2026 catalog | Free + free cert offered | KEEP — core week 4 spine |
| 5 | https://www.kaggle.com/learn/advanced-sql | LIVE | Actively listed 2026 | Free + free cert | KEEP — core week 6 spine |
| 6 | https://www.kaggle.com/learn/pandas | LIVE | Actively listed 2026 | Free + free cert | KEEP — core week 10/11 spine |
| 7 | https://www.kaggle.com/learn/data-visualization | LIVE | Actively listed 2026 | Free + free cert | KEEP — core week 7 supplement |
| 8 | https://sqlbolt.com | LIVE | Site active, copyright 2024 on footer | Free, browser-interactive | KEEP — week 4 warm-up |
| 9 | https://www.db-fiddle.com | LIVE (WebFetch returned shell only; site resolves; widely used in 2026) | Active | Free, anonymous use | KEEP — sandbox for quick queries, with sqliteonline as primary |
| 10 | https://sqliteonline.com | LIVE | Changelog shows active dev through 2026, v0.7.83 | Free, browser sandbox | KEEP — primary SQL sandbox |
| 11 | https://public.tableau.com/app/resources/learn | LIVE (curl HEAD 200) | Tableau Public actively maintained 2026 | Free tier, downloadable workbooks | KEEP — week 7 primary |
| 12 | https://analytics.google.com/analytics/academy/ | LIVE (redirects to goo.gle/ga-courses → Skillshop) | Active, GAIQ cert valid 12 months | Free + free cert (GAIQ) | KEEP as optional stretch cert in week 8 |
| 13 | https://colab.research.google.com | LIVE | Free tier active 2026 with ~15-30 GPU hrs/week T4 | Free tier confirmed | KEEP — Python environment for weeks 10-12 |
| 14 | https://fred.stlouisfed.org | LIVE (curl HEAD 200) | Active, 840k series in 2026 | Public data, free API key | KEEP — treasury-domain datasets, Stephen's moat |
| 15 | https://fiscaldata.treasury.gov/ | LIVE (curl HEAD 200) | Active, no API key needed | Public domain | KEEP — Stephen's treasury angle goldmine |
| 16 | https://www.sec.gov/dera/data/financial-statement-data-sets | LIVE (curl returns 403 from bot; confirmed live via data.gov catalog metadata timestamp 2026-04-13) | Updated quarterly, current through 2026 | Public domain (US gov work) | KEEP — week 11 capstone data |
| 17 | https://corporatefinanceinstitute.com/course-catalog/?course_category=free | LIVE | Active, mixed free/paid | Free tier exists, certs paywalled | KEEP as optional supplement; do not rely on for core path |
| 18 | https://github.com/lerocha/chinook-database | LIVE | pushed 2025-10-05, 2.5k stars | NOASSERTION in GitHub metadata (prior agent claimed MIT — verify by reading LICENSE file directly before redistribution) | KEEP for classroom use; INVESTIGATE license before any public repo includes the DB files |
| 19 | https://github.com/microsoft/sql-server-samples | LIVE | pushed 2026-04-14, 11k stars | NOASSERTION (Microsoft custom license; historically MIT-like for samples — verify LICENSE.txt before redistributing Northwind/AdventureWorks schemas) | KEEP for reference; do not repackage wholesale |
| 20 | https://github.com/stefan-jansen/machine-learning-for-trading | STALE | pushed 2024-08-18 (20+ months stale), 17k stars | NOASSERTION (verify LICENSE.md in repo) | REPLACE for core content — use only as inspiration for Stephen's capstone; content still valuable but not actively maintained |

### Net call
17 of 20 KEEP as-is. 3 items need follow-up: Chinook license file verification, MS sql-server-samples LICENSE.txt read, ML-for-trading is stale (OK as inspiration, not foundation). Zero dead URLs. The curriculum can proceed.

---

## REPO README.md — Landing page Stephen sees when he forks

```markdown
# Stephen's Data Pivot — 12 Weeks to AI-Native Analyst

Welcome Stephen. This is your curriculum. Built by Jon Hayles and Muse (Claude)
specifically for you — a treasury/accounting pro pivoting into data analytics in 2026.

## The bet we are making

Bootcamp grads in 2026 learn tools. They come out knowing SQL syntax and how to
drag fields in Tableau. That's commodity. AI writes SQL now. AI builds dashboards now.

Your moat is two things bootcamp grads don't have:

1. **Real domain judgment.** You spent years reading financial statements,
   reconciling accounts, catching errors a spreadsheet couldn't see. That pattern
   matching does not come from a bootcamp. It comes from your career.

2. **AI co-work skill.** Knowing how to *command* an AI to write the SQL, build
   the viz, structure the analysis — and then validate the output against what
   you know is true about the business. That is the 2026 analyst skill.

This course drills both, every week, for 12 weeks.

## The rhythm

- **Solo learning:** 8-12 hrs/week reading, watching, doing exercises
- **AI co-work time:** 4-6 hrs/week pairing with Claude on that week's mini-project
- **Jon time:** 1 hr/week check-in, usually Sunday evening (voice or video)
- **Portfolio entry:** 1 shipped artifact per week, added to your public GitHub

Total: ~15 hrs/week. You're unemployed. You have the hours. Use them.

## What you ship

By week 12 you have a public GitHub portfolio with 12 entries:
3 spreadsheet/financial analyses, 3 SQL analyses, 3 dashboards, 3 Python/pandas
notebooks. Plus a capstone that ties everything together using real SEC or
Treasury data and your domain expertise.

This is what recruiters and hiring managers see. Bootcamp grads show 2-3
Kaggle-derivative projects. You show 12 weeks of progressive work with treasury
context.

## The five AI co-work skills

Every week drills one of these in a new context. By week 12 you've drilled each
~2-3 times:

1. **Translate business problem → data question** — what are we actually asking?
2. **Command AI to execute the data question** — prompt well, get working code
3. **Validate output against domain knowledge** — does this number even make sense?
4. **Iterate with AI to refine** — push back, correct course, add nuance
5. **Present the insight to non-technical stakeholders** — the story, not the SQL

These are not commands you memorize. They are habits. We build them in reps.

## How to use this repo

Start at `00_getting_started/01_what_is_ai_cowork.md`. Do not skip it.
Then work through phases in order. Each week folder has:

- `README.md` — the plan for the week
- `AI_COWORK_PATTERN.md` — specific prompting drills (this is the meta-skill)
- `exercises.md` — hands-on work
- `datasets.md` — where to pull data
- `stephen_portfolio_entry_template.md` — what you commit at week's end

## Before you start

- Claude Pro subscription ($20/mo — Jon will reimburse first 3 months)
- GitHub account (free)
- Google account for Colab and Kaggle
- LinkedIn profile updated to "Data Analyst in Training"
- A clean notebook or Obsidian vault for logging what you learn

## Commitment

This is a 12-week contract with yourself. Miss a week, push it back — don't
skip it. The sequence matters. Each week builds on the last.

Let's go.

— Jon & Muse
```

---

## 00_getting_started/

### 01_what_is_ai_cowork.md

```markdown
# What AI Co-Work Actually Is

## Stop thinking of Claude as a search engine

Most people treat Claude like Google with personality. They ask a question,
skim the answer, and move on. That is not co-work. That is lookup.

Co-work is different. Co-work is: I am doing a real piece of work, and Claude
is sitting next to me executing the parts it is faster at while I apply the
judgment it cannot. At the end we have a deliverable that neither of us could
have produced alone as efficiently.

## The five skills, unpacked

**1. Translate business problem → data question.**
Your boss says "our AR is climbing, why?" That is a business problem. It is
not a data question. The data question might be: *"For invoices aged 60+ days
in Q1 2026 vs Q1 2025, by customer segment, what is the distribution of
days-outstanding and has the mix shifted?"* You translate. Claude doesn't
know the business. You do.

**2. Command AI to execute the data question.**
Now you have the data question. You don't sit down and write SQL. You tell
Claude: *"I have a table called `invoices` with columns [...]. Write me a
query that returns [...], grouped by [...], with a flag when days outstanding
crosses 60. Use PostgreSQL syntax. Explain what each CTE does."* Claude
writes it. You read it.

**3. Validate output against domain knowledge.**
Claude returns SQL. You run it. The output says AR from Customer X is $4.2M.
You know Customer X's typical AR balance is $400K. Something is wrong.
Maybe a join duplicated rows. Maybe the filter is off. Maybe Customer X
really is in trouble. Your treasury brain catches this. A bootcamp grad
without your domain would ship the bad number.

**4. Iterate with AI to refine.**
You paste the output back: *"The $4.2M for Customer X is 10x their
historical AR. I suspect the join is duplicating. Show me row counts before
and after the join and check for a one-to-many relationship."* Claude digs.
You iterate until the number is trustworthy.

**5. Present the insight to non-technical stakeholders.**
Your CFO doesn't want SQL. She wants: *"AR is up 18% YoY, driven by two
mid-tier customers on extended terms. Recommend treasury follow up before
quarter close. One exception flagged for data-quality review."* That is the
deliverable. You wrote three sentences. Claude helped draft them. You
validated every claim.

## What this is not

It is not "I'll just ask Claude to do my job." Claude doesn't know your
company. Claude doesn't know your customers. Claude cannot tell you when a
number smells wrong. You can.

It is also not "I'll copy Claude's output without reading it." If you do
that in a real job, you will ship a bad number, and your career pivot ends
the same week it started.

## The habit to build this week

Every time you open Claude, before you type the prompt, write a single
sentence in your own notebook: *"I am trying to accomplish [X] and I need
Claude to help with [Y]."* If you can't finish the sentence, don't send the
prompt. Think more first.

This is the single habit that separates AI co-workers from AI users.
```

### 02_setting_up_claude_pro.md

```markdown
# Setting Up Claude Pro

## Why Pro, not free

Free Claude works for casual questions. Co-work is different. You will paste
large spreadsheets, run long analyses, share multiple documents. Free tier
caps you out mid-project. $20/mo is the cost of dinner. It pays for itself
the first week.

## Sign up

1. Go to https://claude.ai
2. Sign in with Google (use the email you'll use for this whole course)
3. Click Upgrade → Pro → $20/mo
4. Enable Projects (toggle in left sidebar)

## Create your first Project

Projects are Claude's memory across sessions. Make one called
**"Stephen Data Pivot"** with this system prompt:

> I am Stephen Branch, pivoting from treasury/accounting into data analytics.
> I am working through a 12-week curriculum. Help me think through problems
> and drill AI co-work skills. When I paste code or data, validate
> carefully. When I am wrong, tell me directly. Assume I have 10+ years
> finance/treasury domain expertise but I am learning SQL, pandas, and viz
> tools for the first time. Do not over-explain finance concepts. Do
> explain technical concepts patiently.

Upload to the Project:
- This course README
- The current week's README and AI_COWORK_PATTERN files
- Any datasets you are actively working on

## Desktop app vs web

Install the Claude desktop app. It handles long pastes better and keeps
your sessions organized. Web is fine as a backup.

## Prompting habits, day one

- Full sentences. Not keyword fragments.
- State your goal, state what you've tried, state what you want back.
- Push back when Claude is wrong. "That number doesn't match my domain
  expectation — show me how you derived it" is a valid, expected move.
- When Claude gives you code, paste the output back. Don't just trust it ran.

## What NOT to paste into Claude

- Real company data from a future employer — that's their IP
- PII (names, SSNs, account numbers)
- Anything you'd be uncomfortable seeing on a billboard

For the course: public datasets only (FRED, Treasury, SEC EDGAR, Chinook).
Safe by design.
```

### 03_how_this_course_works.md

```markdown
# How This Course Works

## Weekly rhythm

| Day | What |
|---|---|
| Mon | Read that week's README. Set up tools. 30 min with Claude planning the week. |
| Tue-Wed | Solo learning: 3-4 hrs each day on the resources list. |
| Thu | AI co-work block: 3-4 hrs pairing with Claude on the mini-project. |
| Fri | Finish mini-project. Draft portfolio entry. |
| Sat | Polish portfolio entry. Commit to GitHub. |
| Sun | 30-60 min with Jon. Review the week, preview next week. |

## Total time

~15 hrs/week minimum. Push to 20 if you want to finish stronger. You are
unemployed. Treat this as your 40-hour-a-week job, with the other 25 hours
on job search, LinkedIn, interview prep (see `resources/job_search_kit.md`).

## What "shipped" means

A portfolio entry is shipped when:

- It lives in a public GitHub repo
- It has a README explaining the problem, approach, findings
- It includes the code (SQL, notebook, or workbook link)
- It includes the deliverable (writeup, dashboard screenshot, or chart)
- The commit history shows Stephen learning — not Claude doing it alone

## How to handle struggling

If you are stuck for more than 30 minutes, do these in order:

1. Tell Claude exactly what's stuck and what you've tried
2. Read the week's AI_COWORK_PATTERN for guidance
3. Post in your notes what the blocker is, move on to another task
4. Bring it to Jon on Sunday

Do not grind alone for 4 hours. Time box everything.

## How to handle a week where life happens

Slide the week. Don't skip it. The course is sequential. Week 6 assumes
weeks 4 and 5. If you have a bad week, push the schedule right by one week.
Tell Jon. Don't ghost.

## Success metrics

By week 12 you have:
- 12 GitHub portfolio entries
- Kaggle certs in Intro SQL, Advanced SQL, Pandas, Data Visualization
- Updated LinkedIn with 3+ case studies written up as posts
- Mock-interviewed at least 5 times with Claude, 2 times with Jon
- Applied to 20+ analyst roles in weeks 10-12

That is a hire-able profile. Not a guarantee. A floor.
```

---

## Phase 1 — Foundation (Weeks 1-3)

### week_01_claude_as_pair_partner/README.md

```markdown
# Week 1 — Claude as Pair Partner

## Goals
- Build the habit of writing-before-prompting
- Drill skill #1: translate a business problem into a data question
- Ship a portfolio entry: "My treasury career in 5 analyses"

## AI co-work pattern this week
Skill #1: Translate business problem → data question.
See `AI_COWORK_PATTERN.md` for the full drill.

## Resources
- This week's readings in `00_getting_started/` (all 3 files, if not already done)
- Microsoft Data-Science-For-Beginners, Lesson 1 (Defining Data Science): https://github.com/microsoft/Data-Science-For-Beginners (MIT, confirmed live 2026-04-14)
- Jon's "Facts vs Opinions" rule (you'll see Muse cite it) — useful writing habit
- YouTube: StatQuest "Statistics Fundamentals" playlist (free, foundational)

## Mini-project
Write a 1,500-word document titled **"5 data questions I could have answered
in my last treasury job."** For each:
- State the business problem (2 sentences, plain English)
- State the data question (precise, SQL-able even if you can't write it yet)
- State what data you would have needed (tables, fields, grain)
- State what decision it would have informed

This is a stealth exercise. You are drilling skill #1 on territory you know
cold. By the end of the week you can translate any finance problem into a
data question. That skill is rarer than SQL syntax.

## Portfolio entry this week
`portfolio/week_01_five_treasury_questions.md` — the document above, with a
short intro explaining who Stephen is and why this matters. This is your
first public GitHub commit.

## Time budget
- 2 hrs: read the 3 `00_getting_started` files + this README
- 3 hrs: MS DS-for-beginners Lesson 1 + 1 StatQuest video per day
- 5 hrs: draft, iterate, polish the 5 questions document with Claude
- 2 hrs: portfolio entry + GitHub setup + first public commit
- 1 hr: Sunday with Jon
- Total: 13 hrs, light week by design — we are building the habit infrastructure

## How this builds forward
Every subsequent week you will translate new problems into data questions.
This week you do it on home turf (treasury) so the translation mechanics
are clear. Weeks 4+ you'll do it with unfamiliar domains (retail, music
sales, public debt) and the skill has to work there too.
```

### week_01_claude_as_pair_partner/AI_COWORK_PATTERN.md

```markdown
# AI Co-Work Pattern — Week 1

## The skill: Translate business problem → data question

## The drill

For each of your 5 treasury questions, run this exact sequence with Claude:

### Step 1 — You write, alone, no AI

In your notebook, write:
- Business problem (1-2 sentences)
- First-cut data question (1 sentence, as precise as you can)

Do not open Claude yet. Write it yourself first. This is the muscle.

### Step 2 — You paste to Claude and ask for critique

Prompt template:

> I am trying to translate a treasury business problem into a precise data
> question. Here is my attempt.
>
> Business problem: [yours]
> Data question: [yours]
>
> Critique the data question on three dimensions:
> 1. Is it precise enough that someone could write SQL against it?
> 2. What ambiguity remains (dates, grain, filters, definitions)?
> 3. What are 2-3 follow-up data questions that would make this analysis
>    more useful?
>
> Do not rewrite my question for me. Point at the gaps. I will rewrite.

### Step 3 — You rewrite, alone again

Based on Claude's critique, rewrite YOUR data question. Don't paste
Claude's version. Paste YOUR rewrite back for final check.

### Step 4 — You validate

Prompt template:

> Here is my rewritten data question: [yours v2]
>
> Act as a data engineer who just received this as a ticket. What clarifying
> questions would you ask before writing SQL?

If the engineer-Claude has zero clarifying questions, your question is
tight. If they have 3+, your question needs more work.

## Why this pattern

The temptation with Claude is to hand over the problem and get the answer.
That is not the skill. The skill is: you write, Claude critiques, you
revise, Claude stress-tests, you revise. You stay the author. Claude is a
senior engineer reviewing your work, not a junior doing it for you.

Once this pattern feels natural, you use it on every analysis task for the
rest of your career.

## Trap to avoid

"Claude, what data questions should I write for treasury?"
That's lookup, not co-work. You'd get generic answers. Your real lived
experience generates better questions than Claude's training data can.
```

### week_02_advanced_sheets_excel/README.md

```markdown
# Week 2 — Advanced Sheets & Excel (AI-Assisted)

## Goals
- Level up Excel/Sheets beyond what you used in treasury: INDEX/MATCH,
  XLOOKUP, dynamic arrays, LAMBDA, pivot tables with calculated fields
- Drill skill #2: command AI to execute a data question (formulas this week)
- Build muscle memory for "describe what I want, get a formula, validate it"

## AI co-work pattern this week
Skill #2: Command AI to execute. You describe a transformation in plain
English, Claude returns a formula, you paste into Sheets, you validate.

Sample drill:

> I have a Google Sheet with columns A=invoice_date, B=customer, C=amount,
> D=paid_date. I want a formula in column E that returns "days to pay"
> when D is populated, "open - [N] days" when D is blank and A is more
> than 30 days old, and "current" otherwise. Write me the formula.

That is a skill #2 rep. Do 20 of them this week.

## Resources
- Microsoft Excel/Sheets advanced tutorials (YouTube: ExcelIsFun, free)
- Google Sheets Advanced Formulas cheat sheet (searchable)
- Dataset: pick a public M&A transaction log or SEC quarterly filings CSV
  from https://www.sec.gov/data-research/sec-markets-data/financial-statement-data-sets (public domain, live 2026)
- FRED for macro context: https://fred.stlouisfed.org (live 2026, free API key)

## Mini-project
Build a **Treasury Operations Dashboard Workbook**. Tabs:
1. Raw AP/AR data (you fabricate this — 500 rows, realistic)
2. Aged receivables pivot (with calculated fields)
3. Cash flow forecast (12 weeks forward, using rolling averages)
4. Variance vs prior period (XLOOKUP-based)
5. Executive summary (written narrative, pulls numbers from tabs 2-4 via cell references)

Every formula gets a comment explaining what it does. Every calculation
gets Claude-assisted, then manually verified against a second method.

## Portfolio entry
`portfolio/week_02_treasury_ops_dashboard/` — workbook exported as .xlsx,
plus a README explaining the structure and one screenshot of the exec
summary tab.

## Time budget
- 4 hrs: advanced formula tutorials
- 2 hrs: build the raw data (realistic fake data, 500 rows)
- 5 hrs: build the analysis tabs, pair with Claude on every formula
- 2 hrs: exec summary narrative, portfolio commit
- 1 hr: Jon Sunday
- Total: 14 hrs

## How this builds forward
Week 4 moves the same operations to SQL. You will find SQL easier because
you already thought through the transformations in formulas. The translation
from "I want this calculation" to "here is the SQL" becomes automatic.
```

### week_03_financial_analysis_formalized/README.md

```markdown
# Week 3 — Financial Analysis Formalized

## Goals
- Translate your treasury instincts into standard financial analysis vocab:
  ratio analysis, variance analysis, DuPont, common-size statements,
  trend decomposition
- Drill skill #3: validate AI output against domain knowledge
- Position your resume/LinkedIn to name-drop these frameworks

## AI co-work pattern this week
Skill #3: Validate. Claude is going to tell you things about financial
statements. Some will be right. Some will be wrong or oversimplified. Your
job: catch the bad ones.

Example drill:

> Claude, explain the DuPont identity and give me a worked example on
> Apple's FY2024 financials.

Claude returns an explanation with numbers. You open Apple's actual 10-K
(via SEC EDGAR) and check: did Claude use real numbers? Are the ratios
computed right? Is the interpretation correct?

Report back: "You said ROE = 170%. I pulled the actual 10-K and got 157%.
Show me where the discrepancy is." Iterate.

## Resources
- Corporate Finance Institute free tier: https://corporatefinanceinstitute.com/course-catalog/?course_category=free (confirmed live; free tier has intros, certs are paid — use only the free content)
- SEC EDGAR: https://www.sec.gov/edgar/searchedgar/companysearch (public domain)
- Aswath Damodaran's free YouTube lectures (NYU Stern prof, gold standard)
- Financial Times free-tier articles for current-events ratio analysis

## Mini-project
Pick 3 public companies (1 strong, 1 mediocre, 1 struggling — Stephen's
pick, your call based on treasury instincts). Pull their last 3 years of
10-Ks from SEC EDGAR. For each:
- Compute 8 core ratios (liquidity, leverage, efficiency, profitability)
- DuPont decomposition of ROE
- Common-size income statement
- Variance analysis YoY
- 500-word "treasury reviewer's note" — what would you flag for the CFO?

Three companies × 4 analyses × 500 words = a real analyst deliverable.

## Portfolio entry
`portfolio/week_03_three_company_ratio_analysis/` — one PDF per company
plus a comparative overview document. This is the first portfolio entry
that looks like hire-able analyst work.

## Time budget
- 3 hrs: CFI free tier + Damodaran for framework
- 2 hrs: pull 10-Ks, organize data
- 7 hrs: analysis + Claude-assisted calculations + validation drills
- 2 hrs: portfolio writeups
- 1 hr: Jon Sunday
- Total: 15 hrs

## How this builds forward
Weeks 4-9 put these analyses on SQL foundations and build dashboards that
automate them. The reasoning you drilled this week becomes the logic you
encode in SQL next week.
```

---

## Phase 2 — SQL (Weeks 4-6)

### week_04_sql_basics/README.md

```markdown
# Week 4 — SQL Basics with Claude at Your Side

## Goals
- SELECT, WHERE, ORDER BY, LIMIT, basic aggregates (COUNT, SUM, AVG, GROUP BY)
- Finish Kaggle Intro to SQL (get the cert)
- Drill skill #2 in a new context: command AI to write SQL
- Build: "I can query a database I've never seen before" confidence

## AI co-work pattern this week
Skill #2 in SQL form. See `AI_COWORK_PATTERN.md`.

Core move: you describe the schema and the question, Claude writes SQL,
you run it against the real DB (sqliteonline or BigQuery sandbox), you
validate, you iterate.

Sub-habit: always ask Claude to explain each clause. You are not here to
copy-paste. You are here to read SQL fluently by end of week 6.

## Resources
- SQLBolt: https://sqlbolt.com (live, browser-interactive, free, no signup)
- Kaggle Intro to SQL: https://www.kaggle.com/learn/intro-to-sql (live 2026, free, cert)
- Microsoft DS-for-Beginners Lessons 6-8 (SQL with Python)
- Sandbox: https://sqliteonline.com (live 2026, active dev through v0.7.83)
- Fallback sandbox: https://www.db-fiddle.com
- Sample database: Chinook (from https://github.com/lerocha/chinook-database — MIT per project docs; verify LICENSE file on clone before redistributing)

## Mini-project
Using the Chinook database, answer these 10 questions in SQL:
1. Top 10 customers by total spend
2. Top 5 genres by revenue
3. Monthly revenue trend for 2012-2013
4. Average invoice size by country
5. Employee with the highest customer retention (repeat buyers)
6. Tracks that have never been purchased
7. Artists with >50 tracks but <$100 revenue (catalog depth vs commercial success)
8. Revenue concentration — what % of revenue comes from top 10% of customers?
9. Median invoice size by customer segment (hint: SQL medians are a drill)
10. Month-over-month growth rate, with a flag when growth < -5%

Every query comes with:
- The SQL
- A plain-English description of what it does
- A treasury-brain interpretation: "if this were my company, what would I do with this answer?"

## Portfolio entry
`portfolio/week_04_chinook_analysis.md` — all 10 questions, SQL, output
snippets, interpretations.

## Time budget
- 3 hrs: SQLBolt front-to-back
- 4 hrs: Kaggle Intro to SQL (earn the cert)
- 5 hrs: 10 questions on Chinook, Claude-paired
- 2 hrs: portfolio writeup
- 1 hr: Jon Sunday
- Total: 15 hrs

## How this builds forward
Week 5 adds joins, which is where SQL gets real. Week 6 adds window
functions and CTEs, which is where analyst-grade SQL lives. You'll use
the Chinook schema across all three weeks so the data stops being the
thing you're learning and SQL becomes the thing you're learning.
```

### week_04_sql_basics/AI_COWORK_PATTERN.md

```markdown
# AI Co-Work Pattern — Week 4

## The skill: Command AI to execute a data question (in SQL)

## The drill — "SDQS" loop: Schema → Data question → Query → Validate → Stress-test

### S — Schema first, always

When you start a Claude session about a new database, paste the schema
first. Every time. Not from memory. Paste the actual CREATE TABLE
statements or a sample row from each table.

Prompt template:

> Here is the schema for the Chinook database: [paste]
>
> Here is a sample row from the Customer table: [paste]
>
> I am going to ask SQL questions against this schema. Before you write
> any SQL, confirm you understand the relationships between Customer,
> Invoice, InvoiceLine, and Track.

Claude confirms. Now you proceed. This prevents 80% of Claude's SQL errors.

### D — Data question, precisely stated

> Question: What are the top 10 customers by total lifetime spend,
> including customer email, country, and total spend. Order by spend
> descending. If two customers tie, break the tie by earliest first purchase.

That level of precision. Not "show me top customers." Be the engineer who
writes tickets other engineers don't have to ask questions about.

### Q — Query from Claude

> Write the SQL. Explain each clause in plain English after the query.
> Use SQLite syntax (for sqliteonline.com).

Read it. Don't just copy. If a clause doesn't make sense, ask.

### V — Validate in the sandbox

Paste into https://sqliteonline.com with Chinook loaded. Run it. Check:
- Did it return the expected number of rows (10)?
- Do the numbers pass a smell test? (If a customer's spend is $50M, red flag.)
- Would you trust this output in a real report?

### S — Stress-test

Paste the output back to Claude:

> Here is the output of your query: [paste]. One thing I want to validate:
> can you show me the raw invoices for Customer #1 so I can manually sum
> them and confirm the total is correct?

Make Claude prove the number. Always.

## Why this pattern works

SQL mistakes are silent. A wrong JOIN returns numbers that look right.
The only defense is validation. The SDQS loop forces it.

## Mental habit to build

When Claude hands you a query, the first thought should not be "does
this run?" It should be "do these numbers match what I expect?" That
question is the difference between an analyst and a typist.
```

### week_05_joins_aggregations/README.md

```markdown
# Week 5 — Joins, Aggregations, and the "It Looked Right But Wasn't" Trap

## Goals
- INNER, LEFT, RIGHT, FULL OUTER joins — when each is right
- Multi-table aggregations (GROUP BY with joins, HAVING)
- Catching the classic "duplicated rows from a one-to-many" bug
- Drill skill #3: validate AI output when SQL LOOKS right but isn't

## AI co-work pattern this week
Skill #3: Validate, specifically against the silent-duplication trap.

Claude will sometimes write a query that returns $4.2M when the right
answer is $420K because a JOIN duplicated rows. Your job this week:
build the habit of always running `SELECT COUNT(*)` before and after
the join and sanity-checking.

Full drill in this week's pattern doc.

## Resources
- Kaggle Intro to SQL (remaining lessons if not finished last week)
- SQLBolt intermediate lessons
- MS sql-server-samples (https://github.com/microsoft/sql-server-samples — check LICENSE.txt before redistributing; use in-sandbox for learning)
  - Northwind database as 2nd sample schema
- YouTube: "Visual JOINs explained" (any of several good 10-min videos)

## Mini-project
Cross-database analysis: answer 8 questions that require joining 3+ tables
in Chinook and 8 in Northwind. Then write a 500-word reflection titled
"The duplicated-row bugs I caught and how I caught them."

## Portfolio entry
`portfolio/week_05_joins_deep_dive.md` — 16 questions, queries, outputs,
plus the bug-reflection essay.

## Time budget
- 4 hrs: joins tutorials + practice
- 6 hrs: 16 questions Claude-paired
- 3 hrs: bug reflection + portfolio
- 1 hr: Jon Sunday
- Total: 14 hrs

## How this builds forward
Week 6 adds window functions and CTEs on top of joins. If your joins are
shaky, week 6 falls apart. Get this solid.
```

### week_06_analyst_grade_sql/README.md

```markdown
# Week 6 — Analyst-Grade SQL: CTEs, Window Functions, Subqueries

## Goals
- CTEs (WITH clauses) for readable multi-step analysis
- Window functions: ROW_NUMBER, RANK, LAG, LEAD, moving averages
- Correlated subqueries (know they exist, mostly avoid them)
- Finish Kaggle Advanced SQL (get the cert)
- Drill skill #4: iterate with AI to refine a multi-step analysis

## AI co-work pattern this week
Skill #4: Iterate. This week's problems are multi-step. First query
returns something. You realize you need to refine. You push back. You
refine again. You build a 5-CTE query through 4 rounds of iteration.

Reps teach you that your first prompt is almost never the right one,
and that's OK. Iteration is the skill.

## Resources
- Kaggle Advanced SQL: https://www.kaggle.com/learn/advanced-sql (live 2026, free, cert)
- Mode Analytics SQL tutorials (free, advanced)
- DataTalksClub zoomcamp Week 1/2 materials (https://github.com/DataTalksClub/data-engineering-zoomcamp — license unclear on GitHub metadata, use as reference not redistribution)
- Window functions visual guide (search for Lukas Eder's posts)

## Mini-project
The **Treasury Forecast Query**. Using Chinook extended (or Northwind):
- Build a single SQL query that returns, for each customer:
  - Total lifetime spend
  - Spend in each of the last 4 quarters (pivot-like)
  - 4-quarter moving average
  - Quarter-over-quarter growth rate
  - Rank within their country by total spend
  - Flag if their spend in the most recent quarter is <50% of their 4-quarter MA
- Use CTEs liberally. The final query should be readable top-to-bottom.
- Add comments explaining what each CTE computes.

This is a real analyst query. You can screenshot it in an interview.

## Portfolio entry
`portfolio/week_06_treasury_forecast_query.sql` + a README walking a hiring
manager through the logic. This is one of your strongest artifacts.

## Time budget
- 5 hrs: Kaggle Advanced SQL + cert
- 6 hrs: the forecast query, iterated 3-4 rounds with Claude
- 3 hrs: README walkthrough + portfolio
- 1 hr: Jon Sunday
- Total: 15 hrs

## How this builds forward
Weeks 7-9 build dashboards on top of SQL like this. The queries become
the data source for visualizations. Without analyst-grade SQL, the
dashboards are shallow.
```

---

## Phase 3 — Visualization (Weeks 7-9)

### week_07_dashboard_fundamentals/README.md

```markdown
# Week 7 — Dashboard Fundamentals with Tableau Public

## Goals
- Chart type literacy: when to use what (bar vs line vs scatter vs area vs heatmap)
- Tableau Public end-to-end: connect, build, publish
- Principles of non-terrible dashboard design (Stephen Few, Cole Knaflic)
- Drill skill #5: present the insight to non-technical stakeholders (viz edition)

## AI co-work pattern this week
Skill #5: Present. Viz is presentation. Claude helps you critique drafts
and articulate the story. See `AI_COWORK_PATTERN.md`.

Specific move: build a dashboard. Screenshot it. Paste to Claude with:

> I built this dashboard for a CFO audience. Critique it on: clarity,
> cognitive load, chart choices, and whether the story lands in 10
> seconds of viewing. Be direct. Do not soften feedback.

Claude gives critique. You iterate.

## Resources
- Tableau Public free: https://public.tableau.com (live 2026, free downloads, workbooks downloadable from community)
- Tableau training videos: https://www.tableau.com/learn/training (free tier)
- Kaggle Data Visualization: https://www.kaggle.com/learn/data-visualization (live 2026, free, cert)
- Cole Knaflic "Storytelling With Data" blog (free, principles-focused)
- Viz of the Day from Tableau Public — daily inspiration

## Mini-project
Using FRED data (https://fred.stlouisfed.org — live 2026, free API key),
build a **"Macro Weather Report" dashboard** showing:
- US unemployment rate (trend, 5 years)
- CPI (trend, 5 years, with Fed target overlay)
- 10Y-2Y Treasury spread (trend, with recession flag)
- GDP growth YoY (bars)
- One executive-summary text box pulling your interpretation

Publish to Tableau Public. Share the link.

## Portfolio entry
`portfolio/week_07_macro_weather_report/` — link to published dashboard,
screenshot, 300-word interpretation doc, link to the .twbx workbook.

## Time budget
- 4 hrs: Tableau training + Kaggle viz
- 2 hrs: FRED data pulls, cleaning
- 6 hrs: dashboard build, 3 rounds of Claude-assisted critique
- 2 hrs: publish + portfolio writeup
- 1 hr: Jon Sunday
- Total: 15 hrs

## How this builds forward
Week 8 applies these principles to a business/ops dashboard (non-macro).
Week 9 is portfolio week — assembling everything into a cohesive analyst
brand.
```

### week_07_dashboard_fundamentals/AI_COWORK_PATTERN.md

```markdown
# AI Co-Work Pattern — Week 7

## The skill: Present the insight to non-technical stakeholders

## The drill — "Ten-Second Test"

A dashboard fails if a CFO walks past your monitor and cannot state the
headline insight in 10 seconds. That's your standard.

### Round 1 — Build

Build a first draft of your dashboard. Don't polish. Just get the charts
on screen with real data.

### Round 2 — Screenshot, paste, critique

Prompt template:

> I built a dashboard titled [title] for a [CFO / treasury lead / ops
> manager] audience. The core question they want answered is: [question].
>
> I am going to describe the dashboard (since you can't see images clearly):
> - Chart 1: [type, variables, what it shows]
> - Chart 2: [...]
> - ...
> - Summary text: [verbatim]
>
> Critique on four dimensions:
> 1. Ten-second test: can a viewer state the headline insight in 10s?
> 2. Cognitive load: too many charts? redundant info?
> 3. Chart-type choices: is each one the right fit for the underlying data?
> 4. Story arc: does the dashboard answer the question, or just display data?
>
> Be direct. Bootcamp grads over-decorate. I don't want polish. I want clarity.

### Round 3 — Rewrite the executive summary

Prompt template:

> Based on my dashboard, write 3 candidate 40-word executive summaries.
> Each should:
> - Lead with the headline insight
> - Include one supporting number
> - End with a recommended action
>
> I will pick one, edit it, and paste it onto the dashboard.

### Round 4 — Second-pass critique

Re-screenshot. Re-critique. Stop when Claude says "this lands."

## Why this pattern

Dashboards fail because builders fall in love with their charts. Fresh
eyes catch it. Claude is fresh eyes on demand.

## Trap to avoid

Do not ask Claude to design the dashboard from scratch. You design. Claude
critiques. You stay the designer. This is the pattern for the rest of your
career — AI does not replace your design judgment, it stress-tests it.
```

### week_08_business_dashboards/README.md

```markdown
# Week 8 — Business Dashboards (Ops, Finance, Sales)

## Goals
- Build 2 full dashboards on business data (not macro)
- Learn dashboard wiring: drill-downs, parameters, filter actions
- Add Google Analytics Academy cert as resume flex (optional, free, ~6 hrs)
- Drill skill #1 + #5 together: translate a CFO question into a dashboard

## AI co-work pattern this week
Combination pattern. Skill #1 (translate problem → question) at the top
of the week, skill #5 (present) at the bottom. Full round trip.

## Resources
- Tableau Public (continuation)
- Google Analytics Academy: https://skillshop.withgoogle.com/ (live 2026, free, GAIQ cert valid 12 months) — optional, but a resume line
- Kaggle Data Visualization cert (if not already earned)
- Stephen Few "Show Me the Numbers" — classic, used copies cheap

## Mini-project — two dashboards
1. **AR Aging Dashboard** — using Chinook or fabricated data, build a
   dashboard for a treasury lead showing AR by age bucket, by customer
   segment, with drill-down to invoice detail
2. **Revenue Performance Dashboard** — using Chinook, build a sales-style
   dashboard showing revenue by genre/country/month with parameter-driven
   comparisons

Each dashboard gets a 300-word "CFO brief" written alongside.

## Portfolio entry
`portfolio/week_08_two_business_dashboards/` — links to both published
dashboards, screenshots, CFO briefs, a "how I'd deploy this in a real
company" paragraph each.

## Time budget
- 3 hrs: advanced Tableau (parameters, actions)
- 3 hrs: Google Analytics Academy (optional cert)
- 6 hrs: two dashboards
- 2 hrs: portfolio
- 1 hr: Jon Sunday
- Total: 15 hrs

## How this builds forward
Week 9 takes all 8 weeks of work and packages it as a portfolio website
with writeups. You start applying to jobs at end of week 9.
```

### week_09_portfolio_assembly/README.md

```markdown
# Week 9 — Portfolio Assembly & Job-Search Launch

## Goals
- Consolidate weeks 1-8 into a coherent public portfolio (GitHub Pages
  site or Notion public page)
- Update LinkedIn to data analyst positioning with weekly case studies
- Draft master resume + 2 tailored versions (FP&A analyst, treasury
  analyst)
- Apply to 10+ roles by end of week

## AI co-work pattern this week
Skill #5 at the meta level. Claude helps you craft the narrative of your
career pivot. You are the subject-matter expert on your own career.
Claude edits. You write.

Key drill:

> Here is the story I want to tell on my LinkedIn "About" section.
> [paste your draft]
>
> Critique it on three dimensions:
> 1. Does it explain the pivot without apologizing for it?
> 2. Does it show domain expertise + AI-native skill as a combined moat?
> 3. Would a hiring manager read it all the way through?
>
> Do not rewrite it. Point at specific sentences that fail each test.

## Resources
- GitHub Pages docs (free portfolio site)
- `resources/job_search_kit.md` in this repo
- LinkedIn profile examples from strong analysts (search "data analyst
  Denver" or your target market)

## Mini-project
- Portfolio site live (GitHub Pages or Notion public)
- LinkedIn fully updated — headline, About, featured section with 3 case studies
- Master resume + 2 tailored versions
- 10 applications submitted

## Portfolio entry
This week the portfolio IS the entry. No separate write-up.

## Time budget
- 4 hrs: portfolio site build (static HTML or Notion, not fancy)
- 3 hrs: LinkedIn rewrite + case study posts
- 3 hrs: resume work
- 3 hrs: 10 applications (researched, tailored, not spray-and-pray)
- 1 hr: Jon Sunday
- Total: 14 hrs

## How this builds forward
Weeks 10-12 you learn Python/pandas + capstone while actively interviewing.
The applications you send this week are likely to produce interviews around
weeks 11-12. You will be mid-capstone when your first interviews happen.
That's a feature, not a bug — fresh skills, real projects to discuss.
```

---

## Phase 4 — Python & Capstone (Weeks 10-12)

### week_10_python_pandas_basics/README.md

```markdown
# Week 10 — Python & Pandas Foundations

## Goals
- Python syntax (variables, control flow, functions, list/dict comprehensions)
- pandas DataFrame fundamentals (read_csv, filter, groupby, merge)
- Google Colab as your working environment
- Drill skill #2 again, new context: command AI to write pandas

## AI co-work pattern this week
Skill #2 in pandas. You describe the transformation. Claude writes the
pandas. You run it in Colab. Validate. Iterate.

Key difference from SQL: pandas errors are noisier. Read the traceback.
Ask Claude to explain the error in plain English before blindly fixing.

## Resources
- Kaggle Python course (if Python is new to Stephen): https://www.kaggle.com/learn/python (live, free, cert)
- Kaggle Pandas: https://www.kaggle.com/learn/pandas (live 2026, free, cert)
- Google Colab: https://colab.research.google.com (live 2026, free T4 tier)
- MS Data-Science-For-Beginners Python section
- MS ML-For-Beginners as stretch (https://github.com/microsoft/ML-For-Beginners — MIT, pushed 2026-04-20)

## Mini-project
Redo the Chinook SQL analysis from week 4 in pandas. Same 10 questions.
Different tool. Now you can translate between SQL and pandas fluently —
which is most of what pandas interviews test.

## Portfolio entry
`portfolio/week_10_chinook_in_pandas.ipynb` — Jupyter notebook, published
via Colab public link + committed to GitHub. Include a reflection:
"Which tool was better for each question and why."

## Time budget
- 3 hrs: Kaggle Python (skip if Stephen has Python)
- 4 hrs: Kaggle Pandas + cert
- 5 hrs: Chinook-in-pandas rebuild
- 2 hrs: reflection writeup
- 1 hr: Jon Sunday
- Total: 15 hrs

## How this builds forward
Week 11 adds analytics-grade pandas (time series, merges, reshaping).
Week 12 is capstone using real SEC or FRED data.
```

### week_10_python_pandas_basics/AI_COWORK_PATTERN.md

```markdown
# AI Co-Work Pattern — Week 10

## The skill: Command AI to execute (pandas edition)

## The drill — "Load, Describe, Transform, Validate"

### L — Load

Prompt:

> I am loading [dataset] in a pandas DataFrame called df. Here are the
> first 3 rows (with column names): [paste df.head().to_string()]
>
> Here is df.info(): [paste]
>
> Confirm you understand the dtypes and any nulls before we do anything.

Claude confirms. Critical because pandas silently coerces types and Claude
needs to know what's actually in memory, not what it assumes.

### D — Describe what you want

Not code. English.

> I want to group df by [column], aggregate [columns] using [operations],
> filter to rows where [condition], and return the top 10 by [column].
> Return the result as a new DataFrame called top10.

### T — Transform (Claude writes code)

> Write the pandas code. Include comments on any non-obvious choices.
> Explain what dtypes the result will have.

### V — Validate

Run in Colab. Then:

> Here is the output: [paste top10.head(10).to_string()]
>
> Two validation questions:
> 1. Do the row count and shape match what I'd expect? (yes/no)
> 2. If I re-ran the same logic in SQL, would I get the same result?
>    Walk me through how you'd verify that.

Always make Claude walk the cross-check. This is the muscle.

## Why this pattern

pandas is more forgiving than SQL (errors scream instead of silently
returning wrong data) but also more seductive — it's easy to write 10
lines of pandas that each look right but compound into a wrong answer.
The LDTV loop slows you down enough to catch compounded errors.

## Trap to avoid

"Claude, just analyze this CSV for me."
Too vague. Claude will do something — probably not what you want. You
stay in control. Claude executes. Always.
```

### week_11_pandas_analytics/README.md

```markdown
# Week 11 — Analytics-Grade Pandas

## Goals
- Time series in pandas (resample, rolling windows, shift)
- Reshaping (pivot, melt, stack, unstack)
- Merging multiple sources (pandas' equivalent of JOINs)
- Visualization directly from pandas (matplotlib basics)
- Drill skill #4 again: iterate with AI on multi-step analyses

## AI co-work pattern this week
Skill #4. You build a 3-step analysis. First pass fails or is wrong.
You push back with Claude. Second pass better. Third pass right.

The habit: when Claude's first answer is 70% right, don't rewrite it
yourself — describe what's wrong and let Claude patch. But never accept
50% right. Keep pushing.

## Resources
- Kaggle Pandas (finish if not done)
- Wes McKinney's "Python for Data Analysis" (free online chapters)
- Stefan Jansen ML-for-Trading (https://github.com/stefan-jansen/machine-learning-for-trading — last push 2024-08, use as reference/inspiration only, stale but high-quality content)
- YouTube: Corey Schafer pandas playlist (free, excellent)

## Mini-project
**Treasury Liquidity Monitor** — using FRED data (https://fred.stlouisfed.org)
pull 5 years of:
- 3-month Treasury yield
- 10-year Treasury yield
- Effective Federal Funds Rate
- CPI
- Unemployment rate

Build a Colab notebook that:
- Loads all 5 series via API
- Aligns them on a common date index (resample monthly)
- Computes yield-curve spread, real interest rate (FFR - CPI)
- Rolling 3-month and 12-month correlations between series
- Plots with matplotlib
- Outputs a "current state" summary pandas can print as a table

## Portfolio entry
`portfolio/week_11_treasury_liquidity_monitor.ipynb` — notebook + 500-word
writeup of your interpretation (the treasury-brain commentary is what
separates this from a bootcamp grad's notebook).

## Time budget
- 4 hrs: pandas time series study
- 6 hrs: build the monitor, iterate with Claude
- 3 hrs: interpretation writeup + portfolio commit
- 1 hr: Jon Sunday
- Also: 1-3 hrs on active interviews if scheduled
- Total: 14-17 hrs

## How this builds forward
Week 12 capstone pulls everything together. Week 11's notebook is a
component of the capstone.
```

### week_12_capstone/README.md

```markdown
# Week 12 — Capstone: "Treasury Insights from Public Data"

## Goals
- Ship a capstone project that demonstrates all 5 AI co-work skills
  applied across SQL, pandas, and Tableau
- Write a 2,000-word case study pitched at hiring managers
- Close out the 12-week sprint with a complete public portfolio

## AI co-work pattern this week
All 5 skills. This is the black-belt test.

## Resources
- Your own portfolio (weeks 1-11)
- FRED: https://fred.stlouisfed.org
- Treasury Fiscal Data: https://fiscaldata.treasury.gov
- SEC EDGAR: https://www.sec.gov/data-research/sec-markets-data/financial-statement-data-sets

## Capstone brief
**"Is the US Treasury under liquidity stress in 2026?"**

A fictional CFO of a mid-market manufacturer wants to understand whether
there are signals in public Treasury data that should change how they
think about cash management over the next 12 months. You are the analyst
they hired to answer that.

Deliverables:
1. **Data layer (SQL).** Load 3+ Treasury datasets into a local SQLite
   or DuckDB. Build 5 queries that extract the core time series.
2. **Analysis layer (pandas).** Notebook that joins the sources, computes
   5+ derived metrics (spreads, rolling stats, flags).
3. **Presentation layer (Tableau).** Published dashboard summarizing the
   findings for a non-technical CFO audience.
4. **Case study write-up (2,000 words).** Problem statement, approach,
   findings, recommendations, limitations. Published on your portfolio
   site and LinkedIn.
5. **Demo video (5 min, optional but powerful).** Screen-record yourself
   walking through the analysis. Post to LinkedIn.

## Portfolio entry
`portfolio/capstone_treasury_liquidity/` — all 4 deliverables + demo
video link. This is the flagship of your portfolio.

## Time budget
- 20+ hrs on the capstone (you may go over 15 this week — it's worth it)
- 3 hrs on active job search / interviews
- 1 hr with Jon (final Sunday check-in — review the whole pivot)
- Total: 24+ hrs

## After week 12
- You have a complete portfolio and an active job search.
- Keep applying. Keep interviewing. Keep adding one polished portfolio
  entry every 2-3 weeks while you hunt.
- The course ends. The career starts.
```

---

## Resources

### resources/verified_resources.md

(See the URL verification table at the top of this document. That content
is the source of truth. This file in the repo is the same table plus these
additional notes:)

**Re-verify before week starts:**
- Kaggle course URLs — Kaggle occasionally reorganizes
- SEC EDGAR dataset — updated quarterly, URL stable but file paths shift
- Tableau Public — community URLs (Viz of the Day) rotate

**Licenses to verify on clone:**
- Chinook database LICENSE file (GitHub metadata says NOASSERTION; project docs historically say MIT — read actual LICENSE before redistributing in portfolio repos)
- MS sql-server-samples LICENSE.txt
- DataTalksClub zoomcamp — some components MIT, some not; check per-folder

**Stale but useful:**
- stefan-jansen/machine-learning-for-trading (last push 2024-08) — excellent content, use as reference, don't treat as actively maintained

### resources/ai_cowork_prompt_library.md

```markdown
# AI Co-Work Prompt Library

Reusable prompt patterns. Adapt freely.

## Skill #1 — Translate business problem → data question

### Critique-my-translation
> I am trying to translate a business problem into a data question.
>
> Business problem: [yours]
> My data question: [yours]
>
> Critique on: precision, ambiguity, follow-up questions that would
> strengthen the analysis. Do not rewrite my question. Point at gaps.

### Engineer-stress-test
> Here is my data question: [yours]
> Act as a data engineer receiving this as a ticket. What clarifying
> questions would you ask before writing code?

## Skill #2 — Command AI to execute

### SQL — SDQS loop
> Schema: [paste CREATE TABLEs or equivalent]
> Sample rows: [paste 1 row per table]
> Question: [precise]
> Write the SQL in [SQLite / PostgreSQL / BigQuery] syntax. Explain each
> clause. Note edge cases.

### Pandas — LDTV loop
> DataFrame shape: [df.info() paste]
> First rows: [df.head() paste]
> I want to: [describe transformation in English]
> Write the pandas. Explain each step. Note dtype implications.

### Excel/Sheets
> Sheet structure: columns A=[], B=[], ... rows 2-N.
> I want a formula in column [X] that [describes logic].
> Write the formula. Explain each function. Note what happens on edge
> cases (empty cells, mismatched types).

## Skill #3 — Validate

### Cross-check
> Here is [query / function / formula] output: [paste]
> Two validation questions:
> 1. Do the row count / shape / magnitude match my domain expectation?
> 2. Walk me through how to cross-check this result with an independent
>    method.

### Smell-test
> The output says [X]. My domain knowledge says I'd expect roughly [Y].
> The gap is [gap size]. Help me figure out whether the output is wrong
> or my expectation is stale. What would you check first?

## Skill #4 — Iterate

### Patch-don't-rewrite
> Your previous answer was 70% right. The issue is [specific problem].
> Keep the correct parts. Fix only [specific issue]. Show me the diff
> vs the previous version.

### Add-a-dimension
> Extend the previous analysis to also [new dimension]. Do not redo the
> earlier work. Build on it.

## Skill #5 — Present

### Ten-second test
> Audience: [CFO / ops lead / non-technical exec]
> Dashboard described: [list of charts + summary text]
> Core question they want answered: [question]
>
> Critique on: 10-second insight, cognitive load, chart choices, story arc.
> Do not soften feedback.

### Executive summary drafts
> Based on the analysis above, draft 3 candidate 40-word executive
> summaries. Lead with headline, include one supporting number, end with
> recommended action.

## Meta-skill — Session hygiene

### Start-of-session
> I am working on [this week's goal]. My current context:
> [paste relevant files / previous work]
> Today's objective: [one sentence]
> Let's plan the next 2 hours.

### End-of-session
> Summarize what we accomplished in this session. What's open? What
> should I pick up on first thing tomorrow? Flag anything I should
> double-check before committing to portfolio.
```

### resources/job_search_kit.md

```markdown
# Job Search Kit

Runs in parallel with weeks 9-12.

## LinkedIn — rewrite checklist

### Headline (under 220 chars)
Template:
> Data Analyst | Former Treasury/Accounting Lead | SQL, Python, Tableau |
> AI-Native Analyst Building Next-Gen Finance Insights

Avoid: "aspiring", "seeking", "in training" — these signal weakness.
You are a data analyst. You started in treasury. Own it.

### About section — 3 paragraphs

Paragraph 1 — who you are:
> Former treasury and accounting professional with 10+ years closing
> monthly books, managing cash positions, reconciling across multi-entity
> structures. I read financial statements the way most people read
> newspaper headlines.

Paragraph 2 — the pivot:
> In 2026 I made a deliberate move into data analytics. Not because
> treasury is dying — it isn't — but because the analyst role is
> changing. Companies need people who combine domain expertise with the
> ability to command AI tools to do the grunt work. My 12 weeks of
> immersive project-based training built exactly that skill set.

Paragraph 3 — what you bring:
> I ship analyst deliverables in days instead of weeks because I pair
> with Claude, ChatGPT, and Copilot throughout the workflow. I don't
> just use AI. I command it, validate it, and apply domain judgment on
> top. That's the 2026 analyst stack. Let's talk.

### Featured section
Pin 3 portfolio entries with 1-paragraph write-ups each. Rotate as you
produce stronger ones.

## Resume — format

- 1 page for 0-10 years experience, 2 pages max
- Skills section lists: SQL, Python (pandas), Tableau, Excel/Sheets,
  AI-assisted workflows (Claude, ChatGPT), Google Colab, plus your
  finance domain
- Experience section rewrites your treasury bullets to emphasize analysis,
  not operations. "Reconciled X" → "Designed reconciliation workflow
  that caught $X variance across Y entities"
- Projects section lists 3-5 from your portfolio with 1-line descriptions

## Application rhythm (weeks 9-12)

- 10 applications/week minimum, 20 max
- Each one tailored — change summary, adjust 3-5 bullets, match keywords
- Track in a spreadsheet: company, role, date applied, source, status,
  follow-up date

## Interview prep

### Mock interviews with Claude
> I am interviewing for a data analyst role. Give me 3 technical SQL
> questions at [junior / mid] level. After I answer each, critique my
> answer and show me the ideal solution.

Rotate through: SQL, pandas, viz critique, case-study walkthroughs.

### Mock interviews with Jon
Every 2 weeks during weeks 10-12. Jon plays hiring manager. Real-time
feedback on voice, pacing, confidence, BS detection.

### Case studies to master
Three from your portfolio. Know the data, the approach, the decisions,
the limitations, and what you'd do differently. Practice the walkthrough
until it's 5 minutes tight.

## Target companies (mid-market analyst roles, 2026)

Denver / Raleigh / Austin / Nashville / Charlotte / Jacksonville —
mid-market financials, regional banks, insurance, REITs, logistics,
any industry where treasury/cash-mgmt matters. You fit best where your
domain is an asset, not just SQL.

Avoid (initially):
- FAANG — they hire bootcamp pipeline, hard to break in without a
  traditional path
- Pure SaaS startups — they want product analysts, different skill tree

Target:
- Mid-market CFO orgs hiring their first dedicated analyst
- Corp finance teams adding an analyst to an existing group
- Treasury-as-a-service firms
- Consulting firms with a finance analytics practice

## When to take the first offer

Rough rule: if it's $10-20K below your treasury peak, but it's a real
analyst title at a company with growth, take it. The 2-year follow-up
role will pay above your treasury peak. Your pivot is the investment.

If it's a title that's "Data Specialist" or "Jr. Analyst" but pays
reasonably and the team has analysts you can learn from, take it.

Do not take: any role that sounds like treasury wearing a data hat. The
pivot only works if the new role is actually analytical.
```

### resources/dataset_inventory.md

```markdown
# Dataset Inventory

Curated datasets for Stephen's curriculum. All public, all free, all
relevant to treasury/finance domain.

## Tier 1 — Use throughout course

### Chinook Database
- URL: https://github.com/lerocha/chinook-database
- License: project docs state MIT; GitHub metadata NOASSERTION — verify LICENSE file before redistributing
- What it is: sample music-store DB (11 tables, realistic relationships)
- Why it's good: small enough to understand, rich enough to ask analyst
  questions. Customer, Invoice, InvoiceLine, Track, Album structure mirrors
  typical B2C businesses.
- Used in: weeks 4, 5, 6, 10

### Northwind Database
- URL: https://github.com/microsoft/sql-server-samples (Northwind subfolder)
- License: verify LICENSE.txt in repo before redistributing
- What it is: classic Microsoft sample DB, wholesale/distribution
- Why it's good: 2nd schema to prove you can query databases you haven't seen
- Used in: week 5

## Tier 2 — Treasury/finance domain (Stephen's moat)

### FRED — Federal Reserve Economic Data
- URL: https://fred.stlouisfed.org
- License: public data, free API key (instant signup)
- What's there: 840,000+ economic time series, sourced from 119 public/private orgs
- Why it's good: macro context for everything. Interest rates, unemployment,
  inflation, GDP, yield curves.
- Used in: weeks 7, 11, 12

### US Treasury Fiscal Data
- URL: https://fiscaldata.treasury.gov/
- License: public domain (US government)
- What's there: debt-to-the-penny, daily/monthly Treasury statements,
  public debt, revenue collections, exchange rates
- Why it's good: literal treasury data. Perfect for Stephen's capstone.
  No API key needed, simple REST API.
- Used in: week 12 capstone

### SEC EDGAR Financial Statement Data Sets
- URL: https://www.sec.gov/data-research/sec-markets-data/financial-statement-data-sets
- License: public domain (US government)
- What's there: structured XBRL financial statement data for all publicly
  traded companies, updated quarterly
- Why it's good: you can do ratio analysis across hundreds of companies
  at once. Great for the week 3 project.
- Used in: weeks 3, 11 (optional), 12

### Yahoo Finance (unofficial via yfinance library)
- URL: used via `pip install yfinance`
- License: use is tolerated; not official public API
- What's there: stock prices, fundamentals, dividends
- Why it's good: easy pull of historical prices for any ticker
- Used in: weeks 11-12 as optional supplement
- Caveat: not guaranteed, Yahoo can break the library anytime

## Tier 3 — Stretch / inspiration

### Kaggle competitions archive
- URL: https://www.kaggle.com/competitions?listOption=completed
- License: varies per competition
- What's there: structured ML competitions with provided datasets
- Used in: only if Stephen wants to stretch into ML in week 11-12

### Stefan Jansen ML-for-Trading repo
- URL: https://github.com/stefan-jansen/machine-learning-for-trading
- License: verify LICENSE.md
- What's there: very good applied-finance notebooks
- Caveat: last push 2024-08, stale. Use for inspiration only.

## What to avoid

- Any dataset Stephen has from a prior employer. That is their IP.
- Personal financial data (his own or family). PII risk.
- Scraped data from live websites without reading their ToS. Lots of
  traps there. Stick to official APIs.

## Datasets to fabricate

For weeks 2 (sheets) and 5 (joins practice), Stephen should fabricate
small realistic datasets (500-1000 rows). Fabrication forces him to
think about what "realistic" means — a useful domain-judgment muscle.
Claude can help generate fake data with `faker` or a prompt template.
```

---

## Appendix — How Jon uses this document

1. Fork a new GitHub repo: `github.com/247group/stephen-data-pivot`
   (or personal org — whatever Stephen can own long-term)
2. Create the directory structure in the tree above
3. Paste each section of this document into the appropriate file
4. Share the repo with Stephen on Day 1
5. Sunday check-ins: open the week's README together, review last
   week's portfolio entry, preview next week's AI co-work pattern
6. Iterate — this is v1. Weeks 5-12 will sharpen as Stephen's real
   learning patterns emerge.

## Appendix — Sources cited during verification

- https://github.com/microsoft/Data-Science-For-Beginners
- https://github.com/microsoft/ML-For-Beginners
- https://github.com/DataTalksClub/data-engineering-zoomcamp
- https://github.com/lerocha/chinook-database
- https://github.com/microsoft/sql-server-samples
- https://github.com/stefan-jansen/machine-learning-for-trading
- https://www.kaggle.com/learn (catalog landing; individual courses listed)
- https://sqlbolt.com
- https://sqliteonline.com
- https://www.db-fiddle.com
- https://public.tableau.com/app/resources/learn
- https://www.tableau.com/learn/training
- https://skillshop.withgoogle.com/
- https://colab.research.google.com
- https://fred.stlouisfed.org
- https://fred.stlouisfed.org/docs/api/fred/
- https://fiscaldata.treasury.gov/
- https://fiscaldata.treasury.gov/api-documentation/
- https://www.sec.gov/data-research/sec-markets-data/financial-statement-data-sets
- https://catalog.data.gov/dataset/financial-statement-data-sets
- https://corporatefinanceinstitute.com/course-catalog/?course_category=free

End of document.
