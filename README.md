
# 🌳 Global Deforestation and Forest Cover Change Analysis (2000-2020)

## Project Overview

This repository contains a Jupyter Notebook dedicated to analyzing and visualizing global forest cover change between the years **2000 and 2020**.

The project focuses on identifying the countries that experienced the most significant absolute forest cover **loss** and **gain**, using key metrics to understand the global dynamics of deforestation and reforestation efforts.

---

## 📊 Dataset and Key Metrics

The analysis utilizes a publicly available dataset, typically sourced from platforms like Kaggle, focusing on forest change metrics by country.

* **Key Data Points:**
    * `forests_2000`: Forest cover percentage in the year 2000.
    * `forests_2020`: Forest cover percentage in the year 2020.
    * `trend`: A metric indicating the change trajectory over the period.

* **Calculated Metric:**
    * **`forest_change`**: The absolute difference (`forests_2020` - `forests_2000`), representing the net change in forest cover percentage over the two decades.

---

## ✨ Analysis Pipeline and Visualizations

The notebook `Deforestation__Analysis.ipynb` performs the following steps:

### 1. Data Preparation and Cleaning
* **Missing Value Imputation:** Handled 10 missing values in the `trend` column by imputing them with the calculated **mean** of the existing trend values.
* **Metric Calculation:** Created the critical `forest_change` column to quantify the extent of loss or gain.
* **Targeted Subset Selection:** The analysis was narrowed down to the **top 10 countries** with the largest forest gain and the **bottom 10 countries** with the largest forest loss for focused visualization.

### 2. Key Visualizations
Two primary visualizations were generated using `matplotlib` and/or `seaborn`:

* **Bar Plot (Forest Change):** Clearly illustrates the magnitude of forest cover change, highlighting countries with large positive bars (gain) and large negative bars (loss).
* **Heatmap (Comparative Metrics):** Provides a rich visual comparison of all metrics (`forests_2000`, `forests_2020`, `trend`, and `forest_change`) across the top and bottom countries, revealing patterns in the data.

### 3. Insights and Future Work
The analysis provides a clear snapshot of global forest health. Future work includes investigating the **socioeconomic and policy factors** that contribute to these dramatic changes in the identified countries.

---

## 💻 Dependencies

To execute the notebook and reproduce the analysis, you need a Python environment with these libraries installed:

```bash
pandas
numpy
matplotlib
seaborn
````

You can install them using `pip`:

```bash
pip install pandas numpy matplotlib seaborn
```

-----

## 🚀 How to Run the Notebook

1.  **Clone the repository:**
    ```bash
    git clone [your-repository-url]
    cd [your-repository-name]
    ```
2.  **Ensure Data is Present:** Make sure the underlying deforestation dataset (e.g., a file named `forest_change.csv` or similar) is in the project directory, or update the file loading path in the notebook.
3.  **Launch Jupyter:**
    ```bash
    jupyter notebook Deforestation__Analysis.ipynb
    ```
4.  **Execute Cells:** Run all cells sequentially to perform the data cleaning, analysis, and generate the comparative visualizations.

<!-- end list -->

```
```
