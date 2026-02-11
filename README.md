# 🏏 Cricket Test Match Data Cleaning 

## 📌 Project Overview
This project focuses on performing extensive **Data Cleaning** and **Feature Engineering** on a dataset containing historical records of cricket players' performances. The raw data, sourced from ESPN Cricinfo, contained several inconsistencies, special characters, and incorrect data types that required systematic cleaning before any analysis could be conducted.

---

## 🖼️ Data Transformation (Before & After)

### Raw Data (Before Cleaning)

<img width="80%" height="80%" alt="Raw Data" src="https://github.com/user-attachments/assets/24eac46d-93fd-471f-9a94-c246d2184499" />

---

### Cleaned Data (After Processing)

<img width="80%" height="80%" alt="Clean Data 1" src="https://github.com/user-attachments/assets/5d41d59a-1e03-4335-bc71-5010b9cc918b" />

<img width="80%" height="80%" alt="Clean Data 2" src="https://github.com/user-attachments/assets/0fce204a-a587-41b6-b9a9-7c73461c97f1" />

---


## 🛠️ Data Cleaning Steps
In this project, I handled various data quality issues using **Python** and **Pandas**:

1.  **Column Renaming:** Renamed abbreviated column headers (e.g., `HS`, `BF`, `SR`) into descriptive names for better readability.
2.  **Handling Special Characters:** * Removed `*` from the `Highest_Inns_Score` to indicate "not out" cases and converted them to integers.
    * Cleaned the `+` sign from columns like `Balls_Faced` and `Boundary_Fours` to enable mathematical calculations.
3.  **Splitting & Extracting Data:** * Split the `Playing_Span` column (e.g., "1990-2010") into separate `Start_Year` and `End_Year` columns.
4.  **Data Type Conversion:** Converted object/string columns into proper numerical formats (`int`, `float`) for statistical analysis.
5.  **Handling Missing Values:** Identified and imputed null values in key metrics like `Balls_Faced` and `Batting_Strike_Rate` with appropriate defaults.
6.  **Feature Engineering:** Calculated the **Career_Length** for each player based on their active years.

---

## 📊 Key Findings (Post-Cleaning)
* **Average Career Length:** Calculated the average duration of a professional cricket career from the dataset.
* **Performance Metrics:** Analyzed the `Batting_Strike_Rate` for veteran players (those with over 10 years of experience).
* **Historical Analysis:** Counted the number of players who started their careers before 1960.

---

## 🛠️ Tech Stack
* **Data Source:** <a href= "https://www.espncricinfo.com/records/highest-career-batting-average-282910">ESPN Cricinfo</a>.
* **Language:** Python.
* **Library:** Pandas.
* **Environment:**  Google Colab.


