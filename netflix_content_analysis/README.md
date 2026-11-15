<h1 align="left">🎬 Netflix Content Strategy Dashboard</h1>
<p align="left"><b>An interactive Tableau dashboard analyzing 8,807 Netflix titles</b></p>
---

## 📌 At a Glance

| | |
|---|---|
| **Tool** | Tableau Public |
| **Dataset** | Netflix Movies and TV Shows ([Kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows)) |
| **Records** | 8,807 titles, 12 columns |
| **Focus** | Catalog growth, genres, ratings, countries, movie length |

## 🎯 Business Question

> How has Netflix's catalog changed over time, and what kind of content does it add, from where, and for whom?

## 🔍 Key Insights

- 🎥 About **70%** of the catalog is movies and **30%** is TV shows
- 📈 Yearly additions grew sharply from 2016 and **peaked in 2019** at roughly 2,000 titles
- 🎭 **Dramas (1,600)** and **Comedies (1,210)** are the largest genres
- 🔞 **TV-MA (3,207)** is the largest rating, followed by **TV-14 (2,160)**, so the catalog leans toward teen and adult audiences
- 🌍 The **United States** is the largest source of content by a wide margin
- ⏱️ Movies added since 2018 average **about 100 minutes**

## 📊 Dashboard Contents

| Visual | What it shows |
|---|---|
| KPI cards | Total titles (8,807), movie share (70%), countries of origin (86) |
| Titles Added per Year | Catalog growth, split by Movie and TV Show |
| Movies vs TV Shows | Share of each content type |
| Titles by Country | World map of titles by country |
| Top 10 Genres | Most common genres |
| Content Ratings | Distribution of age ratings |
| Avg Movie Length | Average runtime by year added |

## ⚙️ Calculated Fields

| Field | Purpose |
|---|---|
| `Date Added (Date)` | Converts the text date into a real date |
| `Year Added` | Extracts the year for trend charts |
| `Movie Minutes` | Turns movie duration ("90 min") into a number |
| `TV Seasons` | Turns TV duration ("2 Seasons") into a number |
| `Primary Country` | Keeps the first listed country, so each title counts once |
| `Primary Genre` | Keeps the first listed genre, so each title counts once |
| `Pct Movies` | Share of titles that are movies (KPI) |
| `Countries Covered` | Distinct countries of origin (KPI) |

## 🖱️ Interactivity

Filter actions connect the charts. Click a **content type**, **genre** or **country** and every other chart and KPI card updates. Click an empty area to reset.

## 🧠 What I Learned

- Converting messy text fields (dates and durations) into usable data
- Handling cells that hold several values, such as multiple countries or genres
- Reading data honestly: 2021 looks incomplete, so I did not call it a decline
- Designing one dashboard that tells a single clear story

## ⚠️ Notes and Limitations

- Each title is counted under its **first-listed** country and genre, so totals add up to 8,807
- About 9% of titles have no country listed and are left out of the map
- Average movie length is by the year added to Netflix, not the release year
- Avg Movie Length is blank when TV Show is selected, because TV shows are measured in seasons
- The 2021 data appears to be partial

## 🚀 Possible Improvements

- Split titles that list several countries or genres
- Add a director analysis
- Add a quarterly trend view

## 📂 How to Open

1. Download `netflix_content_dashboard.twbx` from this folder
2. Open it in **Tableau Public** or **Tableau Desktop** (the data is packaged inside)

---

<sub>Independent portfolio project, not affiliated with Netflix. Dataset from Kaggle.</sub>
