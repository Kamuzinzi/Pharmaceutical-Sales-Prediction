# Pharmaceutical Sales Prediction

A machine learning project to forecast Rossmann store sales using store, promotion, and competitor data.

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Business Context](#business-context)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Technologies Used](#technologies-used)
- [License](#license)

## 🎯 Project Overview

This project builds an end-to-end machine learning solution to forecast sales across Rossmann pharmaceutical stores six weeks ahead of time. The solution leverages factors such as promotions, competition, school and state holidays, seasonality, and locality to deliver accurate predictions for the finance team.

## 💼 Business Context

**Role:** Machine Learning Engineer at Rossmann Pharmaceuticals

**Problem:** The finance team needs to forecast sales across all stores. Store managers currently rely on experience and judgment, which is inconsistent and time-consuming.

**Solution:** Build and serve a data-driven prediction product that delivers reliable forecasts to analysts in the finance team.

## 📊 Dataset

The dataset is from the [Rossmann Store Sales Kaggle competition](https://www.kaggle.com/competitions/rossmann-store-sales/data).

**Data Sources:**
- [Kaggle](https://www.kaggle.com/competitions/rossmann-store-sales/data)
- [Google Drive](https://drive.google.com/file/d/1sGLyrytv6xYBrCPdjZkE1ZDSwngDij4W/view?usp=sharing)

**Key Data Fields:**

| Field | Description |
|-------|-------------|
| Id | (Store, Date) identifier in the test set |
| Store | Unique ID for each store |
| Sales | Daily turnover (target variable) |
| Customers | Number of customers per day |
| Open | Store open indicator (0 = closed, 1 = open) |
| StateHoliday | a = public holiday, b = Easter, c = Christmas, 0 = None |
| SchoolHoliday | Whether public schools were closed |
| StoreType | Store model (a, b, c, d) |
| Assortment | a = basic, b = extra, c = extended |
| CompetitionDistance | Distance in meters to nearest competitor |

## 📁 Project Structure

```
Pharmaceutical-Sales-Prediction/
│
├── data/
│   ├── raw/                    # Raw data (DVC-tracked)
│   │   ├── train.csv
│   │   ├── test.csv
│   │   └── store.csv
│   └── processed/               # Processed datasets
│
├── notebooks/
│   ├── exploratory/            # EDA, preprocessing, modeling trials
│   │   └── exploratory_data_analysis.ipynb
│   └── final/                   # Polished report-style notebook
│
├── src/                         # Python modules for deployment
│
├── environment.yml              # Conda environment
├── requirements.txt             # Python dependencies
├── setup.py                     # Package setup
└── README.md
```

## 🚀 Installation

### Option 1: Conda (Recommended)

```bash
conda env create -f environment.yml
conda activate initial-env
pip install -e .
```

### Option 2: pip

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
pip install -e .
```

### Data Setup (DVC)

If using DVC for data versioning:

```bash
dvc pull
```

Otherwise, download the data from [Kaggle](https://www.kaggle.com/competitions/rossmann-store-sales/data) and place the CSV files in `data/raw/`.

## 💻 Usage

1. **Exploratory Analysis:** Run notebooks in `notebooks/exploratory/` for EDA and modeling trials
2. **Final Results:** See `notebooks/final/` for the polished report
3. **Deployment:** Use modules in `src/` for model deployment

## 🛠️ Technologies Used

- **Python 3.8+**
- **Data & ML:** pandas, numpy, scipy, PySpark
- **Experiment Tracking:** DVC, MLflow
- **Deployment:** Flask, Docker
- **Notebooks:** Jupyter

## 📝 License

See [LICENSE](LICENSE) for details.

---

⭐ If you find this project helpful, please consider giving it a star!
