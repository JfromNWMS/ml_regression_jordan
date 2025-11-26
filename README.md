# Jordan Regression Final
### Author:  [JfromNWMS](https://github.com/JfromNWMS)

## Overview
This project uses the Kaggle Medical Cost Personal dataset, insurance.csv. We preprocess the data, perform EDA, and fit various linear regression models to predict insurance charges received by individuals.  Then, we give comparisons of the models to each other and declare a best fit model.

This project is a guided notebook assignment that demonstrates how to:
- Load and explore a dataset.
- Choose and justify features for predicting a target variable.
- Train a regression model and evaluate performance.
- Compare multiple regression approaches.
- Document your work in a structured Jupyter Notebook.
- Conduct a peer review of a classmate's project.

A link to the notebook can be found here: [regression_jordan.ipynb](https://github.com/JfromNWMS/ml_regression_jordan/blob/main/regression_jordan.ipynb)

## Dataset  
- We use the Medical Cost Personal Datasets from Kaggle:  
   - [Medical Cost Personal Datasets](https://www.kaggle.com/datasets/mirichoi0218/insurance)

## Peer Review
- clickable link to peer review

## Model Summary

| Model                         |    R² |    RMSE |     MAE |
|:------------------------------|------:|--------:|--------:|
| Linear Train                  | 0.864 | 4425.51 | 2389.16 |
| Linear Test                   | 0.886 | 4208.77 | 2315.03 |
| Linear Pipeline Train         | 0.864 | 4425.51 | 2389.16 |
| Linear Pipeline Test          | 0.886 | 4208.77 | 2315.03 |
| Log Linear Pipeline Train     | 0.829 | 4967.96 | 2473.66 |
| Log Linear Pipeline Test      | 0.863 | 4610.51 | 2259.47 |
| Polynomial Pipeline Train     | 0.88  | 4168.1  | 2354.85 |
| Polynomial Pipeline Test      | 0.848 | 4856.92 | 2776.89 |
| Log Polynomial Pipeline Train | 0.873 | 4280.57 | 1977.27 |
| Log Polynomial Pipeline Test  | 0.843 | 4935.53 | 2349.62 |

## Instructions to Set up Virtual Environment

Run these commands in your VS Code terminal:

```shell
# 1. Create an isolated virtual environment
uv venv

# 2. Pin a specific Python version (3.12 recommended)
uv python pin 3.12

# 3. Install all dependencies, including optional dev/docs tools
uv sync --extra dev --extra docs --upgrade

# 4. Enable pre-commit checks so they run automatically on each commit
uv run pre-commit install

# 5. Verify the Python version (should show 3.12.x)
uv run python --version
```

Next, activate the virtual environment.

Windows (PowerShell):

```script
.\.venv\Scripts\activate
```

macOS / Linux / WSL:

```script
source .venv/bin/activate
```

## Instructions to Run Jupyter Notebook Locally

### Install the Jupyter Extension for VS Code:

Open the Extensions view in VS Code by pressing Ctrl+Shift+X (Windows/Linux) or Cmd+Shift+X (Mac).
Search for "Jupyter" and install the official extension.
Open the notebook in VS Code. The file will have a .ipynb extension.

### Task 1. Select Notebook Kernel
Open the notebook (.ipynb) file in VS Code.
If prompted, select a Python interpreter that corresponds to your project’s .venv.
If not prompted:
Click the Kernel Selector in the top-right corner.
Choose the interpreter labeled with your project name and path.
Or open the Command Palette (Ctrl Shift P / Cmd Shift P) and run: Python: Select Interpreter, then pick your .venv.

### Task 2. Start and Run the Notebook
To run notebooks directly in VS Code, click on a cell and press:
<br>Shift Enter to run cell and move to next
<br>Ctrl Enter to run cell and stay in place
<br>Save often or enable File / Auto Save.
