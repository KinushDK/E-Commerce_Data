# Copilot Instructions for E-Commerce Data Workspace

## Overview
This workspace is focused on data analysis for e-commerce datasets. The main files are:
- `data.csv`: The primary dataset (CSV format)
- `data.py`: Python scripts for data processing and analysis
- Jupyter notebooks (e.g., `Untitled-1.ipynb`) for interactive exploration

## Architecture & Data Flow
- Data is loaded from `data.csv` using pandas.
- Analysis, cleaning, and visualization are performed in Python (`data.py`) and notebooks.
- Notebooks are used for step-by-step exploration, visualization, and prototyping.

## Developer Workflows
- **Interactive Analysis**: Use Jupyter notebooks for exploratory data analysis and visualization.
- **Scripted Processing**: Place reusable functions and batch processing logic in `data.py`.
- **Data Loading**: Always use pandas (`pd.read_csv('data.csv')`) for reading the main dataset.
- **Visualization**: Use matplotlib, seaborn, or plotly for charts. Import conventions: `import matplotlib.pyplot as plt`, `import seaborn as sns`.

## Conventions & Patterns
- Keep notebooks focused on one analysis or experiment per file.
- Place reusable code (functions/classes) in `data.py` and import into notebooks as needed.
- Use clear, descriptive variable names for columns and analysis steps.
- Document notebook cells with markdown for clarity.
- Avoid hardcoding file paths; use relative paths (`data.csv`).

## Integration Points
- External dependencies: pandas, numpy, matplotlib (install via pip if missing).
- No complex service boundaries or cross-component communication; all logic is local to the workspace.

## Examples
- Loading data: `df = pd.read_csv('data.csv')`
- Plotting: `plt.plot(df['column'])`
- Importing functions: `from data import my_function`

## Key Files
- `data.py`: Main Python logic
- `data.csv`: Dataset
- Notebooks: Interactive analysis

---

For questions about unclear workflows or missing conventions, ask the user for clarification or examples from their recent work.