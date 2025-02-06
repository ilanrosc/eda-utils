# eda-utils

**eda-utils** is a Python package designed for reusable Exploratory Data Analysis (EDA) functions. It provides utility functions for data loading, statistical summaries, data visualization, data cleaning, and outlier detection, making it easier to perform preliminary data analysis.

## 📌 Features
- **Data Loading**: Read CSV, Excel, JSON, and other file formats.
- **Statistical Summaries**: Generate descriptive statistics and correlation matrices.
- **Data Visualization**: Create histograms, boxplots, and correlation heatmaps.
- **Data Cleaning**: Handle missing values, remove duplicates, and standardize column names.
- **Outlier Detection**: Identify and handle outliers using various statistical methods.

## 🚀 Installation
You can install `eda-utils` directly from GitHub:
```sh
pip install git+https://github.com/ilanrosc/eda-utils.git
```

## 🛠️ Usage
```python
import eda_utils as eda
import pandas as pd

# Load dataset
df = eda.data_loader(path="your_path", filename="your_filename.csv", type="csv")

# Generate summary statistics
summary = eda.stats_summary.generate_summary(df)

# Visualize missing values
eda.data_visualization.plot_missing_values(df)

# Clean missing values
df_cleaned = eda.data_cleaning.clean_missing_values(df, method="mean")

# Detect outliers
outliers = eda.outlier_detection.detect_outliers_iqr(df, column="age")
```

## 📂 Project Structure
```
eda-utils/
│── eda_utils/                # Main package directory
│   ├── __init__.py           # Package initialization
│   ├── data_loader.py        # Load data from CSV, Excel, JSON, etc.
│   ├── stats_summary.py      # Compute descriptive statistics
│   ├── data_visualization.py # Generate plots and visualizations
│   ├── data_cleaning.py      # Handle missing values, duplicates, and inconsistencies
│   ├── outlier_detection.py  # Identify and handle outliers
│── tests/                    # Unit tests for package functions
│── docs/                     # Documentation
│── notebooks/                # Usage examples in Jupyter notebooks
│── requirements.txt          # Package dependencies
│── setup.py                  # Installation script
│── README.md                 # Project overview
│── .gitignore                # Ignore unnecessary files
```

## 📌 Dependencies
The package requires the following dependencies:
```sh
pandas
numpy
matplotlib
seaborn
scipy
scikit-learn
```
Dependencies are installed automatically when using `pip`. However, you can also install them manually if needed using:
```sh
pip install -r requirements.txt
```

## 📄 Documentation
Detailed documentation for each function, including usage examples, can be found in the `docs/` folder.

## 📄 License
This project is licensed under the MIT License.

## 👤 Author
Developed by **Ilana Molcanova**  
🔗 GitHub: [ilanrosc](https://github.com/ilanrosc)
Email: ilana.roscina@gmail.com

---
🚀 **Easily integrate powerful EDA functions into your data projects!**

