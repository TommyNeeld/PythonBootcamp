# Setting up your computer
If you aren’t already setup with Python and Jupyter Notebook or JupyterLab please install either Anaconda or MiniConda. For ease, I would recommend installing Anaconda. Anaconda is a big application but is much more user-friendly - it is much bigger  because it installs almost every Python module you will ever need in addition to a nice User Interface. MiniConda is less user friendly but much lighter (basically installs Python and Conda for managing packages). With MiniConda you will likely need to import additional modules as you go. Although less user friendly, using MiniConda gives a user more control and is more suited to developers. Instructions for installing Anaconda and MiniConda are below.

First, download the **data and notebook** by cloning this repo or downloading a zip of the repo (top right). Once unzipped rename the folder to `PythonBootcamp` for simplicity.

Next install either ***MiniConda or Anaconda*** (if required):

**MiniConda:**

*If you already have MiniConda installed, skip to step 2. If you want to use Anaconda instead of MiniConda skip this section*

1. If you haven’t already got MiniConda please install MiniConda it for Python 3.7 from https://docs.conda.io/en/latest/miniconda.html (keep all default options)
2. Once installed, open `anaconda prompt (miniconda3)` by pressing the Windows button and searching ` anaconda prompt`.
3. Navigate to the `PythonBootcamp` directory using `cd` commands
4. Once in the Python directory run the command `conda install -c conda-forge -c plotly --file requirements.txt -y` from the anaconda prompt to install all modules required during this bootcamp - this may take some time. If you get the error 'CondaHTTPError: HTTP 000 CONNECTION FAILED ...' then you may need to use a network without a firewall or set a proxy.
5. Run the command `jupyter notebook`. This should open a new browser running [jupyer notebook](https://jupyter.org/). On the pannel open the file `Bootcamp.ipynb`

**Anaconda:**

*If you already have Anaconda installed, skip to step 2.*

1. Install Anaconda for Windows and Python 3.7 from https://www.anaconda.com/distribution/#windows (install the 'Graphical Installer' to avoid compilcations opening .pkg files). Follow the installation instructions and keep everything as-per the default.
2. Open the `anaconda prompt (anaconda3)` by pressing the Windows button and searching `anaconda prompt` and run the command: `conda install -c conda-forge -c plotly --file requirements.txt -y` from the anaconda prompt to install all modules required during this bootcamp. If you get the error 'CondaHTTPError: HTTP 000 CONNECTION FAILED ...' then you may need to use a network without a firewall or set a proxy.
5. Open the `anaconda navigator (anaconda3)` by pressing the Windows button and searching `anaconda navigator`. Launch a jupyter notebook session. This should load a UI in your default browser. On the panel navigate to the `PythonBootcamp` directory and open the file `Bootcamp.ipynb`. You could also open the `anaconda prompt (anaconda3)`, navigate to the `PythonBootcamp` directory and type `jupyter notebook` in the command prompt.

## Bootcamp aims:
We are going to be using an open Airbnb dataset on NewYork listings to learn how to:  
- Load and manipulate data in Pandas
- Visulise and analyse data using Matplotlib and Seaborn
- Create interactive plots using Plotly
- Mock-up a Dashboard web application using Dash (maybe)

## Data source - Airbnb
The data source we are going to use is currently the 'hottest' in [Kaggle](https://www.kaggle.com/datasets). It is the New York City Airbnb Open Data for 2019 and it is avaliable [here](https://www.kaggle.com/dgomonov/new-york-city-airbnb-open-data). 
