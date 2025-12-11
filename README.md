# 🚢 Titanic Dataset — End-to-End Exploratory Data Analysis (EDA)

Welcome aboard!
This project dives deep into the legendary **Titanic dataset** to uncover what really influenced survival on that fateful voyage. From data cleaning to feature engineering to beautiful visualizations, this notebook is your complete guide to understanding the data **before** building any machine learning model.

---

## 🎯 **Project Objective**

The goal of this project is simple:
**To perform a complete end-to-end Exploratory Data Analysis (EDA)** that reveals key patterns, relationships, and insights hidden in the Titanic dataset.

This includes:

* Data loading and initial inspection
* Cleaning missing values
* Univariate, bivariate & multivariate exploration
* Outlier detection
* Feature engineering (yes, we give the data a little makeover ✨)
* Correlation analysis
* Automated profiling with `ydata-profiling`

By the end, we not only understand *what* happened — but *why* certain passengers were more likely to survive.

---

## 📘 **What is EDA (Exploratory Data Analysis)?**

EDA is like getting to know your data over coffee ☕ — before asking it to do anything difficult, like training a machine learning model.

It helps answer questions like:

* What does the dataset *look* like?
* Are there missing values lurking around?
* Which features matter?
* What patterns or trends jump out visually?
* Are there weird outliers trying to ruin your model later?

In other words:
**Clean first, analyze second, model last.**

---

## 🧰 **Tech Stack & Libraries**

This project uses the industry-standard data toolkit:

* **Pandas** → For data wrangling and manipulation
* **NumPy** → Mathematical backbone for numerical operations
* **Seaborn** → Gorgeous statistical plots
* **Matplotlib** → Plotting at the metal
* **ydata-profiling** → Automated EDA magic 💫

---

## 🧼 **Data Cleaning Highlights**

* Handled missing **Age** using median imputation
* Filled missing **Embarked** values with the mode
* **Cabin** had too many missing entries — so we engineered a new feature:
  `Has_Cabin` (1 = yes, 0 = nope)
* Removed noisy columns when appropriate
* Ensured the entire dataset was squeaky clean before analysis

---

## 📊 **Exploratory Analysis**

### 🔹 **Univariate Analysis**

We examined the distribution of individual features:

* Age distribution → Peaked around 20–30
* Fare → Super skewed, thanks rich people
* Sex, Pclass, Embarked → Clear class & gender imbalance

### 🔹 **Bivariate Analysis**

Survival vs each variable gave crystal-clear insights:

* Women had a *much* higher survival rate
* 1st class passengers were VIP (Very Important Passengers… literally)
* Passengers with cabins were more likely wealthy → more likely to survive
* Cherbourg port passengers had higher survival rates

### 🔹 **Multivariate Analysis**

We explored combinations like:

* Sex × Pclass
* Age × Sex × Survival

These visualizations paint a more holistic picture.

---

## 🧩 **Feature Engineering**

We upgraded the dataset with intelligent new features:

* **FamilySize** → `SibSp + Parch + 1`
* **IsAlone** → 1 if solo traveler
* **Title extraction** from passenger names → 'Mr', 'Mrs', 'Master', etc.

These engineered features turned out to be *powerful predictors* — especially **Title**, which beautifully captures age, gender, and social rank in one word.

---

## 🔥 **Key Insights (TL;DR Edition)**

* **Sex** is the strongest predictor → Women survived far more than men
* **Pclass** mattered — 1st class passengers had much higher survival rates
* **Title** (Mr/Miss/Master/etc.) tells an incredible survival story
* **Age**: Children had significantly better survival outcomes
* **FamilySize**: Best odds? Traveling with 2–4 people
* **Fare & Cabin**: Wealth significantly improved survival chances
* **Embarked**: Cherbourg passengers did better overall

Humans love patterns — and so did the Titanic passengers.

---

## 📄 **Automated EDA Report**

We generated a **full HTML profiling report** using `ydata-profiling`, which includes:

* Variable types
* Interactions
* Missing values
* Correlations
* Alerts & warnings
* Visualizations

Saved as:
➡️ **`titanic_eda.html`**

Open it in your browser and enjoy the data magic!

---

## 🚀 **Conclusion**

This project sets up a strong foundation for the next big step:
**Building a predictive machine learning model for Titanic survival.**

We now know which features matter, which don’t, and how to properly prepare the data for modeling. With insights, engineered features, and a clean dataset ready… ML awaits! 🤖

---

## 📂 **Project Contents**

```
├── Titanic-Dataset.csv
├── titanic_eda.ipynb
├── titanic_eda.html
├── README.md  ← (You’re reading it!)
```

---

## 🛳️ **Fair Winds & Following Seas**

Thanks for checking out this EDA project.
May your data always be clean and your visualizations always insightful.
