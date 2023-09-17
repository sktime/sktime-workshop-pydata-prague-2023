Welcome to the sktime workshop at PyData Prague 2023
=================================================

This tutorial is about [sktime] - a unified framework for machine learning with time series. sktime contains algorithms and tools for building, applying, evaluating modular pipelines and composites for a variety of time series learning tasks, including forecasting, classification, regression.

`sktime` is easily extensible by anyone, and interoperable with the python data science stack.

This is an introductory `sktime` half-day tutorial with:

* a general introduction to `sktime`
* forecasting with `sktime` - uni/multivariate, hierarchical/global, probabilistic
* feature extraction, transformation pipelines, parameter tuning
* advanced pipeline including autoML and graphical pipelines
* evaluation and benchmarking in sktime.

[sktime]: https://www.sktime.net

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sktime/sktime-workshop-pydata-prague-2023/main?filepath=notebooks) [![!discord](https://img.shields.io/static/v1?logo=discord&label=discord&message=chat&color=lightgreen)](https://discord.com/invite/54ACzaFsn7) [![!slack](https://img.shields.io/static/v1?logo=linkedin&label=LinkedIn&message=news&color=lightblue)](https://www.linkedin.com/company/scikit-time/)

## :rocket: How to get started

In the tutorial, we will move through notebooks section by section.

You have different options how to run the tutorial notebooks:

* Run the notebooks in the cloud on [Binder] - for this you don't have to install anything!
* Run the notebooks on your machine. [Clone] this repository, get [conda], install the required packages (`sktime`, `seaborn`, `jupyter`) in an environment, and open the notebooks with that environment. For detail instructions, see below. For troubleshooting, see sktime's more detailed [installation instructions].
* or, use python venv, and/or an editable install of this repo as a package. Instructions below.

[Binder]: https://mybinder.org/v2/gh/sktime/sktime-workshop-pydata-prague-2023/main?filepath=notebooks
[clone]: https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository
[conda]: https://docs.conda.io/en/latest/
[installation instructions]: https://www.sktime.net/en/latest/installation.html

Please let us know on the [sktime discord](https://discord.com/invite/54ACzaFsn7) if you have any issues during the conference, or join to ask for help anytime.

## :bulb: Description


This workshop presents  [sktime] - a unified framework for machine learning with time series. sktime covers multiple time series learning problems, including time series transformation, classification and forecasting, among others.`sktime` allows you to easily apply an algorithm for one task to solve another (e.g. a scikit-learn regressor to solve a forecasting problem). In the tutorial, you will learn about how you can identify these problems, what their key differences are and how they are related.
This tutorial is an introduction to advanced forecasting techniques using sktime and its objectives encompass:

- Learn how to create forecasting pipelines that integrate forecasters and feature extraction methods.
- Explore more sophisticated and advanced forecasting scenarios and realise them using graphical pipelines and auto-ML.
- Learn how to evaluate the performance of forecasters.
- Learn how benchmarks can be created, similar to M4/M5 competitions.

Additionally, this tutorial provides an introduction to reproducibility tools, such as auditably storing model blueprints and fitted models together with a methodological primer.

`sktime` not just a package, but also an active community which aims to be welcoming to new joiners.
We invite anyone to get involved as a developer, user, supporter (or any combination of these).

## :movie_camera: Other Tutorials:

- [Pydata Berlin 2022 - Advanced Forecasting Tutorial](https://www.youtube.com/watch?v=4Rf9euAhjNc)

- [Pydata London 2022 - How to implement your own estimator in sktime](https://www.youtube.com/watch?v=S_3ewcvs_pg)

- [Pydata Global 2022 - Feature extraction, Pipelines, Tuning](https://github.com/sktime/sktime-tutorial-pydata-global-2022)

- [Pydata London 2023 - Time Series Classification, Regression, Distances & Kernels](https://github.com/sktime/sktime-tutorial-pydata-london-2023)

- [Europython 2023 - Time Series Forecasting, Classification, Distances, Kernels, Alignments with sktime](https://github.com/sktime/sktime-tutorial-europython-2023)

- [Pydata Amsterdam 2023: Probabilistic prediction, probabilistic forecasting with sktime, and probabilistic supervised regression with skpro](https://github.com/sktime/sktime-tutorial-pydata-Amsterdam-2023)


## :wave: How to contribute

If you're interested in contributing to sktime, you can find out more how to get involved [here](https://www.sktime.net/en/latest/get_involved.html).

Any contributions are welcome, not just code!

## Installation instructions for local use

To run the notebooks locally, you will need:

* a local repository clone
* a python environment with required packages installed

### Cloning the repository

To clone the repository locally:

`git clone https://github.com/sktime/sktime-workshop-pydata-prague-2023`

### Using conda env

1. Create a python virtual environment:
`conda create -y -n pycon_prague python=3.9`
2. Install required packages:
`conda install -y -n pycon_prague pip sktime seaborn jupyter pmdarima statsmodels dtw-python`
3. Activate your environment:
`conda activate pycon_prague`
4. If using jupyter: make the environment available in jupyter:
`python -m ipykernel install --user --name=pycon_prague`

### Using python venv

1. Create a python virtual environment:
`python -m venv pycon_prague`
2. Activate your environment:
 - `source pycon_prague/bin/activate` for Linux
 - `pycon_prague/Scripts/activate` for Windows
3. Install the requirements:
`pip install -r requirements`
4. If using jupyter: make the environment available in jupyter:
`python -m ipykernel install --user --name=pycon_prague`
