# solar-challenge-week0

This repository contains the environment setup, basic CI configuration, and exploratory data analysis (EDA) notebooks for Week 0 of the Solar Challenge project.

## Repository Structure

solar-challenge-week0/
├─ .github/workflows/ci.yml # GitHub Actions workflow for environment validation
├─ data/ # Raw and cleaned datasets (ignored in Git)
├─ notebooks/ # Country-specific EDA notebooks
│ ├─ benin_eda.ipynb
│ ├─ sierraleone_eda.ipynb
│ └─ togo_eda.ipynb
├─ requirements.txt # Python dependencies
└─ README.md


## Environment Setup
```bash
1. Clone the repository

git clone https://github.com/mihret7/solar-challenge-week0.git
cd solar-challenge-week0

2. Create a virtual environment
# Windows
python -m venv venv
venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate

3. Install dependencies
pip install -r requirements.txt


4. Run notebooks

Open the Jupyter notebooks in VS Code or Jupyter Lab/Notebook:

jupyter notebook notebooks/<country>_eda.ipynb
Replace <country> with benin, sierraleone, or togo.

```
## Notes
- The `data/` folder is in `.gitignore` to avoid committing large CSVs.
- The CI workflow ensures environment reproducibility by installing dependencies on every push.
- Notebooks include data profiling, cleaning, EDA visualizations, and correlation analysis.