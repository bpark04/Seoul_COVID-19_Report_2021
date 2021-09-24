# Seoul_Covid_19_Report_2021

## About
'Seoul Covid-19 Status Report 2021' is a Python project that analyzes Covid-19 infection patterns of Seoul.

A Python web scraper is written to harvest official Covid-19 infection data from Seoul Metropolitan Government’s webpage. After data scrapping, the project preprocesses and maskes text data from raw Korean JSON file to analyzable Pandas DataFrame.

This project mainly uses Pandas and Numpy to infer the Covid-19 occurrence patterns per target age, occupation, districts, and other variables.

Then, Pandas functions and Seaborn library is used to modify and visualize DataFrame


## Description
### Data Crawling and Text Preprocessing
* Preparing for Data Scraping
* A Function for scraping one pages
* Python code for combining all pages
* Data Preprocessing

### Seoul_Covid_19_Analysis
* COVID-19 Analysis by 'Date'
* COVID-19 Analysis by 'Area'
* COVID-19 Analysis by 'Transmission Route'
* COVID-19 Analysis by 'Patients Status'
* COVID-19 Analysis by 'Travel History'


## Important Notes
### Note 1
When you try to open **'Seoul_Covid_19_Analysis.ipynb'** to view, you might see `Sorry, something went wrong. Reload?` message.
This is because .ipynb file is too big to open in github. Please click 'Reload' several times more until you see the contents.
If you cannot see the contents after clicking 'Reload' more than 5 times, you can download and open the file in your machine.
I highly recommend using **Anaconda** to open the file. Please refer to **How to Download and Install** section for the detailed instruction.

### Note 2
If you choose to run the jupyter notebook files on your computer, please double-check that there is a Python function for scrapping data from the actual website named `get_multi_page_list` in **'Data Crawling & Preprocessing.ipynb'** file. As Covid-19 cases are increasing rapidly these days, it may take more than 30 minutes to run this line of the code. If you want to skip this part and save your time, you can use **'covid_19_recent_data.csv'**. This file is collected on last August, so the pattern of the result can be different from recently dataset.

## How to Download and Install

**Anaconda** is a Python distribution that makes it easy to install Python plus a number of its most often used 3rd party libraries in a flexible way. You can open **Jupyter Notebook** through Anaconda and upload the file after downloading from this repository to open.

**Download link**: https://www.anaconda.com/products/individual

After downloading Anaconda, you have to install following libraries:
* If you are using Mac OS, plsease navigate to 'Environemnt' -> 'base (root)' -> 'Open Terminal' 
* Once you open the terminal through Anaconda Navigator, please install following commands:
* Requests: `conda install -c anaconda requests`
* Beautifulsoup4: `conda install -c anaconda beautifulsoup4`
* Tdqm: `conda install -c conda-forge tdqm`
* Using `pip list` command on the terminal, double-check whether following libraries are successfully installed: `pandas`, `numpy`, and `matplotlib`
* If any of three libraries are missing, please install by commanding `pip install [library name]`


## Data Resource
* https://www.seoul.go.kr/coronaV/coronaStatus.do
