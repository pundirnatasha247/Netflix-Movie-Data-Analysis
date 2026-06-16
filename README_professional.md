# 🎬 Netflix Movie Data Analysis Dashboard

![Netflix](https://img.shields.io/badge/Netflix-E50914?style=for-the-badge&logo=netflix&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

---

## 📌 Project Overview

Netflix has one of the largest movie libraries in the world — but what stories does the data tell?

In this project, I explored a dataset of **9,827 Netflix movies** to find patterns in genres, popularity scores, vote ratings, and release trends over the years. The data was first cleaned and transformed using **Python (Pandas)** in Jupyter Notebook, and then visualized through an interactive **Power BI dashboard** with a Netflix-inspired dark theme.

This project covers the full data analysis pipeline — from raw messy data to a clean, insightful dashboard — making it easy to answer questions like:
- Which genre dominates Netflix?
- Which year saw the most releases?
- What kinds of movies are most popular?

---

## 📁 Project Structure

```
📦 Netflix-Movie-Data-Analysis
 ┣ 📓 movie_data_analysis_netflix.ipynb   # Jupyter Notebook - Data Cleaning
 ┣ 📄 netflix_cleaned.csv                 # Cleaned & Transformed Dataset
 ┣ 📊 Netflixproject.pbix                 # Power BI Dashboard File
 ┗ 📝 README.md                           # Project Documentation
```

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Python** | Programming language |
| **Pandas** | Data cleaning & transformation |
| **Jupyter Notebook** | Development environment |
| **Power BI Desktop** | Dashboard & visualization |
| **CSV** | Data storage & transfer |

---

## 🔄 Data Cleaning Steps

The raw dataset `mymoviedb.csv` contained **9,827 movies** with these columns:
`Release_Date`, `Title`, `Overview`, `Popularity`, `Vote_Count`, `Vote_Average`, `Original_Language`, `Genre`, `Poster_Url`

### Steps performed in Jupyter Notebook:

1. **Removed unnecessary columns** — `Overview`, `Original_Language`, `Poster_Url`
2. **Extracted year from date** — `2021-12-15` → `2021`
3. **Categorized Vote_Average** into 4 groups:
   - `not_popular` → lowest ratings
   - `below_avg` → below average
   - `Average` → moderate ratings
   - `Popular` → highest ratings
4. **Split Genre column** — one movie with multiple genres was exploded into separate rows
5. **Removed NaN values** — cleaned incomplete records
6. **Exported** cleaned data to `netflix_cleaned.csv`

> 📌 Result: 9,827 movies → **25,552 rows** after genre explosion

---

## 📈 Key Findings

| Insight | Finding |
|---------|---------|
| 🎭 Most Popular Genre | **Drama** (3,715 movies) |
| 😂 2nd Most Popular | **Comedy** (3,006 movies) |
| 💥 3rd Most Popular | **Action** (2,652 movies) |
| 📅 Peak Release Year | **2021** (most movies released) |
| 🌟 Highest Avg Popularity | **Adventure** genre |
| 🗳️ Vote Distribution | Almost equal across all 4 categories (~25% each) |
| 🎬 Total Movies | **9,827** |
| 🏷️ Total Genres | **19** unique genres |
| 🔥 Max Popularity Score | **5,084** |

---

## 📉 Power BI Dashboard Features

### 📦 KPI Cards
- **Total Movies** — 25.552K
- **Maximum Popularity** — 5.08K
- **Total Genres** — 19
- **Peak Year** — 2021

### 📊 Charts
1. **Movies Count by Genre** — Clustered Horizontal Bar Chart
2. **Vote Average Distribution** — Donut Chart
3. **Movies Released Per Year** — Line Chart
4. **Average Popularity by Genre** — Horizontal Bar Chart

### 🎛️ Interactive Filter
- **Genre Slicer** — Filter all visuals by selecting any genre

---

## 🚀 How to Run This Project

### Jupyter Notebook
```bash
pip install pandas
jupyter notebook movie_data_analysis_netflix.ipynb
```

### Power BI Dashboard
1. Download [Power BI Desktop](https://powerbi.microsoft.com/downloads/)
2. Open `Netflixproject.pbix`
3. Explore the interactive dashboard!

---

## 📦 Dataset

- **Source:** TMDB Movie Database
- **Original File:** `mymoviedb.csv`
- **Total Records:** 9,827 movies
- **Cleaned Records:** 25,552 rows (after genre split)

