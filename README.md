
<div align="center">
<h1>Do not 😴 on linear models</h1>
<h2>Simple and Interpretable Techniques Outperform Deep Learning for Sleep Scoring</h2>
</div>

Code from the paper *Do Not Sleep on Linear Models: Simple and Interpretable Techniques Outperform Deep Learning for Sleep Scoring*.

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

