
# 🎮 Video Game Sales Analysis with Python

This project analyzes a video game sales dataset to uncover trends and insights based on regional, national, and global sales performance. The analysis is done using **Pandas**, **NumPy**, **Seaborn**, and **Matplotlib**.

## Dataset

The dataset used:  
`VideoGamesSales.csv`  
It includes the following columns:
- `Region`
- `Country`
- `Year`
- `Genre`
- `NA_Sales`
- `Global_Sales`
- `NA_Profit`
- `Global_Profit`

## 🛠️ Data Cleaning & Preparation

- Removed duplicate rows.
- Filled missing `Region` values with `"North"`.
- Converted `NA_Sales` to numeric, removing dollar signs.
- Replaced missing sales values with the **average national sales**.
- Standardized country names (e.g., `"USA"` → `"United States"`).
- Formatted country names to **title case**.
- Renamed columns for clarity:
  - `NA_Sales` → `National Sales`
  - `Global_Sales` → `Global Sales`
  - `NA_Profit` → `National Profit`
  - `Global_Profit` → `Global Profit`
- Capped extreme outliers in `National Sales` using the 95th percentile.

## 📊 Visualizations

### 1. National Sales by Region and Country

A bar plot showing national sales totals grouped by region and country.

![Barplot](#)

---

### 2. National Sales Distribution by Country and Genre

A boxplot highlighting the distribution of national sales across countries, split by genre, including mean markers.

![Boxplot](#)

---

### 3. Pie Charts: Sales Distribution

- **National Sales by Country**
- **Global Sales by Country**

Two side-by-side pie charts representing each country’s share of total sales.

---

### 4. Line Chart: Sales Over Time

A line plot showing how both national and global sales evolved over the years.

---

## 📦 Libraries Used

- `pandas`
- `numpy`
- `seaborn`
- `matplotlib.pyplot`

Make sure to install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn
