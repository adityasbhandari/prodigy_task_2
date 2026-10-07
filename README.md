# Titanic Data Cleaning & EDA 🚢

Exploratory data analysis on the Titanic passenger dataset, built as Task 2 of my Prodigy InfoTech internship. The goal: clean the data, then find out which factors affected survival.

## 🛠️ Technologies
- **Python**
- **Pandas** and **NumPy** for data handling
- **Matplotlib** and **Seaborn** for charts
- **SciPy** for z-score outlier detection
- **Google Colab / Jupyter Notebook**

## ✨ Features
- A reusable `DataUnderstanding` class for summary stats, missing values, data types, and value counts
- Data cleaning: dropped `Cabin`, filled missing `Embarked` values, removed rows with missing `Age`
- Duplicate check on `PassengerId`
- Boxplots of numerical columns before and after outlier removal
- Visuals: survival pie chart, age histogram, passenger class count plot, pair plot, violin plot, and an Age vs Fare correlation heatmap
- Dark theme with a blue colour palette

## 🔄 The Process
1. Loaded `train.csv` and inspected its structure
2. Checked missing values and data types
3. Cleaned the data (dropped, filled, and removed as needed)
4. Detected and removed outliers using z-scores (threshold = 3)
5. Visualised distributions and relationships between variables
6. Looked for patterns in survival by age, class, and fare

## 📚 What I Learned
- **Data Cleaning:** Deciding when to drop a column, fill a value, or remove rows depending on how much data is missing.
- **Outliers:** Using z-scores to spot extreme values and comparing boxplots before and after removal.
- **Clean Code:** Wrapping repeated steps in a class and functions made the analysis easier to reuse.
- **Seaborn:** Building violin plots, pair plots, and heatmaps to compare several variables at once.
- **Choosing Charts:** Pie charts for proportions, histograms for distributions, heatmaps for correlation.
- **Storytelling:** Turning raw numbers into visuals that explain who survived and why.

## 📁 Files
- `train.csv`: the dataset
- `prodigy_2.py`: the analysis script

## ▶️ How to Run
```bash
pip install pandas numpy matplotlib seaborn scipy
python prodigy_2.py
```
