# dsview – Beautiful Interactive AI & Data Science Inside Notebooks

dsview turns your notebook into an AI studio: data exploration, model training, model comparison, and monitoring in notebook-native interactive views.

## Installation
```bash
pip install dsview
```

## Quickstart
```python
import pandas as pd
import dsview

df = pd.read_csv("data.csv")
dsview.show(df)
session = dsview.train(df, target="label")
leaderboard = dsview.compare(["logistic_regression", "random_forest"], df, target="label")
```

## MVP (v0.1.0)
- `dsview.show(data)` for dataset preview and profile
- `dsview.explore(df)` for deeper profiling and graph suggestions
- `dsview.train(df, target)` for baseline model training
- `dsview.compare(models, df, target)` for model leaderboard
- `dsview.dashboard()` for live hardware stats

## License
MIT

