# Data Analysis (EDA) on the Titanic Dataset

## Overview

This project performs exploratory data analysis (EDA) on the Titanic dataset to uncover insights into passenger survival patterns. Using Python, Pandas, Seaborn, and Matplotlib, the project examines relationships between features like class, gender, age, and survival rates, showcasing skills in data preprocessing, statistical analysis, and visualization for data science applications.

## Dataset

The dataset (`train.csv`) is sourced from the Kaggle Titanic dataset and contains information about 891 passengers on the Titanic. Key columns include:

- **PassengerId**: Unique identifier for each passenger.
- **Survived**: Survival status (0 = No, 1 = Yes).
- **Pclass**: Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd).
- **Name**: Passenger's name.
- **Gender**: Male or female.
- **Age**: Passenger's age (with 177 missing values).
- **SibSp**: Number of siblings/spouses aboard.
- **Parch**: Number of parents/children aboard.
- **Ticket**: Ticket number.
- **Fare**: Ticket fare.
- **Cabin**: Cabin number (77.1% missing values).
- **Embarked**: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton).

## Features

- **Data Loading and Inspection**:
  - Loads the dataset using Pandas.
  - Displays basic information (`df.info()`) and summary statistics (`df.describe()`).
  - Identifies missing values, particularly in `Age` (19.9% missing) and `Cabin` (77.1% missing).
- **Exploratory Data Analysis**:
  - Analyzes data distribution and skewness using `df.skew()` to understand feature distributions (e.g., high skewness in `Fare` and `SibSp`).
  - Examines unique values in categorical columns like `Cabin`.
  - Visualizes correlations between numerical features using a Seaborn heatmap, revealing relationships such as a strong negative correlation between `Pclass` and `Survived` (-0.63).
- **Tools and Libraries**:
  - Python: Pandas, NumPy, Seaborn, Matplotlib
  - Jupyter Notebook for interactive analysis and visualization

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/titanic-data-analysis.git
   cd titanic-data-analysis
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Place the `train.csv` file in the `data/` directory.

## Usage

1. Open the Jupyter Notebook:

   ```bash
   jupyter notebook Titanic_Data_Analysis.ipynb
   ```

2. Update the file path in the notebook to point to your `data/train.csv` file (e.g., `./data/train.csv`).

3. Run all cells to:

   - Load and preprocess the dataset.
   - Perform statistical analysis (e.g., skewness, missing value checks).
   - Generate a correlation heatmap to visualize feature relationships.

## Repository Structure

```
titanic-data-analysis/
├── data/
│   └── train.csv            # Titanic dataset
├── Titanic_Data_Analysis.ipynb  # Main notebook
├── requirements.txt         # Python dependencies
├── README.md               # Project documentation
├── LICENSE                 # MIT License
```

## Requirements

Install the required libraries using:

```bash
pip install pandas numpy seaborn matplotlib
```

## Notes

- The dataset has significant missing values in the `Cabin` column (77.1%), which may limit its use in analysis without imputation.
- The correlation heatmap indicates that `Pclass` and `Fare` are strongly correlated with `Survived`, suggesting these features may be key predictors in survival models.
- Future enhancements could include:
  - Imputing missing `Age` and `Cabin` values.
  - Adding more visualizations (e.g., survival rates by gender or embarkation port).
  - Building a predictive model using machine learning to classify survival outcomes.
- The notebook uses a local file path (`C:\\Users\\student\\Downloads\\train.csv`). Update to a relative path (e.g., `./data/train.csv`) for portability.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contact

For questions, contact \[nayyabm16@gmail.com\] or open an issue on GitHub.