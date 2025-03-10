# AutoXEDA - Automated Exploratory Data Analysis (EDA)

![AutoXEDA Banner](https://your-image-url.com/banner.png)

[![PyPI Version](https://img.shields.io/pypi/v/autoxeda)](https://pypi.org/project/autoxeda/)
[![Python Versions](https://img.shields.io/pypi/pyversions/autoxeda)](https://www.python.org/)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/your-username/autoxeda/blob/main/LICENSE)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://www.linkedin.com/in/2024-jahanzebahmed/)
[![GitHub](https://img.shields.io/badge/GitHub-Repo-black)](https://github.com/Jahanzeb-git/autoxeda)

## 🚀 Introduction

**AutoXEDA** is an advanced Python library designed for **automated exploratory data analysis (EDA)**. It streamlines the data analysis process by providing detailed insights, business intelligence summaries, and AI-powered suggestions. Whether you are a data scientist, analyst, or business professional, **AutoXEDA** helps you make data-driven decisions with ease.

## ✨ Features

✅ **Automated Statistical Analysis** - Get key descriptive statistics with one function call.  
✅ **Business Insights** - Generate structured insights tailored for decision-making.  
✅ **AI-Powered EDA** - Leverages LLM-based models (via API key) for intelligent data summaries.  
✅ **Customizable Detail Levels** - Choose from basic, intermediate, or detailed reports.  
✅ **Data Cleaning & Missing Values Handling** - Detects and suggests fixes for data inconsistencies.  
✅ **Correlation & Distribution Analysis** - Understand relationships between variables.  
✅ **Seamless Pandas Integration** - Works with pandas DataFrames effortlessly.  

---

## 📌 Installation

AutoXEDA is available on PyPI and can be installed easily using pip:

```bash
pip install autoxeda
```

---

## 🔥 Quick Start

Here's a quick example to get started with **AutoXEDA**:

```python
import pandas as pd
from autoxeda.core import autoeda

# Create a sample dataset
data = {"x": [10, 20, 30, 40, 50], "y": [5, 15, 25, 35, 45]}
df = pd.DataFrame(data)

# Run AutoXEDA
result = autoeda(df, analysis_type="business", api_key=None, detail_level='basic')

# Print the output
print(result)
```

---

## 📊 Example Output

```
{
    "status": "success",
    "summary": {
        "total_rows": 1000,
        "total_columns": 5,
        "missing_values": 0,
        "correlation_matrix": {...},
        "business_insights": "The data shows a positive trend..."
    }
}
```

---

## 🛠️ Advanced Usage

### 1️⃣ **Using AI-Powered Analysis**

If you want to leverage **AI-powered insights**, provide an API key:

```python
result = autoeda(df, analysis_type="business", api_key="your-api-key", temperature=0.5)
```

### 2️⃣ **Custom Detail Levels**

```python
result = autoeda(df, analysis_type="business", detail_level='detailed')
```

### 3️⃣ **Handling Large Datasets**

If your dataset is large, you can **optimize performance** by sampling:

```python
result = autoeda(df.sample(500), analysis_type="business", detail_level='basic')
```

---

## Hyperparameters
AutoXEDA allows customization through hyperparameters:

| Parameter       | Type    | Default | Description |
|---------------|--------|---------|-------------|
| `data`         | data  | Required    | Input data (DataFrame, CSV, or SQL query) |
| `analysis_type` | str    | 'business' | Type of analysis ('business' or 'prediction') |
| `api_key`     | str    | None    | API key (Your API key from Groq) |
| `max_retries`     | int    | 2    | Number of retries for failed actions |
| `columns`     | int    | None (all columns)    | Subset of columns to analyze |
| `detail_level` | str    | 'basic' | Level of detail ('basic', 'advanced' or 'intermediate') |
| `temperature`  | float  | 1.0    | LLM creativity level (0.0-1.0) |

---

## 📝 Contributing

We welcome contributions from the community! To contribute:
1. Fork the repository.
2. Clone it: `git clone https://github.com/Jahanzeb-git/autoxeda.git`
3. Create a new branch: `git checkout -b feature-branch`
4. Make your changes and commit: `git commit -m "Add new feature"`
5. Push the changes: `git push origin feature-branch`
6. Submit a pull request with a clear description of your contribution.

---

## 📄 License

This project is licensed under the **GNU General Public License v3.0**. See the [LICENSE](https://github.com/Jahanzeb-git/autoxeda/blob/main/LICENSE) file for details.

---

## 🌎 Connect with Me

- 📂 **GitHub**: [Jahanzeb-git](https://github.com/Jahanzeb-git/autoxeda)  
- 🌐 **Website**: [jahanzebahmed.com](https://jahanzebahmed.netlify.app)  
- 💼 **LinkedIn**: [Jahanzeb Ahmed](https://www.linkedin.com/in/2024-jahanzebahmed/)  

---

⭐ **If you like this project, don't forget to star it on GitHub!** ⭐


