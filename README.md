# 🚀 Space Launch Records Analysis & Prediction (Capstone Project)

## 📌 Project Overview
This project is the final capstone of the IBM Data Science Professional Certificate. It explores **SpaceX launch data** using various data science techniques, including **data wrangling**, **exploratory data analysis**, **SQL queries**, **geospatial mapping**, **interactive dashboards**, and **machine learning** to predict launch success.

---

## 🎯 Objective
- Analyze patterns and trends from past space launch records.
- Use interactive visualization tools to explore data from multiple perspectives.
- Build predictive models to forecast the success of a launch based on key factors.

---

## 🧾 Dataset Description
The dataset is a collection of historical SpaceX launch records, including:
- **Launch Site**
- **Payload Mass**
- **Orbit Type**
- **Launch Outcome (Success/Failure)**
- **Booster Version**
- **Flight Number**
- **Launch Date**
- **Landing Pad Info**

Target variable: `class` (1 for success, 0 for failure)

---

## 🛠 Tools & Technologies Used
- **Python Libraries**: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`
- **Visualization**: `folium`, `plotly`, `dash`
- **Database Querying**: `ipython-sql`
- **Development Tools**: Jupyter Notebook, Git, GitHub

---

## 📁 Project Structure

```
space-launch-capstone/
├── Data/                       # Data files
├── Notebooks/                 # Jupyter Notebooks for each task
├── presentation/              # Final presentation PDF & screenshots
├── app/                       # Dash interactive dashboard
├── requirements.txt           # Python dependencies
└── README.md                  # Project summary
```

---

## 🔎 Exploratory Data Analysis (EDA) – Insights

### 📌 Key Insights from Visual Analysis
- **Launch Site CCAFS SLC 40 and KSC LC 39A** had the highest number of launches.
- **Payload mass** between **2000–6000 kg** had the highest success rate.
- The **Falcon 9 Booster Version B5** performed most reliably.
- **Polar orbits** had slightly higher failure rates than LEO or GTO orbits.
- **Year-on-year success rates** improved significantly after 2014.

### 📊 Sample Visuals:
- Payload vs Success Scatter Plot
- Launch Success by Site Bar Chart
- Booster Version vs Success Rate
- Orbit Distribution Pie Chart

---

## 🧮 SQL Analysis – Highlights
Using SQL queries embedded in notebooks, we found:
- Launch Site **KSC LC 39A** had the **highest success rate**.
- **Booster Version B5** was used most frequently with a **>95% success rate**.
- Average payload for successful launches was **~4000 kg**.
- The number of launches **increased every year**, indicating SpaceX's expansion.

---

## 🗺️ Geospatial Mapping – Folium Map

Interactive map features:
- Launch sites marked with colored icons:
  - ✅ Green = Success
  - ❌ Red = Failure
- Distance markers to nearest cities, highways, and coastlines
- Useful for analyzing strategic site placement

---

## 📊 Dash Dashboard – Interactive Visuals

An interactive dashboard was created using **Plotly Dash**, with:
- Launch site filter
- Payload slider
- Pie charts for launch success
- Scatter plots of payload vs outcome

---

## 🤖 Predictive Modeling

### Models Tested:
- **Logistic Regression**
- **Support Vector Machine (SVM)**

### Best Model:
- **Logistic Regression with StandardScaler and GridSearchCV**
- Accuracy on test data: **84%**
- Most important features: Payload Mass, Orbit, Booster Version

### Confusion Matrix:
- True Positive: High
- False Negatives: Low

---

## 🧑‍💻 How to Run

1. Clone this repo:
```bash
git clone https://github.com/yourusername/space-launch-capstone.git
cd space-launch-capstone
```

2. Install requirements:
```bash
pip install -r requirements.txt
```

3. Launch Jupyter Notebooks:
```bash
jupyter notebook
```

4. Run the Dash app (optional):
```bash
cd app
python dash_app.py
```

## Dash Dashboard
Run the below command to the terminal.
  python3.11 -m pip install pandas dash
Run the following wget command line in the terminal to download dataset as spacex_launch_dash.csv
  wget "https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DS0321EN-SkillsNetwork/datasets/spacex_launch_dash.csv"
Download a skeleton Dash app to be completed in this lab:
  wget "https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/t4-Vy4iOU19i8y6E3Px_ww/spacex-dash-app.py"
Test the skeleton app by running the following command in the terminal:
  python3.11 spacex-dash-app.py
---

## 🖼 Final Presentation
- 📄 [PDF Report](presentation/final_presentation.pdf)
- 📊 Includes visuals, charts, maps, and prediction results

---

## 🧠 Conclusion

The analysis highlights how **payload size**, **booster version**, and **orbit type** are strong indicators of launch success. With interactive maps, dashboards, and a trained classification model, this project provides both **insightful visuals** and **predictive power** for future space missions.

---

## 👩‍🚀 Author

**Manisha Linguntla**  
IBM Data Science Capstone | June 2025

---

## 📜 License
This project is open-sourced for educational and demonstration purposes. Credit to SpaceX and IBM for data and framework.
