# Project Title

This repository contains the code, experiments, and analysis for the study on vehicle fuel efficiency prediction and direct tailpipe CO₂ emission estimation using machine learning and explainable AI.


## Overview

This project develops a machine-learning framework for predicting vehicle fuel efficiency (`combinationmpg`) from vehicle specification data. Direct tailpipe CO₂ emissions are then estimated deterministically from predicted fuel consumption using fuel-type-specific emission factors.

The workflow includes:
- Data preprocessing
- Feature engineering
- Model training and evaluation
- Hyperparameter tuning
- Explainable AI analysis using SHAP, LIME, and permutation importance

## Project Structure

```bash
├── data/ (download form the link below)
├── notebooks/fuel-car-data-analysis.ipynb
```

## Requirements

Install Python 3.10+ recommended.

If `requirements.txt` is available:

```bash
pip install -r requirements.txt
```

If `environment.yml` is available:

```bash
conda env create -f environment.yml
conda activate your_env_name
```

## How to Run

### Option 1: Run the notebook

If the main workflow is in a Jupyter notebook:

```bash
jupyter notebook
```

Then open the notebook file and run all cells in order.

### Option 2: Run the Python script

If the main workflow is a Python script:

```bash
python main.py
```

Replace `main.py` with your actual entry file.

## Typical Workflow

1. Clone the repository:

```bash
git clone PASTE_YOUR_GITHUB_REPO_LINK_HERE
cd YOUR_REPO_NAME
```

2. Create and activate a virtual environment:

```bash
python -m venv venv
source venv/bin/activate
```

On Windows:

```bash
venv\Scripts\activate
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Run the project:

```bash
python main.py
```

## Input Data

First downlaod the dataset from 'https://www.kaggle.com/datasets/arslaan5/explore-car-performance-fuel-efficiency-data' and then place the dataset in the appropriate directory, for example:

```bash
data/
```

Update file paths in the script or notebook if needed.

## Output

The project may generate:
- Model performance tables
- Figures and plots
- SHAP explanations
- LIME local explanations
- Permutation importance rankings
- Processed datasets

These outputs are typically saved in:

```bash
outputs/
```

## Notes

- The target variable is `combinationmpg`.
- CO₂ values are not independently predicted by a separate model; they are estimated deterministically from fuel consumption.
- Results may vary slightly depending on package versions and random seed settings.

## Citation

If you use this repository, please cite the associated manuscript.


## Contact

For questions regarding the code or manuscript, please contact the repository author.
