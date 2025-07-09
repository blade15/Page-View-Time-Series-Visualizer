# 📊 freeCodeCamp Forum Page Views Time Series Visualizer

This project is part of the freeCodeCamp Data Analysis with Python certification. The goal is to visualize time series data representing the number of daily page views on the freeCodeCamp forum from May 2016 to December 2019. The project involves data cleaning and visualizing the dataset using line plots, bar plots, and box plots.

## 📁 Dataset
The dataset used in this project is: `fcc-forum-pageviews.csv`. It contains two columns:
- `date`: the date of the forum activity.
- `value`: the number of page views on that date.

---

## 🧹 Data Cleaning
To ensure more accurate visualizations, the data was cleaned by removing the top 2.5% and bottom 2.5% of page view counts (outliers), based on quantiles.

---

## 📈 Visualizations

### 1. Line Plot
- **Function:** `draw_line_plot()`
- **Purpose:** Visualizes the daily page views over time.
- **Details:**
  - X-axis: Date
  - Y-axis: Page Views
  - Title: *"Daily freeCodeCamp Forum Page Views 5/2016-12/2019"*

### 2. Bar Plot
- **Function:** `draw_bar_plot()`
- **Purpose:** Displays the average daily page views per month grouped by year.
- **Details:**
  - X-axis: Years
  - Y-axis: Average Page Views
  - Legend: Months (January to December)
  - Data is grouped using `groupby(['year', 'month'])` and reshaped with `.unstack()`.

### 3. Box Plots
- **Function:** `draw_box_plot()`
- **Purpose:** Shows distributions and seasonality of page views.
- **Details:**
  - **Left Plot (Year-wise Trend):**
    - X-axis: Year
    - Y-axis: Page Views
    - Title: *"Year-wise Box Plot (Trend)"*
  - **Right Plot (Month-wise Seasonality):**
    - X-axis: Month (Jan to Dec)
    - Y-axis: Page Views
    - Title: *"Month-wise Box Plot (Seasonality)"*

---

## 🛠️ Technologies Used
- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## ✅ How to Run
1. Clone this repository.
2. Make sure the dataset `fcc-forum-pageviews.csv` is in the working directory.
3. Run the notebook `fcc_pageviews_analysis.ipynb`.
4. The visualizations will be generated and displayed within the notebook.

---

## 📌 Project Status
✅ Completed – All required visualizations are implemented and meet the project specifications.

---

## 📚 License
This project is part of the [freeCodeCamp Data Analysis with Python](https://www.freecodecamp.org/learn/data-analysis-with-python/) curriculum and is intended for educational purposes.
