# 🏎️ Formula One Lap Time Analysis (2019–2021)

## 📌 Project Overview
This project is an end-to-end exploration of Formula One race data.  
The dataset was obtained from the **FastF1 API** and enriched with additional information to make it more complete and useful for analysis.

The focus is on **lap times, race results, and conditions** — uncovering insights beyond simple finishing positions.  
The analysis was extended into Tableau for interactive visual exploration.

---

## 🗂️ Data Sources
- **FastF1 API** – Primary source of lap time and race data.  
- **Custom Python Scripts** – Used to collect and clean the data, and to add missing races.  
- **SQL + Python** – Applied for data enrichment and transformation.  

---

## 🛠️ Data Preparation
1. **Base Data**  
   - Extracted lap times and race details using the FastF1 API.  

2. **Missing Races**  
   - The 2021 season had **15 races missing** in the raw FastF1 dataset.  
   - These were added back using Python data processing.  

3. **Additional Columns Added**  
   - `Starting_Position` → via SQL/Python joins  
   - `Finishing_Position` → via SQL/Python updates  
   - `Weather` → integrated weather conditions per race  
   - `Winner` → annotated race winners for each GP  

4. **Cleaning & Validation**  
   - Standardized race names (e.g., *Mexico City GP* vs *Mexican GP*).  
   - Converted lap/sector times to consistent formats.  
   - Ensured null values handled properly (e.g., DNFs in finishing positions).  

---

## 📊 Analysis in Tableau
A Tableau workbook is included with **basic race insights**, such as:
- Lap time comparisons across drivers.  
- Tyre strategies (stints and compound usage).  
- Starting vs. finishing position analysis.  
- Impact of weather on race performance.  

---

## 📁 Repository Contents
- `data/` → Processed datasets (CSV/SQL).  
- `notebooks/` → Python scripts for cleaning and enrichment.  
- `tableau/` → Tableau workbook with exploratory visualizations.  

---

## 🚀 Next Steps
- going deep in the analysis
- Explore correlations between weather, tyre choices, and lap time consistency.  

---

## 🙌 Acknowledgments
- **FastF1 API** developers and community.  
- Formula One official resources.  
