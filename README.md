# Setting up your computer
If you aren’t already setup with Python and Jupyter Notebook or JupyterLab please install either Anaconda or Miniconda. I would recommend installing Miniconda. Anaconda is more user friendly but is a huge application. Miniconda is less user friendly but much lighter (basically installs Python and Conda for managing packages). Anaconda is a much heavier application because it installs pretty much every module you will ever need. With Miniconda you will likely need to import additional modules as you go. I would recommend Miniconda - instructions below.

*Instructions before the session*
1. Go to … and download the file … .ipynb and the requirements.txt file and add them to an empty project directory folder called `PythonBootcamp`
2. Go to Kaggle and download the [New York City Airbnb Open Data](https://www.kaggle.com/dgomonov/new-york-city-airbnb-open-data/version/3#). Unzip the files and place them in the `data` folder within `PythonBootcamp`. You may need to create a kaggle account to download the data (this is worthwhile regardless as it is a great source for data and learning). 

*If you want to install Anaconda instead of Miniconda, skip to step 4. If you already have Miniconda installed, skip to step 3.*

2. If you haven’t already got Miniconda please install Miniconda it for Python 3.7 from https://docs.conda.io/en/latest/miniconda.html (keep all default options)
3. Once installed, open `anaconda prompt (miniconda3)` by pressing the Windows button and searching ` anaconda prompt`.
4. Navigate to the `PythonBootcamp` directory using `cd` commands
5. Once in the Python directory run the command `conda install -c conda-forge --file requirements.txt -y` from the anaconda prompt to install all modules required during this bootcamp - this may take some time. If you get the error 'CondaHTTPError: HTTP 000 CONNECTION FAILED ...' see the **EY network issue.** below.
6. Run the command `jupyter lab`. This should open a new browser running JupyterLab (https://jupyterlab.readthedocs.io/en/stable/). You can use either JupyterLab or Jupyter Notebook (by running `jupyter notebook`), JupyterLab is just a better version of Jupyter Notebook (in my opinion).

Miniconda setup:
1.	
2.	
When going through the installation steps add Python to path

**EY network issue.** 

If you are getting the error 'CondaHTTPError: HTTP 000 CONNECTION FAILED ...' this is because the EY network is blocking the anaconda (and pip) online repo.
To get around network issues, we use the EY proxies. These are set as environement variables during a session by running the two command below:
```
SET http_proxy=http://empweb2.ey.net:8080
SET https_proxy=https://empweb2.ey.net:8443
```
Once set commands such as `conda install <module>` should work. Unfortunetly you will have to set these every time you open a new session (open a new Anaconda Prompt).
