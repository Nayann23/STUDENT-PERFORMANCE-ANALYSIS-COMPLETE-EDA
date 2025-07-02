# 🚧 Student Performance Analysis (INCOMPLETE - Ends at EDA)

> **Status**: 🔧 In Progress  
> This project focuses on end-to-end data analysis of the *Student Performance* dataset.  
> The goal was to understand patterns in student marks using exploratory data analysis (EDA).  
> Model-building was planned but not included in this version.

---

## 📂 Dataset Source

- Dataset: **Student Performance Data**  
- Columns include: `gender`, `race/ethnicity`, `parental level of education`, `lunch`, `test preparation course`, and scores in `math`, `reading`, and `writing`.

---

## ✅ Data Cleaning & Inspection

- Checked for **null values**, **duplicates**, and **inconsistent types**.
- Verified shape and unique values with `.shape`, `.info()`, and `.nunique()`.
- Data was already clean — no missing or corrupt values.
- Column `race/ethnicity` was renamed to `race_ethnicity` for easier access.

---

## 📊 Exploratory Data Analysis (EDA)

### 🔹 Categorical Plots
- **Gender Distribution** – Bar plot showing the count of males and females.
- **Gender vs Race/Ethnicity** – Multi-hue count plot.
- **Lunch Type by Gender** – Visualizing whether lunch type is skewed by gender.

### 🔹 Score Distributions
- **Histograms + KDE** for:
  - `math score`
  - `reading score`
  - `writing score`
- Observed **roughly normal distributions** with slight **left skew**.

### 🔹 Boxplots
- **Math Score by Gender** – Identified some low-performing outliers (possible failures).
- Helped compare central tendency and spread across gender.

### 🔹 Correlation Heatmap
- Used `sns.heatmap(df.corr())` to visualize relationships between numeric features.
- Strong correlation between all three score columns.

---

## 🧠 Key Insights
- Female students are slightly more in number in the dataset.
- Students with standard lunch and test prep tend to perform better.
- High inter-correlation between reading, writing, and math scores.
- Some outliers in score data suggest possible failures (marks < 28).

---

## 🧰 Tools & Libraries Used

- **Pandas** for data handling  
- **Matplotlib & Seaborn** for visualization  
- **Jupyter Notebook** as the IDE  

---

## 🚧 What’s Next (Planned but Not Implemented)

- Feature Engineering (total score, pass/fail logic)
- Preprocessing (encoding, scaling)
- Classification model creation
- Model evaluation

---

## 📌 Final Note

This version was intentionally capped after EDA to ensure full focus on exploratory skills.  
Future updates may include model-building.

