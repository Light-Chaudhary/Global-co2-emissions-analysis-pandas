# Global CO₂ Emissions Analysis (2020)

This project analyzes global CO₂ emissions data from the [Our World in Data](https://github.com/owid/co2-data) dataset. We focus on filtering and interpreting emissions data for the year **2020**, including CO₂ per capita, population, and identifying top contributors.

## 📁 Dataset

- Source: [owid/co2-data.csv](https://github.com/owid/co2-data)
- Columns used:  
  - `country`  
  - `year`  
  - `co2`  
  - `co2_per_capita`  
  - `population`  

## 📊 Tasks Performed

1. **Load and clean the dataset**
   - Selected relevant columns.
   - Filtered data for the year 2020 only.
   - Removed rows with missing `co2_per_capita`.

2. **Top 10 countries by CO₂ per capita**
   - Sorted and displayed countries with the highest emissions per person.

3. **Global average CO₂ per capita**
   - Calculated the mean CO₂ per capita for all countries in 2020.

4. **Countries above the global average**
   - Filtered countries whose `co2_per_capita` exceeded the global average.

5. **Large countries with high emissions**
   - Used `.query()` to find countries with:
     - `population > 100,000,000`  
     - `co2 > 500` million metric tons

## 🛠️ Tools Used

- Python
- Pandas
- Jupyter Notebook / Anaconda

## 📌 Key Learnings

- Filtering rows using conditions
- Handling missing data with `.dropna()`
- Sorting with `.nlargest()`
- Column selection and renaming
- Using `.query()` for clean condition-based filtering

---

> This is a beginner-friendly analysis to practice real-world data handling with `pandas`. Future improvements may include visualizations and time-based trends.
