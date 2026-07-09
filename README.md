# House Price Predictor (Linear Regression)

A beginner-friendly Machine Learning project that predicts house values using **Linear Regression**. This project demonstrates a clean, end-to-end data science pipeline inside a Jupyter Notebook.

## Performance Milestone
*   **R² Score (Accuracy)**: **0.55** (The model successfully explains 55% of the variance in house prices!)
*   **Features Used**: `RM(Room)` (Average number of rooms) and `LSTAT(economic status of neighbourhood)`.

## Features & Pipeline
1.  **Feature Engineering**: Custom descriptive column mapping for easier analysis.
2.  **Data Cleaning**: Automatically removes missing `NaN` rows using `dropna()`.
3.  **Data Splitting**: Uses a standard `test_size=0.2` split (80% training, 20% testing).
4.  **Feature Scaling**: Applies `StandardScaler` to prevent data leakage by fitting *only* on the training set.
5.  **Prediction Post-Processing**: Uses `np.clip` to guarantee no house ever outputs an unrealistic negative price.

##  How to Run
1. Ensure `HousingData.csv` is downloaded in the same folder as the notebook.
2. Install dependencies: `pip install pandas scikit-learn numpy`
3. Open `Project.ipynb` in VS Code or Jupyter Notebook and select **"Run All Cells"**.
