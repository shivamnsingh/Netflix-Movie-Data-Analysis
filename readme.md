![Netflix Movie Data Analysis](https://raw.githubusercontent.com/shivamnsingh/netflix-movie-analysis/main/figures/netflix_banner.png)

# 🎬 Netflix Movie Data Analysis Project  

A complete **data science & analytics project** exploring insights from over **25,000 Netflix movie records**.  
This project showcases **data cleaning, preprocessing, exploratory analysis, and visualization** using Python — revealing how genres, popularity, and release trends shape Netflix’s movie catalog.

---

## 🧠 Project Overview  

Netflix is known for its use of **data science, AI, and machine learning** to build recommendation systems that understand user preferences.  
In this project, I analyzed a dataset of **~25,552 movies** to answer key business questions such as:

1. What is the most frequent genre of movies released on Netflix?  
2. Which genres have the highest votes?  
3. What movie has the **highest popularity**, and what is its genre?  
4. What movie has the **lowest popularity**, and what is its genre?  
5. Which **year** had the most films released?

---

## 📊 Dataset Details  

- **Source:** `mymoviedb.csv`  
- **Total Rows:** 25,552  
- **Final Columns:**  
  - `Release_Date` (Year extracted from date)  
  - `Title`  
  - `Popularity`  
  - `Vote_Count`  
  - `Vote_Average` *(Categorized into 4 bins)*  
  - `Genre` *(Exploded for multi-genre movies)*  

---

## 🧹 Data Cleaning & Preprocessing  

✔ Converted `Release_Date` → datetime → extracted **year**  
✔ Dropped irrelevant columns (`Overview`, `Poster_URL`, `Original_Language`)  
✔ Split multi-genre strings and **exploded** dataframe → one genre per row  
✔ Transformed `Vote_Average` → **ordinal bins** using quartiles:  
   `['Not popular', 'Below Average', 'Average', 'Popular']`  
✔ Handled missing values, duplicates, and ensured numeric data types  

---

## 📈 Exploratory Data Analysis  

Key visual insights:  

- 🎭 **Genre Distribution:** Bar chart showing the most frequent genres  
- ⭐ **Vote Average Categories:** Distribution of movies by popularity levels  
- 📆 **Yearly Trend:** Histogram of movie releases over time  
- 🔥 **Popularity Extremes:** Identified movies with highest & lowest popularity  
- ⚠️ **Outlier Detection:** Popularity had visible outliers — recommended robust stats  

---

## 💡 Key Findings  

- **Most frequent genres:** Drama, Comedy, and Action dominate Netflix releases.  
- **Highest-voted genres:** Tend to be Drama and Documentary films.  
- **Popularity:** Skewed toward a few major titles — clear long-tail trend.  
- **Most filmed years:** 2017–2019 saw the maximum surge in Netflix content.  

---

## 🛠️ Tools & Libraries  

| Category | Tools Used |
|-----------|-------------|
| Programming | Python |
| Data Handling | pandas, numpy |
| Visualization | seaborn, matplotlib |
| Notebook | JupyterLab |
| Version Control | Git, GitHub |

---

## 📂 Project Structure  


