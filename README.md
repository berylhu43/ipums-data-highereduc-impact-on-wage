# ipums-data-highereduc-impact-on-wage
# IPUMS Census Data Analysis

This repository contains a data analysis project using IPUMS census microdata. The goal is to explore the impact of higher education on wage return in the U.S. and conduct policy-relevant analyses using Python. 

## Project Overview

This project involves cleaning, exploring, and modeling census data obtained from IPUMS. Key analyses include:
- Data cleaning and one-hot encoding of categorical variables.
- Building predictive models to impute missing information.
- Running regression analyses to study the impact of work schedule flexibility on voting behavior.

## Data

The raw data files are not included in this repository due to licensing restrictions and file size. You will need to obtain the data files separately from [IPUMS USA](https://usa.ipums.org/usa/) following the instructions in datasource.txt.

### Data Files

- `usa_00001.csv.gz`: The main census microdata file.
- `PPHA_30545_MP01-Crosswalk.csv`: A crosswalk file with variable definitions.

**Important:**  
After downloading the data files, place them in a folder named `data/` at the project root. Then, modify your code to import the data using relative paths. For example:

```python
df = pd.read_csv("data/usa_00001.csv.gz")
cross_walk = pd.read_csv("data/PPHA_30545_MP01-Crosswalk.csv")
