
# Task 2: Predict Future Stock Prices (Short-Term)

## Objective

The objective of this project is to predict the next day's stock closing price using historical stock market data and machine learning techniques.

---

## Dataset

Historical stock data was collected from Yahoo Finance using the `yfinance` Python library.

### Selected Stock

* Apple Inc. (AAPL)

### Data Features Used

* Open
* High
* Low
* Volume

### Target Variable

* Close Price

---

# Technologies and Libraries Used

* Python
* pandas
* matplotlib
* scikit-learn
* yfinance

Install required libraries using:

```bash id="0is8mv"
pip install pandas matplotlib scikit-learn yfinance
```

---

# Project Workflow

## 1. Import Libraries

The required Python libraries were imported for:

* Data handling
* Machine learning
* Visualization
* Stock data retrieval

---

## 2. Load Historical Stock Data

Stock market data was downloaded from Yahoo Finance using:

```python id="u7d95f"
yf.download("AAPL", start="2020-01-01", end="2024-01-01")
```

The first few rows of the dataset were displayed using `.head()`.

---

## 3. Feature Selection

The following columns were used as input features:

* Open
* High
* Low
* Volume

The `Close` column was selected as the prediction target.

---

## 4. Split Dataset

The dataset was divided into:

* Training data (80%)
* Testing data (20%)

using `train_test_split()`.

---

## 5. Train Machine Learning Model

A Linear Regression model was created and trained using the training dataset.

```python id="u7g4w1"
model = LinearRegression()
model.fit(X_train, y_train)
```

---

## 6. Predict Stock Prices

The trained model predicted stock closing prices using the test dataset.

```python id="gv63li"
y_pred = model.predict(X_test)
```

---

## 7. Evaluate Model

The model performance was evaluated using Mean Squared Error (MSE).

```python id="8drz01"
mean_squared_error(y_test, y_pred)
```

---

## 8. Visualize Results

A graph was plotted to compare:

* Actual Closing Prices
* Predicted Closing Prices

using matplotlib.

---

# Output

The project successfully:

* Retrieved stock market data from Yahoo Finance
* Trained a Linear Regression model
* Predicted future closing prices
* Compared actual and predicted prices visually

---

# Skills Learned

This project helped in understanding:

* Time series data handling
* Data collection using APIs
* Regression modeling
* Feature selection
* Machine learning workflows
* Data visualization using matplotlib

---

# Conclusion

This task demonstrated how machine learning can be applied to stock market prediction using historical financial data. The Linear Regression model was able to estimate future stock closing prices based on important market features such as Open, High, Low, and Volume.
