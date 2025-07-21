
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

(<img width="1549" height="779" alt="Screenshot (314)" src="https://github.com/user-attachments/assets/b1dccb06-acae-42c1-ac41-e12ca20911cb" />
)

---

### 2. National Sales Distribution by Country and Genre

A boxplot highlighting the distribution of national sales across countries, split by genre, including mean markers.

<img width="1222" height="797" alt="Screenshot (315)" src="https://github.com/user-attachments/assets/2968c2f1-4114-406f-b4a3-1b4febfa697b" />
)

---

### 3. Pie Charts: Sales Distribution

- **National Sales by Country**
- **Global Sales by Country**

Two side-by-side pie charts representing each country’s share of total sales.

---

### 4. Line Chart: Sales Over Time

A line plot showing how both national and global sales evolved over the years.

<img width="1273" height="804" alt="Line" src="https://github.com/user-attachments/assets/a98b35a5-57b5-49f8-a578-59631f8e9239" />



---

## 📦 Libraries Used

- `pandas`
- `numpy`
- `seaborn`
- `matplotlib.pyplot`

Make sure to install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn
