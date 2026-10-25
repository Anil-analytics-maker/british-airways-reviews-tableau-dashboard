# ✈️ British Airways Reviews: Tableau Dashboard

An interactive Tableau dashboard that analyzes 1,324 British Airways customer reviews (2016–2023) to show how passengers rate the airline across overall experience, cabin staff, food, entertainment, ground service, seat comfort and value for money.

🔗 **Live dashboard:**[ (https://public.tableau.com/app/profile/anil.anil4778/viz/BritishAirwaysReviewsDashboard_17929426825700/Dashboard1)](https://public.tableau.com/app/profile/anil.anil4778/viz/BritishAirwaysReviewsDashboard_17929426825700/Dashboard1)



---

## 📸 Dashboard Preview

![Dashboard overview](images/dashboard-overview.png)

| Aircraft view | Country map | Monthly trend |
|---|---|---|
| ![Aircraft](images/aircraft-sheet.png) | ![Map](images/map-sheet.png) | ![Month](images/month-sheet.png) |

---

## 📌 Project Overview

- ✅ Connected two data sources in Tableau: customer reviews and a country-continent lookup table
- ✅ Built a parameter-driven dashboard where one selector switches every chart between 7 rating metrics
- ✅ Created KPI cards, a monthly trend line, a country map, and aircraft bar charts with review counts
- ✅ Added filters for date range, seat type, traveller type, continent and aircraft group

---

## 📁 Dataset

| File | Description |
|---|---|
| `ba_reviews.csv` | 1,324 reviews, 19 columns, March 2016 to October 2023 |
| `Countries.csv` | 251 countries with code, continent and region |

### Key columns

| Column | Description |
|---|---|
| `rating` | Overall rating (1 to 10) |
| `seat_comfort`, `cabin_staff_service`, `food_beverages`, `ground_service`, `value_for_money`, `entertainment` | Sub-ratings (1 to 5) |
| `place` | Country of the reviewer |
| `aircraft` | Aircraft type flown |
| `seat_type` | First, Business, Premium Economy or Economy |
| `traveller_type` | Solo Leisure, Couple Leisure, Family Leisure or Business |
| `date`, `date_flown` | Review date and flight date |

---

## 🔧 How the Dashboard Was Built

1. **Data connection:** joined `ba_reviews.csv` with `Countries.csv` on country name, so every review gets a continent and region (all 1,324 reviews matched).
2. **Data preparation:** grouped similar aircraft models into an **Aircraft Group** field, and treated the -1 placeholder in the sub-rating columns as missing values so averages are not distorted.
3. **Metric selector:** created a parameter, **Pick a metric**, and a calculated field, **Metric Selected**, so one control changes the trend line, map and aircraft charts together.
4. **Worksheets:** Summary (KPI cards), Month (trend), Map (country view) and Aircraft (rating plus number of reviews).
5. **Dashboard:** combined the worksheets with the metric selector, date slider, and traveller type, seat type, continent and aircraft group filters.

---

## 🔑 Key Findings

- **Volume:** 1,324 reviews from 56 countries about 150 aircraft types. 64% of reviews come from the UK, and Europe makes up 76%.
- **Overall rating:** the average is 4.19 out of 10, and 33% of reviews give the lowest score of 1.
- **Decline over time:** the average rating fell from 4.61 in 2017 to 2.61 in 2023.
- **Aircraft (50+ reviews):** Boeing 747-400 is the best rated (4.69) and A321 the lowest (3.59).
- **Seat type:** Business Class averages 3.93, lower than First Class (4.39) and Economy (4.36).
- **Service areas (out of 5):** cabin staff service scores highest (3.3) and food & beverages lowest (2.7).

---

## 🛠️ How to Use

1. Open the live dashboard using the link at the top.
2. Use **Pick a metric** to switch between overall rating and the six sub-ratings.
3. Filter by date range, seat type, traveller type, continent or aircraft group.
4. To explore the workbook itself, download `british-airways-reviews.twbx` and open it in Tableau Public (free).

> ⚠️ The numbers in the top banner change with the filters you select. Key findings above use the full dataset with no filters.

---

## 🧰 Tools Used

Tableau Public • Excel/CSV • GitHub

---

## 👨‍💻 About Me

Hi, I'm **Anil**, a B.Tech Civil Engineering student at Delhi Technological University, building a career in data analytics with SQL, Python, Excel, Power BI and Tableau.

## 🚀 Let's Connect

- 💼 LinkedIn: https://www.linkedin.com/in/anildtu27
- 💻 GitHub: https://github.com/Anil-analytics-maker
- 📧 Email: anil_23bt012@dtu.ac.in
