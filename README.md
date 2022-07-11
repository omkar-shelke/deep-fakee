# DeepSafe
WebBased DeepFake Detection

<h1 align="center">
  gdown
</h1>

<h4 align="center">
  Download a large file from Google Drive.
</h4>

<div align="center">
  <a href="https://pypi.python.org/pypi/gdown"><img src="https://img.shields.io/pypi/v/gdown.svg"></a>
  <a href="https://pypi.org/project/gdown"><img src="https://img.shields.io/pypi/pyversions/gdown.svg"></a>
  <a href="https://github.com/wkentaro/gdown/actions"><img src="https://github.com/wkentaro/gdown/workflows/ci/badge.svg"></a>
</div>

<div align="center">
  <img src=".readme/cli.png" width="90%">
  <img src=".readme/python.png" width="90%">
</div>

<br/>

Mega Drive
https://mega.nz/folder/faxWBbID#B84oIE9VEw2FvV8dEVW1XQ

Download Weights

'''
import gdown

#this takes a while cause the folder is quite big about 3.4G

# a folder
url = "https://drive.google.com/drive/folders/1Gan21zLaPD0wHbNF3P3a7BzgKE91BOpq?usp=sharing"
gdown.download_folder(url, quiet=True, use_cookies=False)


'''

## Description

Download a large file from Google Drive.  
If you use curl/wget, it fails with a large file because of
the security warning from Google Drive.
Supports downloading from Google Drive folders (max 50 files per folder).


## Installation

```bash
pip install gdown

# to upgrade
pip install --upgrade gdown
```


## Usage

### From Command Line

```bash
$ gdown --help
usage: gdown [-h] [-V] [-O OUTPUT] [-q] [--fuzzy] [--id] [--proxy PROXY]
             [--speed SPEED] [--no-cookies] [--no-check-certificate]
             [--continue] [--folder] [--remaining-ok]
             url_or_id
...

### From Python

```python
import gdown

# a folder
url = "https://drive.google.com/drive/folders/15uNXeRBIhVvZJIhL4yTw4IsStMhUaaxl"
gdown.download_folder(url, quiet=True, use_cookies=False)

# same as the above, but with the folder ID
id = "15uNXeRBIhVvZJIhL4yTw4IsStMhUaaxl"
gdown.download_folder(id=id, quiet=True, use_cookies=False)
```

# streamlit-multiapps
A simple framework in python to create multi page web application using streamlit.

# How to Run

1. Clone the repository:
```
$ git clone git@github.com:upraneelnihar/streamlit-multiapps
$ cd streamlit-multiapps
```

2. Install dependencies:
```
$ pip install -r requirements.txt
```

3. Start the application:
```
streamlit run app.py
```

Below are instructions to implement in in your local system using a separate development environment using the [Conda](http://conda.pydata.org/docs/index.html) package management system which comes bundled with the Anaconda Python distribution provided by Continuum Analytics.

### Step 1:
[Fork and clone](https://github.com/siddharthksah/Pose-Estimation-with-MediaPipe) a copy of this repository on to your local machine.

### Step 2:
Create a `conda` environment called `pose-estimation` and install all the necessary dependencies, the environment.yml file is uploaded in the repo for ease:

    $ conda env create --file environment.yml
    
### Step 3:
Install the extra dependencies required to run the webapp smoother:

    $ pip install watchdog

### Step 4:
Activate the `pose-estimation` environment:

    $ source activate pose-estimation

To confirm that everything has installed correctly, type

    $ which pip

at the terminal prompt. You should see something like the following:

    $ ~/anaconda/envs/pose-estimation/bin/pip

which indicates that you are using the version of `pip` that is installed inside the `pose-estimation` Conda environment and not the system-wide version of `pip` that you would normally use to install Python packages.

### Step 5:
Change into your local copy of the this repo:

    $ cd Pose-Estimation-with-MediaPipe

### Step 6:
Run the webapp:

    $ streamlit run main.py


Hosting on Google Cloud Run
Streamlit
Dockerized

<div align="center">

![Streamlit Prophet](streamlit_prophet/references/logo.png)

[![CI status](https://github.com/artefactory-global/streamlit_prophet/actions/workflows/ci.yml/badge.svg?branch%3Amain&event%3Apush)](https://github.com/artefactory-global/streamlit_prophet/actions/workflows/ci.yml?query=branch%3Amain)
[![Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue.svg)](#supported-python-versions)
[![Dependencies Status](https://img.shields.io/badge/dependabots-active-informational.svg)](https://github.com/artefactory-global/streamlit_prophet/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://share.streamlit.io/maximelutel/streamlit_prophet/main/streamlit_prophet/app/dashboard.py)

[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
[![Security: bandit](https://img.shields.io/badge/security-bandit-informational.svg)](https://github.com/PyCQA/bandit)
[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-informational?logo=pre-commit&logoColor=white)](https://github.com/artefactory-global/streamlit_prophet/blob/main/.pre-commit-config.yaml)
[![Semantic Versions](https://img.shields.io/badge/%F0%9F%9A%80-semantic%20versions-informational.svg)](https://github.com/artefactory-global/streamlit_prophet/releases)
[![License](https://img.shields.io/badge/License-MIT-informational.svg)](https://github.com/artefactory-global/streamlit_prophet/blob/main/LICENSE)

Deploy a [Streamlit](https://streamlit.io/) app to train, evaluate and optimize a [Prophet](https://facebook.github.io/prophet/) forecasting model visually

## ⭐  Quick Start  ⭐

[Test the app online](https://share.streamlit.io/maximelutel/streamlit_prophet/main/streamlit_prophet/app/dashboard.py) with shared computing resources & [read introductory article](https://medium.com/artefact-engineering-and-data-science/visual-time-series-forecasting-with-streamlit-prophet-71d86a769928?source=friends_link&sk=590cca0d24f53f73a9fdb0490a9a47a7)

If you plan to use the app regularly, you should install the package and run it locally:
```bash
pip install -U streamlit_prophet
streamlit_prophet deploy dashboard
```

</div>

https://user-images.githubusercontent.com/56996548/126762714-f2d3f3a1-7098-4a86-8c60-0a69d0f913a7.mp4

## 💻 Requirements

### Python version
* Main supported version : <strong>3.7</strong> <br>
* Other supported versions : <strong>3.8</strong> & <strong>3.9</strong>

Please make sure you have one of these versions installed to be able to run the app on your machine.

### Operating System
Windows users have to install [WSL2](https://docs.microsoft.com/en-us/windows/wsl/) to download the package. 
This is due to an incompatibility between Windows and Prophet's main dependency (pystan). 
Other operating systems should work fine.

## ⚙️ Installation


### Create a virtual environment (optional)
We strongly advise to create and activate a new virtual environment, to avoid any dependency issue.

For example with conda:
```bash
pip install conda; conda create -n streamlit_prophet python=3.7; conda activate streamlit_prophet
```

Or with virtualenv:
```bash
pip install virtualenv; python3.7 -m virtualenv streamlit_prophet --python=python3.7; source streamlit_prophet/bin/activate
```


### Install package
Install the package from PyPi (it should take a few minutes):
```bash
pip install -U streamlit_prophet
```

Or from the main branch of this repository:
```bash
pip install git+https://github.com/artefactory-global/streamlit_prophet.git@main
```


## 📈 Usage

Once installed, run the following command from CLI to open the app in your default web browser:

```bash
streamlit_prophet deploy dashboard
```

Now you can train, evaluate and optimize forecasting models in a few clicks.
All you have to do is to upload a time series dataset. 
This dataset should be a csv file that contains a date column, a target column and optionally some features, like on the example below:

![](streamlit_prophet/references/input_format.png)

Then, follow the guidelines in the sidebar to:

* <strong>Prepare data</strong>: Filter, aggregate, resample and/or clean your dataset.
* <strong>Choose model parameters</strong>: Default parameters are available but you can tune them.
Look at the tooltips to understand how each parameter is impacting forecasts.
* <strong>Select evaluation method</strong>: Define the evaluation process, the metrics and the granularity to
assess your model performance.
* <strong>Make a forecast</strong>: Make a forecast on future dates that are not included in your dataset,
with the model previously trained.

Once you are satisfied, click on "save experiment" to download all plots and data locally.


## 🛠️ How to contribute ?

All contributions, ideas and bug reports are welcome! 
We encourage you to open an [issue](https://github.com/artefactory-global/streamlit_prophet/issues) for any change you would like to make on this project.


For more information, see [`CONTRIBUTING`](https://github.com/artefactory-global/streamlit_prophet/blob/main/CONTRIBUTING.md) instructions.
If you wish to containerize the app, see [`DOCKER`](https://github.com/artefactory-global/streamlit_prophet/blob/main/DOCKER.md) instructions.


