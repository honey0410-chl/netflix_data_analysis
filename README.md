# Netflix Dataset Exploratory Data Analysis (EDA)

## Project Overview
This project performs **Exploratory Data Analysis (EDA)** on a Netflix movies dataset using **Python, Pandas, Matplotlib, and Seaborn**.

The notebook focuses on:
- loading and inspecting the dataset
- cleaning and preprocessing data
- handling duplicates and missing values
- transforming date and genre columns
- categorizing vote averages
- visualizing genre, ratings, and release year distributions

---

## Dataset
The notebook uses a CSV dataset named:

`netflix_Dataset.csv`

> Note: Update the dataset path before running the notebook if needed.

---

## Tools & Libraries Used
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Jupyter Notebook**

---

## Workflow
### 1. Data Loading
The dataset is loaded using Pandas:

```python
df = pd.read_csv("netflix_Dataset.csv")
```

### 2. Data Inspection
Initial exploration includes:
- `head()`
- `info()`
- `describe()`
- duplicate checks

### 3. Data Cleaning
Steps performed:
- converted `Release_Date` to datetime
- extracted year from release date
- removed unnecessary columns:
  - `Overview`
  - `Original_Language`
  - `Poster_Url`
- removed missing values

### 4. Feature Engineering
- `Vote_Average` values are grouped into categories:
  - `not_popular`
  - `below_average`
  - `average`
  - `popular`

- `Genre` column is split and expanded for genre-level analysis

### 5. Data Visualization
Visualizations include:
- genre frequency distribution
- vote average category counts
- release year histogram

---

## Key Insights
The notebook helps identify:
- most common genres
- popularity distribution
- release trends over years
- highest and lowest popularity titles

---

## How to Run
1. Install dependencies:
```bash
pip install pandas numpy matplotlib seaborn notebook
```

2. Open Jupyter Notebook:
```bash
jupyter notebook
```

3. Run the notebook cells sequentially.

---

## File Structure
- `*.ipynb` → main analysis notebook
- `README.md` → project documentation

---

## Author
Aryan Chadokar
