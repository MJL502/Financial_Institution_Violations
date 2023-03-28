# Fainancial_Institution_Violations

## Description
- This project analyzes data from the FIDC to determine if there are correlations between institutions with violations and Age of Institution, Types of Institution, and FIDC region.

## RESULTS:

- About 97% of FDIC violations have occurred in banks registered after 1990.
- Banks registered with the OTS have a disproportionately high number of violations.  State banks have a disproportionately low number of violations.
- Proportionally, banks with trust departments have lower rates of violations than banks without trust departments.
- Banks in the FDIC region that report to the New York office have a disproportionately high number of violations.  Banks in the FDIC region that report to the Kansas City office have lower than expected violations.  All other regions are as expected. 

## Technologies:

- Python
- Jupyter Notebook
- Pandas
- Requests
- Conda (if you use that to create a virtual environment)


## Getting Started:

1. Clone `https://github.com/MJL502/Financial_Institution_Violations`
2. Make sure you have pandas installed on your machine (from a command line run: pip3 install pandas)
3. Make sure you have Jupyter Notebook installed on your machine (from a command line run: pip3 install jupyterlab)
4. Make sure you have Python 3.9 or later (from a command line run: pip3 install python)
5. Make sure you have Requests installed (from a command line run: pip3 install requests)
6. Open Financial_Institution_Violations.ipynb
7. Click 'Run All'
8. IF YOU PREFER NOT TO INSTALL PACKAGES ON YOUR MACHINE THERE IS A TXT FILE CALLED HowToSetUpVirtualEnvironment.txt IN THE DIRECTORY.  IT WILL EXPLAIN HOW TO SET UP A VIRTUAL ENVIRONMENT ON YOUR MACHINE.


## Features:

- [ ] 1. Reads data in from an API provided by the FIDC and creates a inst_full.csv file (or reads in inst_full.csv if the API data has already been downloaded.)  Also reads in a CSV file (ots-enforcement-order-listing.csv)  
- [ ] 2. Cleans data, removes null values, changes column names, formats data, removes unnecessary data, and performs multiple merges.
- [ ] 3. Creates 4 visualizations using Tableau.
- [ ] 4. There is a HowToSetUpVirtualEnvironment.txt in the directory that explains how to set up a virtual environment so you don't have to install packages on your machine.
- [ ] 5. The data is interepreted in the markdown and in this read me.


## LIMITATIONS:

- The data in the ots-enforcement-order-listing.csv was poorly formatted.  Many rows did not have docket numbers (the key on which the data was merged).  The names of the institutions were not consistant either, and made fuzzy matching difficult.


## OBSTACLES:

- See limitations..


## TODO:

- [ ] REFACTOR, especially the API get requests.
- [ ] Further clean the ots-enforcement-order-listing.csv data in an attempt correct formating errors and increase the amount of data that could be merged
- [ ] Compare additional factors


## LICENSE:

- None