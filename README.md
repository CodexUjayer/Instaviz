📊 InstaViz – Intelligent Data Visualization






See truth, not just charts.

InstaViz is a next-generation Python visualization library built on top of Matplotlib that automatically chooses the best chart type for your data and provides natural language insights.

✨ Features

🎯 Smart Auto-Selection – Automatically picks the best chart for your data

📈 Built-in Insights – Natural language explanations of your data

🎨 Beautiful Themes – Light, dark, minimal, vibrant, corporate

🔍 One-Line EDA – Full EDA with viz.show(df)

📊 Statistical Annotations – Outliers, trends, stats

🚀 Zero Configuration – Sensible defaults

📦 Installation
pip install instaviz

🚀 Quick Start
import instaviz as viz
import pandas as pd
import numpy as np

# Create sample data
df = pd.DataFrame({
    'category': ['A', 'B', 'C', 'D'] * 25,
    'value': np.random.randn(100),
    'score': np.random.exponential(50, 100)
})

# 🔍 Automatic EDA
viz.show(df)

# 📊 Smart Plotting
viz.plot(df, x='category', y='value')

# 📈 Distribution Analysis
viz.distribution(df, 'score')

# 🆚 Category Comparison
viz.compare(df, x='category', y='value')

# 🔗 Correlation Heatmap
viz.correlate(df)

📖 API Reference
Core Functions
Function	Description
viz.show(df)	Automatic EDA dashboard
viz.plot(df, x, y)	Smart auto-plot
viz.distribution(df, column)	Distribution analysis
viz.compare(df, x, y)	Category comparison
viz.trend(df, date_col, value_col)	Time series trends
viz.correlate(df)	Correlation heatmap
viz.relationship(df, x, y)	Relationship plots
viz.target(df, target)	Feature vs target
🎨 Themes
# Available themes: 'instaviz', 'dark', 'minimal', 'vibrant', 'corporate'
viz.set_theme('dark')

⚙️ Configuration
viz.set_config(
    figsize=(12, 8),
    show_insights=True,
    auto_annotate=True,
    max_categories=20
)

🖼️ Example Gallery
Distribution Analysis
viz.distribution(df, 'price', kind='raincloud')

Time Series
viz.trend(df, 'date', 'revenue', smooth=3)

Relationship with Grouping
viz.relationship(df, 'age', 'income', hue='education')

📋 Requirements

Python >= 3.8

NumPy >= 1.20.0

Pandas >= 1.3.0

Matplotlib >= 3.5.0

SciPy >= 1.7.0

👨‍💻 Author

Md. Ujayer Hasnat

📧 Email: dev.ujayerhasnat@gmail.com

💼 LinkedIn: https://linkedin.com/in/ujayerhasnat

🐙 GitHub: https://github.com/CodexUjayer

📄 License

MIT License — see the LICENSE file for details.

⭐ Star History

If you find this project useful, please consider giving it a ⭐ on GitHub!
