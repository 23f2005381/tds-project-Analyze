# Data Processing Repository

This repository contains a Python script for processing data from an Excel file and a CI workflow to automate the linting, execution, and deployment of the results.

## Files

- `execute.py`: Python script to process data.
- `data.xlsx`: Original data file (not included in repo, replace with your own).
- `data.csv`: Converted CSV file from `data.xlsx`.
- `.github/workflows/ci.yml`: GitHub Actions workflow configuration.

## Usage

1. Ensure you have Python 3.11+ and Pandas 2.3 installed.
2. Run the script locally with `python execute.py` to process the data.
3. View results on GitHub Pages after CI completes on push to `main`.

## GitHub Actions

Upon push to the `main` branch:
- Lints Python code using `ruff`.
- Executes `execute.py`, generating `result.json`.
- Deploys `result.json` to GitHub Pages.

## View Results

Visit the GitHub Pages site to view the results in a browser.