# Task 1: Iris Dataset – Data Visualization & Exploration

## Objective
Perform exploratory data analysis on the classic Iris dataset to understand:
- Feature distributions,
- Relationships between variables,
- Class separability among different Iris species.

---

## 📁 Dataset
- **Name**: Iris Dataset
- **Source**: Available in `.csv` format
- **Features**:
  - `sepal_length`, `sepal_width`, `petal_length`, `petal_width`
  - `species` (target class)

---

## 🛠️ Steps Performed

### 1. Data Loading & Inspection
- Loaded dataset using `pandas` and `seaborn`
- Viewed shape, column names, `.head()`, `.info()`, `.describe()`

### 2. Data Visualization
- **Scatter Plots**: Showed relationships between features
- **Histograms**: Displayed value distributions
- **Box Plots**: Detected outliers class-wise
- **Pairplots**: Visualized how features vary across species

---

## 📈 Key Findings
- Petal dimensions are the most useful in classifying species.
- Setosa is clearly separated, Versicolor and Virginica have some overlap.
- Minor outliers in Sepal Width for certain species.

---

## 📚 Libraries Used
- `pandas`, `matplotlib`, `seaborn`

---

## ✅ Outcome
Built strong EDA and visualization skills. This task serves as a foundation for understanding how data trends and distributions affect model performance.

