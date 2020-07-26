# Data Preprocessing Workshop

## Installation Instructions

### Option 1: Docker
1. Install Docker.
2. Clone this repo.
3. `cd` into this repo.
4. Run `docker-compose build`.
5. To access the notebooks, run `docker-compose up` and go to the URL in the terminal output. 

Docker Compose is automatically configured to launch JupyterLab. If you'd like to disable it, remove the following two lines from `docker-compose.yml`:


    environment:
      - JUPYTER_ENABLE_LAB=1

   and repeat steps 4 and 5.

### Option 2: Virtualenv
1. Install virtualenv using `pip3` (this workshop is specifically made for Python 3).
2. Clone this repo and `cd` into it.
3. Create a virtual environment with `python -m venv venvname`. Feel free to replace `venvname` with whatever you'd like to name the environment.
4. Type `source venvname/bin/activate` to activate the environment.
5. Run `pip install -r requirements.txt`.
6. Run `jupyter notebook` to launch Jupyter Notebook, or `jupyter lab` to launch JupyterLab.

## Workshop Outline

Each bullet will include hands-on exercises.

### Day 1
Section 1: First steps of preprocessing
- Setup and introduction to preprocessing
- Dealing with missing data
- Exploring data types
- Class distribution and imbalance

Section 2: Standardizing data for machine learning
- What is standardization, and when should you standardize?
- Log normalization
- Scaling for feature comparison
- Standardization and modeling

### Day 2
Section 1: Extracting information from features
- What is feature engineering? 
- Extracting features using regular expressions
- Encoding variables
- Aggregate statistics

Section 2: Feature selection
- What is feature selection, and when should you manually remove features?
- Removing correlated features
- Using dimensionality reduction for feature selection
- Using PCA to train a dataset
