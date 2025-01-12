# House Price Prediction Project

## **Overview**
This project aims to predict house prices based on various features such as size, location, number of rooms, and more. Using Python and popular machine learning libraries, the project walks through the entire pipeline from data preprocessing to building and evaluating predictive models.

---

## **Project Structure**
```
house_price_prediction/
├── data/                 # For raw and processed datasets
│   ├── raw/              # Store raw data files
│   ├── processed/        # Store cleaned/preprocessed data
├── notebooks/            # Optional: For any exploratory work
├── src/                  # All Python scripts
│   ├── __init__.py       # Makes this a package
│   ├── data_loader.py    # Code for loading and saving data
│   ├── preprocessing.py  # Data cleaning and feature engineering
│   ├── model.py          # Model training and evaluation
│   ├── utils.py          # Utility functions (e.g., metrics, helpers)
├── tests/                # Unit tests for your code
│   ├── test_model.py     # Tests for model training
│   ├── test_preprocessing.py # Tests for preprocessing
├── requirements.txt      # List of dependencies
├── README.md             # Overview of your project
```

---

## **Setup Instructions**

### **Step 1: Clone the Repository**
```bash
git clone <repository_url>
cd house_price_prediction
```

### **Step 2: Create a Virtual Environment**
```bash
python -m venv venv
source venv/bin/activate   # On Linux/Mac
venv\Scripts\activate     # On Windows
```

### **Step 3: Install Dependencies**
```bash
pip install -r requirements.txt
```

---

## **Usage**

### **Step 1: Add Data**
1. Place your raw dataset in the `data/raw/` directory.
2. Ensure the file is in CSV format with relevant features (e.g., `price`, `size`, `location`).

### **Step 2: Run the Main Script**
Run the project using the following command:
```bash
python main.py
```

The `main.py` script will:
1. Load the dataset.
2. Preprocess the data (e.g., handle missing values, scale features).
3. Train a Linear Regression model.
4. Output the evaluation metrics (e.g., MAE, MSE, R²).

---

## **How It Works**

1. **Data Loading:**
   - Load raw data from `data/raw/` using `data_loader.py`.

2. **Data Preprocessing:**
   - Clean missing values, scale numerical features, and encode categorical variables with `preprocessing.py`.

3. **Model Training and Evaluation:**
   - Train a linear regression model with `model.py` and evaluate it using metrics like:
     - **Mean Absolute Error (MAE)**
     - **Mean Squared Error (MSE)**
     - **R² Score**

4. **Results:**
   - Outputs evaluation metrics to assess model performance.

---

## **Key Scripts**

### 1. **`data_loader.py`**
- Functions to load and save datasets.

### 2. **`preprocessing.py`**
- Functions to handle missing values, scale features, and preprocess data.

### 3. **`model.py`**
- Functions to train and evaluate models.

### 4. **`utils.py`**
- Reusable helper functions (e.g., printing formatted outputs).

---

## **Testing**
Unit tests are provided in the `tests/` directory. Run the tests with:
```bash
pytest
```
Example tests:
- `test_preprocessing.py`: Ensures data preprocessing functions handle missing values and scale data correctly.
- `test_model.py`: Validates the correctness of the training and evaluation functions.

---

## **Future Improvements**
- Add support for more advanced models like Random Forest or XGBoost.
- Perform hyperparameter tuning with GridSearchCV.
- Create a web application interface to make predictions.
- Add feature importance analysis.

---

## **Dependencies**
The project relies on the following Python libraries:
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`

All dependencies are listed in `requirements.txt`.

---

## **Acknowledgments**
- Dataset source: [Kaggle](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data) or similar.
- Tutorials and resources from the data science community.

---

## **Contact**
For questions or feedback, please reach out at **daniel_benisti@protnmail.com**.

