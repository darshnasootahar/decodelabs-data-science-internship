# Week 1 – Data Science Tasks
## DecodeLabs Internship | By: Darsha Sootahar

---

## 📦 Dataset Used
**Titanic Dataset**
- Source: Built-in Seaborn library (`sns.load_dataset('titanic')`)
- Size: 891 rows × 15 columns
- Description: Contains information about passengers aboard the Titanic ship (1912), including age, gender, class, fare, and whether they survived.

---

## ✅ Tasks Completed

### Task 1: Data Collection & Dataset Understanding
- **Goal:** Load the Titanic dataset and explore its structure
- **File:** `task1_data_collection.py`
- **What I did:**
  - Loaded the dataset using Seaborn
  - Identified all 15 columns and their data types
  - Checked dataset size (891 rows, 15 columns)
  - Identified missing values in age, deck, embark_town
  - Described what each column represents

---

### Task 2: Data Cleaning & Preprocessing
- **Goal:** Clean and prepare data for analysis
- **File:** `task2_data_cleaning.py`
- **What I did:**
  - Filled missing `age` values with median (29.0)
  - Filled missing `embarked` values with mode ('S')
  - Dropped `deck` column (77% missing values)
  - Removed duplicate rows (0 found)
  - Encoded `sex` column: male=0, female=1
  - Encoded `embarked` column: S=0, C=1, Q=2
  - Saved cleaned dataset as `cleaned_titanic.csv`

---

### Task 3: Exploratory Data Analysis (EDA)
- **Goal:** Discover patterns and trends in the data
- **File:** `task3_eda.py`
- **What I did:**
  - Calculated basic statistics (mean, median, min, max)
  - Analyzed survival rates by gender and class
  - Detected outliers in fare column using IQR method
  - Summarized key findings

- **Key Findings:**
  | Finding | Value |
  |---------|-------|
  | Overall Survival Rate | 38.38% |
  | Female Survival Rate | ~74% |
  | Male Survival Rate | ~18% |
  | 1st Class Survival | ~63% |
  | 3rd Class Survival | ~24% |
  | Average Age | 29 years |

---

### Task 4: Data Visualization
- **Goal:** Create charts to communicate insights visually
- **File:** `task4_visualization.py`
- **Output:** `titanic_visualizations.png`
- **Charts Created:**
  1. Survival Count (Bar Chart)
  2. Survival Rate by Gender (Bar Chart)
  3. Survival Rate by Passenger Class (Bar Chart)
  4. Age Distribution (Histogram)
  5. Fare Distribution (Histogram)
  6. Embarkation Port (Pie Chart)

---

### Task 5: Predictive Model
- **Goal:** Build a model to predict passenger survival
- **File:** `task5_predictive_model.py`
- **Model Used:** Logistic Regression
- **What I did:**
  - Selected 5 features: pclass, sex, age, fare, embarked
  - Split data: 80% training, 20% testing
  - Trained Logistic Regression model
  - Evaluated model performance
  - Predicted survival for a new passenger

- **Model Results:**
  | Metric | Score |
  |--------|-------|
  | Accuracy | ~80% |
  | Best Predictor | Gender (sex) |
  | 2nd Best | Passenger Class |

---

## 🛠️ Tools & Libraries Used
- Python 3
- Pandas
- Seaborn
- Matplotlib
- Scikit-learn

## ▶️ How to Run
```bash
# Run each task separately
python task1_data_collection.ipynb
python task2_data_cleaning.ipynb
python task3_EDA.ipynb
python task4_ Data_Visualization.ipynb
python task5_Predictive _Model.ipynb
```

Or run in **Google Colab** by uploading the `.ipynb` files directly.

