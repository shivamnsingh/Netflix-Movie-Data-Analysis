# 🎬 Netflix Movie Data Analysis Project: Exploring Catalog Trends


A comprehensive **Data Science & Analytics** project exploring deep insights from over **25,000 Netflix movie records**. This analysis showcases the complete data pipeline—from cleaning and preprocessing to exploratory data analysis (EDA) and visualization using Python—to reveal how **genres, popularity, and release trends** shape Netflix’s vast movie catalog.

## ✨ Features & Highlights

* **25,552** Movie Records Analyzed.
* **Genre-level** analysis (handling multi-genre films).
* **Custom Binning** of `Vote_Average` for better categorical analysis.
* Identification of **Popularity Extremes** and **Outlier Detection**.
* Focus on answering key business questions about content strategy.

## 🧠 Project Overview

Netflix is a leader in using data science, AI, and machine learning to build world-class recommendation systems. This project applies data analysis techniques to a large public dataset to answer critical questions about the content available:

| **Business Question** | **Analysis Goal** |
| :--- | :--- |
| **1. Most Frequent Genre?** | Understand the dominant content type on the platform. |
| **2. Highest-Voted Genres?** | Identify genres that resonate most strongly with viewers. |
| **3. Highest/Lowest Popularity Movie?** | Find the extremes to understand the skewness of the catalog. |
| **4. Peak Release Year?** | Determine which years saw the maximum surge in content production/acquisition. |

---

## 💾 Dataset Details

* **Source:** `mymoviedb.csv`
* **Total Initial Rows:** 25,552
* **Key Columns Used:**
    * `Release_Date` (Year extracted)
    * `Title`
    * `Popularity`
    * `Vote_Count`
    * `Vote_Average` (Transformed into 4 ordinal bins)
    * `Genre` (Exploded for one-genre-per-row analysis)

---

## 🧹 Data Cleaning & Preprocessing

Robust data preparation was essential for accurate analysis:

* **Date Transformation:** Converted `Release_Date` to datetime and extracted the **release year**.
* **Irrelevant Columns Dropped:** Removed `Overview`, `Poster_URL`, and `Original_Language`.
* **Genre Explosion:** Split multi-genre strings and **exploded** the dataframe to ensure each movie-genre pair was a unique row, facilitating genre-level aggregation.
* **Ordinal Transformation:** Transformed the continuous `Vote_Average` into four ordinal categories using quartile-based bins: **`['Not popular', 'Below Average', 'Average', 'Popular']`**.
* **Handling Missing Values:** Ensured data integrity by handling missing values and enforcing correct numeric data types.

---

## 📈 Exploratory Data Analysis (EDA)

Key visual insights revealed through `matplotlib` and `seaborn`:

* **🎭 Genre Distribution:** A bar chart highlighted the most frequent genres dominating the catalog.
* **⭐ Vote Average Categories:** Visualizing the distribution of movies across the new popularity levels.
* **📆 Yearly Trend:** A histogram showed the surge in movie releases, identifying peak years.
* **🔥 Popularity Extremes:** Direct identification of the movies with the absolute highest and lowest popularity scores.
* **⚠️ Outlier Detection:** Noted visible outliers in the `Popularity` distribution, recommending future use of robust statistical methods.

---

## 💡 Key Findings

The analysis successfully answered the project's key business questions, providing a data-backed view of Netflix's content strategy:

* **Most Frequent Genres:** **Drama**, **Comedy**, and **Action** overwhelmingly dominate Netflix releases, forming the core of the catalog.
* **Highest-Voted Genres:** Genres with the highest aggregated votes tend to be **Drama** and **Documentary** films, suggesting higher engagement or critical mass for these types of content.
* **Popularity Skew:** Movie popularity is heavily skewed towards a few major titles, exhibiting a **clear long-tail distribution**.
* **Peak Release Years:** The years **2017–2019** saw the maximum surge and peak in Netflix content acquisition or release volume.

---

## 🛠️ Tools & Libraries

| Category | Tool / Library | Purpose |
| :--- | :--- | :--- |
| **Programming** | **Python 3** | Core language for the project. |
| **Data Handling** | **`pandas`**, **`numpy`** | Data manipulation, cleaning, and numerical operations. |
| **Visualization** | **`seaborn`**, **`matplotlib`** | Creating informative and aesthetic charts for EDA. |
| **Environment** | **JupyterLab** / **Notebook** | Interactive development and documentation. |
| **Version Control** | **Git**, **GitHub** | Code collaboration and project hosting. |

---


