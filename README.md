# 🚀 Capstone Project: Space Launch Records Analysis & Prediction

## 🧠 Objective
This capstone project, part of the IBM Data Science Professional Certificate, aims to analyze space launch data with a focus on identifying key factors that influence launch success. Using interactive visualizations, geospatial mapping, SQL analysis, and predictive modeling, we explore trends in SpaceX launch activity and build a machine learning model to predict future launch outcomes.

---

## 📊 Problem Statement
Space missions are high-cost, high-stakes operations. By analyzing past launch records, this project attempts to:
- Understand trends across launch sites, payloads, orbits, and booster versions.
- Visualize success and failure distributions over time and geography.
- Build a predictive classification model to estimate the probability of a successful launch based on given inputs.

---

## 🧰 Tools & Libraries Used
- **Languages**: Python, SQL
- **Libraries**:
  - `Pandas`, `NumPy`, `Matplotlib`, `Seaborn`
  - `scikit-learn` for machine learning
  - `Folium` for interactive maps
  - `Plotly` and `Dash` for dashboards
  - `ipython-sql` for SQL in notebooks
- **Environment**: Jupyter Notebooks, GitHub

---

## 📁 Project Structure

```
space-launch-analysis/
├── data/
│   └── spacex_launch_data.csv
├── notebooks/
│   ├── 1_data_wrangling.ipynb
│   ├── 2_eda_visualization.ipynb
│   ├── 3_sql_analysis.ipynb
│   ├── 4_folium_map.ipynb
│   ├── 5_plotly_dashboard.ipynb
│   └── 6_predictive_model.ipynb
├── app/
│   └── dash_app.py
├── presentation/
│   ├── final_presentation.pdf
│   └── final_presentation.pptx
├── requirements.txt
└── README.md
```

---

## 🔍 Dataset Description
**`spacex_launch_data.csv`**  
- Features include: `Launch Site`, `Payload Mass`, `Orbit`, `Launch Outcome`, `Booster Version`, `Flight Number`, `Date`
- Target Variable: `Launch Outcome` (Success = 1, Failure = 0)

---

## 📈 Project Workflow

### 1. 📦 Data Wrangling
- Cleaned missing values and standardized columns
- Converted categorical features (Orbit, Launch Site, Booster Version) using `OneHotEncoder`
- Engineered features such as:
  - Year from Date
  - Distance from coast or city (for mapping)

### 2. 🔎 Exploratory Data Analysis (EDA)
- Plotted trends in launch count and success rate over years
- Payload mass vs. success rate correlation
- Orbit type vs. success distribution
- Launch Site and Booster Version patterns

### 3. 🧮 SQL Analysis
- Queried success rates by orbit and site using `ipython-sql`
- Summarized launch counts and average payloads using group-by queries
- Identified top-performing booster versions

### 4. 🗺️ Interactive Map (Folium)
- Marked all launch sites on a world map
- Included success/failure outcomes as colored markers
- Drew lines from launch sites to closest cities/highways

### 5. 📊 Plotly Dash Dashboard
- Created interactive filters for:
  - Launch site
  - Year
  - Payload mass
  - Booster version
- Displayed dynamic success pie charts and scatter plots

### 6. 🤖 Predictive Modeling (Classification)
- Models Tested: Logistic Regression, Support Vector Machine (SVM)
- GridSearchCV used for hyperparameter tuning
- Metrics: Accuracy, Confusion Matrix
- Best accuracy achieved: **84%** with Logistic Regression

---

## 📊 Sample Visualizations
### - Payload vs. Launch Success:
![Payload vs Success](presentation/payload_scatter.png)

### - Launch Site Map:
![Folium Map](presentation/launch_map.png)

### - Plotly Dashboard Screenshot:
![Dashboard](presentation/dash_dashboard.png)

---

## 📌 How to Run Locally

1. **Clone this repo**:
   ```bash
   git clone https://github.com/yourusername/space-launch-analysis.git
   cd space-launch-analysis
   ```

2. **Install required libraries**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Launch notebooks**:
   Open any `.ipynb` from the `notebooks/` folder in JupyterLab or Colab.

4. **Run dashboard app** (optional):
   ```bash
   python app/dash_app.py
   ```

---

## 📄 Final Presentation
- [📥 Download PDF Slides](presentation/final_presentation.pdf)
- [📂 View PowerPoint File](presentation/final_presentation.pptx)

---

## 🧑‍💻 Author
**Manisha Linguntla**  
IBM Data Science Capstone Project  
June 2025

---

## ⚖️ License
Open for educational and demonstration purposes. Credit to SpaceX and IBM for data and structure.
