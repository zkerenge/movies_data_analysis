# 📊 Dataset Information

## 🔗 Source
**TMDB Movies Daily Updates** by `alanvourch`
- **Kaggle Page**: https://www.kaggle.com/datasets/alanvourch/tmdb-movies-daily-updates
- **Update Frequency**: Daily
- **License**: Open Data

## 📥 How to Load

This dataset is **actively updated** and too large for GitHub. It's automatically cached using `kagglehub`:

```python
import kagglehub
import os
import pandas as pd

# Download & cache latest version
path = kagglehub.dataset_download("alanvourch/tmdb-movies-daily-updates")
print(f"✅ Dataset cached at: {path}")

# List available files
files = os.listdir(path)
print(f"📂 Files: {files}")

# Load main CSV (adjust filename if needed)
df = pd.read_csv(os.path.join(path, "tmdb_movies.csv"))  # ← Update to actual filename