## Запуск проекта

1.**Установка uv** 

```cmd
pip install uv
```
2.**Клонирование репозитория**

```cmd
git clone https://github.com/rztuyz/titanic-survival-prediction
cd titanic-survival-prediction
```
3.**Установка зависимостей**

```cmd
uv sync
```

## Project Structure

The repository is organized to reflect a complete machine learning workflow,
from raw data exploration to feature engineering and model training.

.
├── data/
│   ├── raw/                # Original raw dataset
│   ├── processed/          # Cleaned data after initial preprocessing
│   ├── fe/                 # Datasets after feature engineering
│   └── data_preparation.ipynb
│                           # Initial data cleaning and train/test split
│
├── eda/
│   ├── eda_overview.ipynb  # Exploratory data analysis before feature engineering
│   └── eda_fe.ipynb        # Exploratory analysis after feature engineering
│
├── features/
│   └── feature_engineering.ipynb
│                           # Feature engineering logic and feature creation
│
├── models/                 # Model training, tuning, and evaluation notebooks
│
├── catboost_info/          # CatBoost training artifacts and logs
│
├── README.md               # Project description and documentation
├── pyproject.toml          # Project dependencies
├── uv.lock                 # Dependency lock file
├── main.py                 
└── .gitignore
