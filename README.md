[README.md](https://github.com/user-attachments/files/24837769/README.md)
# House Price Regression (Linear / Ridge / Lasso)

This repo trains regression models to predict **House_Price** using:

- Square_Footage
- Num_Bedrooms
- Num_Bathrooms
- Year_Built
- Lot_Size
- Garage_Size
- Neighborhood_Quality

Includes:
- Baseline Linear Regression
- Ridge + Lasso with cross-validated regularization strength (alpha)
- Metrics: MAE, RMSE, R²
- Plots: Predicted vs Actual, Residual plot
- Jupyter notebook walkthrough

---

## Run locally

### 1) Install
```bash
python -m venv .venv
# Windows: .venv\Scripts\activate
source .venv/bin/activate

pip install -r requirements.txt
```

### 2) Train + evaluate
Ridge (recommended):
```bash
python linear_regression.py --model ridge
```

Plain Linear:
```bash
python linear_regression.py --model linear
```

Lasso:
```bash
python linear_regression.py --model lasso
```

Outputs are written to `outputs/`:
- `coefficients.csv`
- `predicted_vs_actual.png`
- `residuals.png`

---

## Notebook

```bash
jupyter notebook
```

Open: `house_price_regression.ipynb`

---

## Push to GitHub

From inside this folder:

```bash
git init
git add .
git commit -m "House price regression: linear + ridge/lasso + notebook"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git push -u origin main
```
