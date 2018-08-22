
# Kaggle Rossmann-Store-Sales-Kaggle-Competition -> CPU approach

## Prerequisites:

-> You have Anaconda already installed in your system

-> conda package manager is installed

-> pip is installed correctly, make sure you check step  1 and 2 of trouble shoot for correct pip installation 

->Downloading data from kaggle: 
  https://www.kaggle.com/c/rossmann-store-sales/data 

  Download all data from above url and extract it in data folder, your final data package should contain below list of file:

  googletrend.csv, state_names.csv, store.csv, store_states.csv, test.csv, train.csv, weather.csv, sample_submission.csv


## Project setup: 

cd into Rossmann-Store-Sales-Kaggle-Competition folder 

-> sudo conda env update -f environment-cpu.yml 

The above command creates a environment "fastai-cpu-dev" in your anaconda.

for activating newly creating environment:

-> source activate fastai-cpu-dev


## Opening Jupyter notebook

run "jupyter notebook" in your fast-ai-cpu environment, it will look something like this:

(fastai-cpu-dev) ➜  Rossmann-Store-Sales-Kaggle-Competition jupyter notebook


## Trouble Shooting

conda install -c anaconda bcolz

### Steps to make your pip default to anaconda environment:

1. First check if pip is already installed
-> which pip
if it comes something like "/usr/local/bin/pip", pip is already installed with default to local

unistall pip: -> sudo pip uninstall pip

2. After successful pip uninstallation:

-> sudo conda install pip 

now check again pip install folder:
-> which pip

it should come something like: /Users/setup/anaconda3/bin/pip


### Dependencies needed for working with fastai library( Also defined in environment-cpu.yml): 

for various ModuleNotFoundError: install below dependencies:

pip:

opencv-python
isoweek
pandas_summary
torchtext
graphviz
sklearn_pandas
feather-format
jupyter_contrib_nbextensions
plotnine
docrepr
awscli
kaggle-cli
pdpbox
seaborn


### Use below pip command to install in one go:

sudo pip install opencv-python isoweek pandas_summary torchtext feather-format graphviz jupyter_contrib_nbextensions plotnine docrepr awscli kaggle-cli pdpbox seaborn 