![Linear Regression](docs/banner.svg)

# Linear Regression

Simple and multiple linear regression in NumPy, R² / RMSE / MAE evaluation, comparison with scikit-learn, and Anscombe’s quartet.

An educational implementation by **Liam Esgueva**, developed in the Machine Learning coursework at **Comillas ICAI**. This fork retains the original course scaffold, teaching material and commit attribution.

## Start exploring

| Entry point | What to inspect |
| --- | --- |
| [Implementation](src/lab_2_3_LinearRegression.py) | Model logic and evaluation helpers |
| [Experiment notebook](notebook/Lab_2_3_LinearRegression.ipynb) | Coursework experiments and discussion |
| [Existing tests](tests/) | The original course checks |
| [Original assignment](docs/coursework.md) | Teaching instructions preserved separately |

## Run locally

```bash
git clone https://github.com/liiiaamm/ml-linear-regression.git
cd ml-linear-regression
python -m venv .venv
# Windows: .venv\Scripts\activate
# macOS / Linux: source .venv/bin/activate
python -m pip install numpy matplotlib seaborn scikit-learn pytest jupyter
python -m pytest tests -q
python -m jupyter notebook
```

Open `notebook/Lab_2_3_LinearRegression.ipynb` in Jupyter. The setup above is a starting environment; dependency compatibility and the full notebook have not been revalidated for this portfolio edition.

## Scope and limitations

Multiple regression uses an explicit matrix inverse and requires a nonsingular design matrix. Constant targets and degenerate inputs need additional handling. The Anscombe example downloads a Seaborn dataset on first use.

This repository presents the underlying learning exercise, not a production estimator. The portfolio update improves documentation; it does not claim new model performance or a freshly passing test suite.

---

[Liam’s portfolio](https://github.com/liiiaamm) · [Original classroom repository](https://github.com/ICAI-IMAT-ML/p2-3-liiiaamm)
