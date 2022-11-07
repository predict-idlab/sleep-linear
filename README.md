
<div align="center">
<h1>Do not 😴 on traditional ML</h1>
<h2>Simple and Interpretable Techniques Are Competitive to Deep Learning for Sleep Scoring</h2>
</div>

Code from the paper *Do Not Sleep on Traditional Machine Learning: Simple and Interpretable Techniques Are Competitive to Deep Learning for Sleep Scoring*.

Preprint: https://arxiv.org/abs/2207.07753

---

## How is the code structured?

For each dataset you can find a separate notebook in the [`notebooks`](notebooks) folder.  

The notebooks allow to reproduce the results as they contain;  
1. data loading (see code in [`src` folder](src))
2. pre-processing & feature extraction
3. (seeded) machine learning experiments

| notebook | dataset |
|---|---|
| [SleepEDF-SC +- 30min.ipynb](notebooks/SleepEDF-SC%20%2B-%2030min.ipynb) | `SC-EDF-20` & `SC-EDF-78` |
| [SleepEDF-ST](notebooks/SleepEDF-ST.ipynb) | `SC-EDF-ST` |
| [MASS-SS3](notebooks/MASS-SS3.ipynb) | `MASS SS3` | 

---

## Additional experiments

The [`notebooks/other`](notebooks/other) folder contains some additional experiments;

| notebook | experiment description |
|---|---|
| [inputs_SleepEDF-SC +- 30min.ipynb](notebooks/other/inputs_SleepEDF-SC%20%2B-%2030min.ipynb) | evaluate impact of signal combination on performance for `SC-EDF-20` & `SC-EDF-78`|
| [inputs_SleepEDF-ST.ipynb](notebooks/other/inputs_SleepEDF-ST.ipynb) | evaluate impact of signal combination on performance for `SC-EDF-ST` |
| [inputs_SleepEDF-MASS.ipynb](notebooks/other/inputs_SleepEDF-MASS.ipynb) | evaluate impact of signal combination on performance for `MASS SS3` |
| [feature_selection.ipynb](notebooks/other/feature_selection.ipynb) | show the (little to no) impact of feature selection on performance |
| [feature_space_visualization.ipynb](notebooks/other/feature_space_visualization.ipynb) | `PCA` and `t-SNE` visualization of the feature vector for `SleepEDF-SC +/- 30min`|

A table showing the impact of signal combination on performance can be found in [notebooks/other/signal_combination_impact.md](notebooks/other/signal_combination_impact.md). 

---

## How to install the requirements?

This repository uses [poetry](https://python-poetry.org/) as dependency manager.  
A specification of the dependencies is provided in the [`pyproject.toml`](pyproject.toml) and [`poetry.lock`](poetry.lock) files.

You can install the dependencies in your Python environment by executing the following steps;
1. Install poetry: https://python-poetry.org/docs/#installation
2. Install the dependencies by calling `poetry install`


## How to download the datasets?

This work uses 4 (sub)sets of data;
- `SC-EDF-20`: first 20 patients (40 recordings) of Sleep-EDFx - Sleep Cassette
- `SC-EDF-78`: : all 78 patients (153 recordings) of Sleep-EDFx - Sleep Cassette
- `ST-EDF`: all 22 patients (44 recordings) of Sleep-EDFx - Sleep Telemetry
- `MASS SS3`: all 62 patients (62 recordings) of the MASS - SS3 subset

### [Sleep-EDFx](https://www.physionet.org/content/sleep-edfx/1.0.0/)

Contains the the `SC-EDF-20`, `SC-EDF-78`, and `ST-EDF` subset.

You can download & extract the data via the following commands;
```sh
mkdir data
# Download the data
wget https://physionet.org/static/published-projects/sleep-edfx/sleep-edf-database-expanded-1.0.0.zip -P data
# Extract all data
unzip data/sleep-edf-database-expanded-1.0.0.zip -d data
```

### [MASS](http://ceams-carsm.ca/mass/)

Contains the [`MASS SS3` subset](https://borealisdata.ca/dataset.xhtml?persistentId=doi:10.5683/SP3/9MYUCS).

In order to access the data you should submit a request as is described here; http://ceams-carsm.ca/mass/

