Sample Python Data Science Project
==============================

A starting point for all data science projects.

Getting Started
------------

To get started using this repo

```sh
$ pip install -r requirements.txt --upgrade
```

Ensure all tests run
```sh
python -m unittest discover ./src/common/tests/
python -m unittest discover ./tests/
```

### Setup .env File for Python Decouple

Add your environmental variables to .env file, 

```sh
PYTHONPATH="/Users/usr/PATH_TO_REPO/"
```

use it like the following in your code:

```py
from decouple import config
config('PYTHONPATH')
```

Check [here](https://simpleisbetterthancomplex.com/2015/11/26/package-of-the-week-python-decouple.html) for more information on python decouple.


Useful Notes
-----------
 
### Setup Virtual Environment
```sh
cd ./example_repo
virtualenv example_repo_env
source ./example_repo_env/bin/activate
```
 
### Database Setup for PostgreSQL
To setup Postgres and an engine for a Postgres database, refer to documentation [here](https://docs.sqlalchemy.org/en/13/core/engines.html).


Project Organization
------------

    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.testrun.org


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
