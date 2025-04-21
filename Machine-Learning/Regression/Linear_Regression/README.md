# 📊 Simple Linear Regression: Predicting Sales from TV Advertising

This project analyzes an advertising dataset to understand how ad spending affects product sales.
Specifically, we focus on building a **Simple Linear Regression** model using **TV ad spending** to predict **Sales**.

---

## 📁 Dataset Overview

- The dataset contains advertising data for a product, with:
  - **TV**: Money spent on TV ads (in thousands of USD)
  - **Radio**: Money spent on Radio ads (in thousands of USD)
  - **Newspaper**: Money spent on Newspaper ads (in thousands of USD)
  - **Sales**: Units sold (in thousands)

---

## 🎯 Objective

> To build a regression model that can predict **Sales** based on **advertising spend**, and to analyze the effectiveness of different advertising channels.

---

## 🧠 Why Simple Linear Regression?

- After checking the correlation matrix, **TV** showed the **strongest correlation** with **Sales** (`correlation ≈ 0.9`).
- Other features (Radio, Newspaper) had weaker or negligible correlations.
- Based on this, a **Simple Linear Regression** using **TV only** was selected to:
  - Simplify the model
  - Reduce noise from irrelevant features
  - Focus on the most impactful factor

---

## 🧪 Tools & Libraries Used

- Python
- Jupyter Notebook
- `pandas` for data handling
- `matplotlib` and `seaborn` for visualization
- `scikit-learn` for linear regression
- **[UV](https://github.com/astral-sh/uv)** package manager for fast dependency management

---

## 📊 Results

- A simple linear regression model was trained to predict **Sales** based on **TV ad spend**.
- The model showed good performance and visual fit, as shown in the scatter plot and best-fit line.
- Evaluation metrics like **MSE**, **RMSE**, and **R² Score** were used to assess accuracy.

---
## 📂 Folder Structure
```
ML-DL-Projects/
├── Machine-Learning/
│   └── Regression/
│       └── Linear_Regression/
│           ├── dataset/
│           │   └── advertising.csv
│           ├── images/
│           │   └── actual_vs_predicted.png
│           ├── notebooks/
│           │   └── Simple_Linear_Regression_Example.ipynb
│           └── README.md
├── uv.lock
├── pyproject.toml

```

---

## 🚀 Getting Started

To run this project, make sure you're inside the `ML-DL-Projects` folder and have **[UV](https://github.com/astral-sh/uv)** installed.

### Step 1: Sync dependencies

```bash
cd ML-DL-Projects
uv venv
uv pip sync
```

### Step 2: Launch Jupyter Notebook

```bash
jupyter notebook
```

---

## 💡 Future Ideas

- Try **Multiple Linear Regression** with all 3 features
- Use feature selection techniques
- Evaluate model improvement with non-linear features or polynomial regression

---

## 📬 Contact

Feel free to reach out if you have questions or want to collaborate!