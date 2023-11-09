# Data Science Cookie Cutter for Prefect

## Why Should You Use This Template?

This template allows you to:

:white_check_mark: Create a readable structure for your  project

:white_check_mark: Automatically run tests when committing your code

:white_check_mark: Enforce type hints at runtime 

:white_check_mark: Check issues in your code before committing

:white_check_mark: Efficiently manage the dependencies in your project

:white_check_mark: Create short and readable commands for repeatable tasks

:white_check_mark: Rerun only modified components of a pipeline

:white_check_mark:	Automatically document your code

:white_check_mark:	Observe and automate your code

## Tools used in this project
* [Poetry](https://python-poetry.org/): Dependency management
* [Prefect](https://www.prefect.io/): Orchestrate and observe your data pipeline
* [Pydantic](https://docs.pydantic.dev/): Data validation using Python type annotations
* [pre-commit plugins](https://pre-commit.com/): Automate code reviewing formatting
* Makefile: Create short and readable commands for repeatable tasks
* [GitHub Actions](https://docs.github.com/en/actions): Automate your workflows, making it faster to build, test, and deploy your code
* [pdoc](https://github.com/pdoc3/pdoc): Automatically create an API documentation for your project
  
## Project structure
```bash
.
├── data            
│   ├── final                       # data after training the model
│   ├── processed                   # data after processing
│   ├── raw                         # raw data
├── docs                            # documentation for your project
├── .flake8                         # configuration for flake8 - a Python formatter tool
├── .gitignore                      # ignore files that cannot commit to Git
├── Makefile                        # store useful commands to set up the environment
├── models                          # store models
├── notebooks                       # store notebooks
├── .pre-commit-config.yaml         # configurations for pre-commit
├── pyproject.toml                  # dependencies for poetry
├── README.md                       # describe your project
├── src                             # store source code
│   ├── __init__.py                 # make src a Python module
│   ├── config.py                   # store configs 
│   ├── process.py                  # process data before training model
│   ├── run_notebook.py             # run notebook
│   └── train_model.py              # train model
└── tests                           # store tests
    ├── __init__.py                 # make tests a Python module 
    ├── test_process.py             # test functions for process.py
    └── test_train_model.py         # test functions for train_model.py
```

## How to use this project

Install Cookiecutter:
```bash
pip install cookiecutter
```

Create a project based on the template:
```bash
cookiecutter https://github.com/HerveMignot/data-science-template --checkout prefect-poetry
```
