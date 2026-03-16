# 📊 Commodity Price Analysis in Indonesia

This project analyzes **commodity price data in Indonesia** using Python to identify price trends, highest and lowest annual changes, and monthly average patterns.

The analysis focuses on **data cleaning, exploratory data analysis (EDA), and visualization** to understand fluctuations in commodity prices across different time periods.

This project demonstrates a typical **Data Analyst workflow**, including data preprocessing, statistical exploration, and visualization of economic data.

---

# 📌 Objectives

The objectives of this project are:

* Clean raw commodity price data
* Transform the dataset into an analyzable format
* Identify commodities with the **highest and lowest annual price changes**
* Analyze **average commodity prices across months**
* Visualize **top commodities with significant price changes**
* Understand **price fluctuations in food commodities**

---

# 🛠 Tools & Libraries

The project uses the following tools:

* Python
* Pandas
* Matplotlib
* Seaborn
* Jupyter Notebook

---

# 📂 Project Workflow

### 1 Data Collection

The dataset contains **commodity price information across multiple months** and is sourced from statistical publications.

---

### 2 Data Cleaning

Data cleaning steps include:

* Fixing incorrect headers
* Renaming columns (e.g., `Unnamed` → `Komoditas`)
* Handling missing values
* Preparing numeric columns for analysis

Example:

```python
data.rename(columns={'Unnamed: 0':'Komoditas'}, inplace=True)
```

---

### 3 Exploratory Data Analysis

Several analyses were performed to understand commodity price behavior:

* Identifying **highest annual price increases**
* Identifying **lowest annual price changes**
* Calculating **average prices across months**

Example:

```python
data.sort_values(by='Tahunan', ascending=False)
```

---

### 4 Data Visualization

Data visualization is used to better understand commodity price trends.

Examples include:

* **Top 10 commodities with the highest annual price increase**
* **Price trend analysis for specific commodity groups**

Example filtering:

```python
komoditas = data[data["Komoditas"] == "Daging Dan Hasil-Hasilnya"]
```

These visualizations help highlight **price volatility and seasonal patterns in commodity markets**.

---

# 📈 Example Visualization

![Commodity Price Visualization](images/visualization.png)

The visualization helps identify:

* Commodities with the **largest annual price increases**
* Commodities with **stable price patterns**
* Possible **seasonal fluctuations in food commodity prices**

---

# 💡 Key Skills Demonstrated

* Data Cleaning
* Data Transformation
* Exploratory Data Analysis (EDA)
* Data Visualization
* Python for Data Analysis
* Economic Data Interpretation

---

# 📁 Project Structure

```
commodity-price-analysis
│
├── data
│   └── data_harga.csv
│
├── notebook
│   └── Analist.ipynb
│
├── images
│   └── visualization.png
│
└── README.md
```

---

# 👨‍💻 Author

This project was created as part of a **Data Analyst portfolio** to demonstrate the ability to process, analyze, and visualize economic datasets using Python.
