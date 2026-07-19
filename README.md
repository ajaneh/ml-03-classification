# ml-03-classification

[![Workflow Guide](https://img.shields.io/badge/Pro--Guide-pro--analytics--02-green)](https://denisecase.github.io/pro-analytics-02/workflow-b-apply-example-project/)
[![Python 3.14](https://img.shields.io/badge/python-3.14%2B-blue?logo=python)](./pyproject.toml)
[![MIT](https://img.shields.io/badge/license-see%20LICENSE-yellow.svg)](./LICENSE)

> Professional Python project: building and evaluating classification models.

## Project Description

This project focuses on how to build models that predict a category.

We learn to:

- train and evaluate a classifier (e.g., decision tree, logistic regression, k-NN)
- read a confusion matrix and classification report
- interpret accuracy, precision, recall, and F1
- choose a model based on the problem and the data


Links:

- [Instructor Notebook](notebooks/ml_03_case.ipynb)
- [My notebook](notebooks/ml_03_al.ipynb)


## Command Reference

<details>
<summary>Show command reference</summary>

### In a machine terminal (open in your `Repos` folder)

After you get a copy of this repo in your own GitHub account,
open a machine terminal in your `Repos` folder:

```shell
git clone https://github.com/ajaneh/ml-03-classification

cd ml-03-classification
code .
```

### In a VS Code terminal

These are listed for convenience.
For best results, follow the detailed instructions in
[ml-03-classification guide](https://ajaneh.github.io/ml-03-classification/).

```shell
uv self update
uv python pin 3.14
uv lock --upgrade
uv sync --extra dev --extra docs --upgrade

uvx pre-commit install
uvx pre-commit autoupdate

git add -A
uvx pre-commit run --all-files
# repeat if changes were made
uvx pre-commit run --all-files

# run the example module to verify the environment (.venv/)
uv run python -m mlstudio.app_case
# run the notebook
cd notebooks
select kernel
run all

# run common chores
uv run ruff format .
uv run ruff check . --fix
uv run python -m pyright
uv run python -m pytest
uv run python -m zensical build

# save progress
git add -A
git commit -m "update"
git push -u origin main
```

</details>

## Findings and Visuals
![Selecting K](docs/images/choosingk.png)


![Model Comparison](docs/images/model_comparison.png)

![Selected Features](docs/images/feature_influence.png)

## Citation

[CITATION.cff](./CITATION.cff)

## License

[MIT](./LICENSE)
