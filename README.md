# Healthcare Data Cleaner 🧹

A Python data-cleaning project that prepares healthcare patient records for analysis and future machine-learning workflows. The notebook investigates missing values and outliers using multiple techniques, compares their effects, and exports a final cleaned dataset.

> **Project type:** Data Analytics / Data Preprocessing  
> **Main tools:** Python, Pandas, NumPy, Scikit-learn, SciPy, Jupyter Notebook

## 📌 Project at a Glance

Healthcare datasets can contain incomplete records and unusual measurements. If these issues are not handled carefully, summaries and machine-learning models may be less reliable. This project demonstrates a repeatable workflow to inspect data quality, test cleaning strategies, and create a cleaned CSV file.

### What this project does

- Inspects dataset structure, column types, and missing values.
- Builds a missing-value report with counts and percentages.
- Compares median, random-sample, KNN, and iterative (MICE-style) imputation.
- Tests Z-score and IQR outlier filtering, percentile clipping, and Winsorization.
- Compares dataset shapes and descriptive statistics before and after outlier treatment.
- Saves the final processed data to `final_cleaned_dataset.csv`.

## 📁 Project Files

```text
Data-Cleaner-Project/
├── Data Cleaner Project.ipynb       # Main notebook and implementation
├── healthcare_patient_dataset.csv   # Input dataset (add this file)
├── final_cleaned_dataset.csv        # Generated after running the notebook
└── README.md                        # Project documentation
```

The input CSV is not embedded in the notebook. Keep `healthcare_patient_dataset.csv` in the same working folder as the notebook, or update the path in the `pd.read_csv()` cell.

## 🧰 Tech Stack

| Tool / Library | How it is used |
|---|---|
| Python | Main programming language |
| Pandas | Loading, inspecting, cleaning, and exporting tabular data |
| NumPy | Numerical operations and random-sample imputation |
| Scikit-learn | `SimpleImputer`, `KNNImputer`, and `IterativeImputer` |
| SciPy | Z-score calculations and Winsorization |
| Jupyter Notebook | Running the workflow cell by cell |

## 🚀 Getting Started

### 1. Install Python libraries

Run this in a terminal or notebook cell:

```bash
pip install pandas numpy scikit-learn scipy jupyter
```

### 2. Add the input dataset

Place `healthcare_patient_dataset.csv` next to `Data Cleaner Project.ipynb`. The notebook expects healthcare fields such as `age`, `gender`, `region`, `bmi`, `blood_pressure`, `cholesterol`, and `glucose`.

### 3. Start Jupyter

```bash
jupyter notebook
```

Open `Data Cleaner Project.ipynb` and run the cells in order. If you are using Google Colab, upload the CSV first or mount the drive and update the file path.

### 4. Check the output

At the end of the notebook, the cleaned DataFrame is exported as:

```text
final_cleaned_dataset.csv
```



## 🎯 Learning Outcomes

By completing this project, you practise:

- Auditing missing data with Pandas.
- Comparing common imputation approaches.
- Detecting and treating statistical outliers.
- Evaluating data changes with descriptive statistics.
- Exporting a reproducible cleaned CSV for downstream analysis.

## 👤 Project

**Repository title suggestion:** `Healthcare Data Cleaning with Python`  
**Notebook:** `Data Cleaner Project.ipynb`
# Author : Kripal Prajapati

---

If you use or extend this project, document the dataset source, explain why each cleaning method was selected, and record any changes made to the workflow.
