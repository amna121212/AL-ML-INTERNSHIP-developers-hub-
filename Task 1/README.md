# README.md

## Task 1: Exploring and Visualizing the Iris Dataset

### Objective

The purpose of this task is to learn how to:

* Load a dataset using pandas
* Inspect and explore data
* Generate descriptive statistics
* Visualize relationships and distributions using graphs

---

## Dataset Used

### Iris Dataset

The Iris dataset is a famous dataset used for machine learning and data analysis.
It contains measurements of iris flowers from three different species:

* Setosa
* Versicolor
* Virginica

Features included:

* Sepal Length
* Sepal Width
* Petal Length
* Petal Width
* Species

Dataset was loaded using the seaborn library.

---

## Technologies and Libraries Used

* Python
* pandas
* matplotlib
* seaborn

Install required libraries using:

```bash
pip install pandas matplotlib seaborn
```

---

## Steps Performed

### 1. Load Dataset

The Iris dataset was loaded using seaborn.

```python
iris = sns.load_dataset('iris')
```

---

### 2. Inspect Dataset

The following functions were used:

* `.shape()` → to check rows and columns
* `.columns` → to display column names
* `.head()` → to display first few rows
* `.info()` → to inspect data types and missing values
* `.describe()` → to generate summary statistics

---

### 3. Data Visualization

#### Scatter Plot

Used to show relationships between:

* Sepal Length
* Sepal Width

#### Histograms

Used to display distribution of numerical features.

#### Box Plot

Used to identify outliers in the dataset.

---

## Output

The program successfully:

* Loaded and inspected the dataset
* Displayed summary statistics
* Created visualizations using seaborn and matplotlib

---

## Learning Outcomes

Through this task, the following concepts were learned:

* Data loading with pandas
* Data inspection and exploration
* Descriptive statistics
* Basic data visualization techniques
* Using matplotlib and seaborn for plotting

---

## Conclusion

This task provided hands-on practice with exploratory data analysis (EDA) using the Iris dataset.
Visualizations helped in understanding feature distributions, relationships, and potential outliers in the data.
