# 🏏 IPL Data Analysis Dashboard (2008 - 
## 📌 Project Overview
This repository contains an interactive **Power BI Data Analytics Dashboard** designed to analyze historical Indian Premier League (IPL) data from 2008 to 2025. The project transforms complex ball-by-ball and match dataset into actionable visual insights, focusing on match statistics, team performances, toss analysis, and player achievements (Orange & Purple Cap analysis).
---
## 📸 Dashboard Preview
![IPL Analysis Dashboard](dashboard_preview.png)
---
## 🎯 Key Business & Analytical Insights
* **Toss Decision & Match Impact:** Analyzed win percentages based on toss decisions (Batting vs. Fielding first across seasons).
* **Top Scorers & Wicket Takers:** Visualized dynamic leaderboard for top run-getters (Orange Cap) and wicket-taking bowlers (Purple Cap).
* **Match Performance Tracking:** Drill-down table showing match-by-match toss winners, venue impact, and match results.
* **Key Metrics (KPIs):** High-level view of Total Matches played, Total Runs, Boundary counts (4s & 6s), and Total Venues hosted.
---
## 🛠️ Data Model & DAX Formulas
Key DAX measures and custom aggregations implemented in this report:
* **Total Boundaries:**
  ```dax
Total Boundaries = CALCULATE(COUNT(ball_by_ball[batsman_runs]), ball_by_ball[batsman_runs] IN {4, 6})
Total Wickets = CALCULATE(COUNT(ball_by_ball[is_wicket]), ball_by_ball[is_wicket] = 1)
**Next Step:**
README editor me pura pura text `Ctr
