# 🎬 IMDb Cinema Analytics – Global Film Industry Trends

_A comprehensive data analysis of 100+ years of cinematic history, focusing on profitability, audience sentiment, and genre evolution using SQL, Python, and Tableu._

---

## 📌 Table of Contents
- [Overview](#overview)
- [Business Problem](#business-problem)
- [Dataset](#dataset)
- [Tools & Technologies](#tools--technologies)
- [Project Structure](#project-structure)
- [Data Cleaning & Preparation](#data-cleaning--preparation)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [KPIs & Key Research Findings](#kpis--key-research-findings)
- [Dashboard Highlights](#dashboard-highlights)
- [How to Run This Project](#how-to-run-this-project)
- [Final Strategic Recommendations](#final-strategic-recommendations)
- [Author & Contact](#author--contact)

---

## 📋 Overview
This project evaluates the performance of the film industry from 1920 to the present. By analyzing IMDb and Meta Scores alongside financial data, the project provides a data-driven roadmap for production houses and distributors to understand what makes a movie successful in both the "Critic's Eye" and the "Public's Pocket."

---

## ❓ Business Problem
Investing in film production is high-risk. This project aims to:
- Identify the most profitable genres and the optimal time for release.
- Correlate critical acclaim (Meta Score) with commercial success (Gross Revenue).
- Detect audience engagement trends based on voting volume.
- Analyze the impact of movie "Runtimes" and "Certificates" on market reach.

---

## 📊 Dataset
- **Primary Source:** IMDb 1000+ Movies Dataset.
- **Features:** Series Title, Released Year, Certificate, Runtime, Genre, IMDb Rating, Meta Score, Director, Stars, No. of Votes, and Gross Revenue.

---

## 🛠️ Tools & Technologies
- **SQL:** Data extraction, ranking (Window Functions), and filtering historical eras.
- **Python (Pandas, Seaborn, Matplotlib):** Statistical distribution analysis (Box Plots) and Word Cloud generation.
- **Tableu:** Interactive dashboarding with advanced DAX for KPI tracking.
- **GitHub:** Version control and documentation.

---

## 📂 Project Structure
```
imdb-cinema-analysis/
│
├── README.md
├── notebooks/                  # Python EDA & Visualizations
│   ├── imdb_data_cleaning.ipynb
│   └── genre_sentiment_analysis.ipynb
│
├── sql_queries/                # Transformation scripts
│   ├── top_performers_by_year.sql
│   └── profit_margin_estimation.sql
│
├── dashboard/                  # Tableu Dashboard
│   └── imdb_analytics_dashboard.twbx
│
└── images/                     # Screenshots for documentation
    └── dashboard_preview.png
```

---

## 🧹 Data Cleaning & Preparation
- **Handling Nulls:** Meta Scores and Gross Revenue columns were cleaned; missing values were imputed using median values or removed where necessary to maintain financial integrity.
- **Feature Engineering:** 
    - Extracted "Genre" into primary categories.
    - Converted "Runtime" from string (e.g., "142 min") to integer for numerical analysis.
- **Filtering:** Removed entries with incomplete historical data to prevent skewing the "Gross by Year" trend.

---

## 🔍 Exploratory Data Analysis (EDA)
- **Financial Growth:** A sharp exponential increase in **Gross Revenue** was identified post-2000, signaling the globalization of cinema.
- **Quality Distribution:** Box plots of **Meta Scores by Genre** revealed that "Biography" and "Drama" have the most consistent critical quality, while "Action" has the highest variance.
- **Popularity vs. Quality:** A strong correlation was found between the **Number of Votes** and commercial success, proving that audience engagement is a better predictor of profit than critical reviews.

---

## 📈 KPIs & Key Research Findings

1.  **Gross Revenue:** Tracked total earnings; identified the shift from niche artistic films to global blockbusters.
2.  **IMDb vs. Meta Score:** Discovered a "Sentiment Gap" where audiences often rate Action movies higher than critics do.
3.  **Voter Volume:** High-performing movies typically cross a threshold of **1M+ votes**.
4.  **Genre Frequency:** **Drama** is the most frequently produced genre (as seen in the Word Cloud), indicating high competition but steady demand.
5.  **Runtime Efficiency:** Most high-grossing films stay within the **120–150 minute** window; outliers like *3 Idiots* (170 min) succeed only with high IMDb ratings (8.4).
6.  **Certificate Reach:** "U" and "UA" certificates dominate the market volume, highlighting the importance of family-accessible content.

---

## 🖥️ Dashboard Highlights
<img src="dashboard%20screenshot/Screenshot%202025-12-28%20105037.png" width="600">

- **Total Gross by Release Year:** Area chart showing the financial evolution of cinema.

- **Meta Score Distribution:** Box-and-whisker plots for quality benchmarking.
 
- **Genre Word Cloud:** Visualizing market saturation and genre popularity.
  
- **Top 10 Rankings:** Dynamic lists of movies by Rating and Voter Engagement.

---

## 💡 Final Strategic Recommendations
- **Content Strategy:** Production houses should prioritize **Biographies/Dramas** for awards (High Meta Score) but look to **Action/Adventure** for maximum Gross Revenue.
- **The "Sweet Spot":** For a high ROI, target a **130-minute runtime** with a **UA Certificate** to maximize audience reach without losing engagement.
- **Investment Timing:** Focus on the "Modern Era" trends (post-2010), as audience voting behavior has shifted significantly toward digital interaction.

---

## 👤 Author & Contact
**PRANAY JHA**  
Data Analyst  
📧 Email: PRANAYJHA535@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/pranay-jha09/)  
