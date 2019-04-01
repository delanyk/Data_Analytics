# Record Temperature in Seoul, South Korea

This project intends to show the current record high and low temperatures for each day of the year in Seoul, South Korea. The year of 2015 is shown as a plot against the previous 10 years. In addition, the there are representations of the 5 year records to the 10 year records, the change after 10 years, and the number of record breaking temperatures in over the records from the previous five years. 
<br/>
<br/>

##  Results
![alt Seoul Temperature](https://raw.githubusercontent.com/delanyk/Data_Analytics/master/Seoul_Temperatures/Seoul_record_temperatures.jpg)
<br/>
In this graph, the previous ten year high and low temperatures are represented in on a 365 day axis with the variance presented as the grey inset. The records broken in the year 2015 are red scatterplots over the graph.
<br/>
<br/>

![alt 10 year change](https://raw.githubusercontent.com/delanyk/Data_Analytics/master/Seoul_Temperatures/10_year_change.png)
<br/>
In these two graphs, the temperature difference from 2005 and 2015 shows how the temperatures have shifted over the previous 10 years. As shown, tempurtures of 2015 were consistantly and in many cases significantly higher than 10 years prior. Likewise, the cold temperatures, though in some cases there were significant drops, most of the points plotted show slight rise in the extreme low temperatures in 2015. 

<br/>
<br/>

![alt extreme temps](https://raw.githubusercontent.com/delanyk/Data_Analytics/master/Seoul_Temperatures/extreme_temps.png)
<br/>
This graph shows each year, with respect to the previous five years where the data was available and how many days in which records were broken that year. As a general trend, the number of record breaking high temperatures has continued to increase nearly each year, the number of record breaking low tempertures has as well been relatively consistant. As it appears within the data, each year is becoming more extreme than the previous years.

<br/>
<br/>

## Prerequisites
You will need matplotlib and pandas libraries

```bash

pip install matplotlib
pip install pandas

```

<br/>
<br/>

## Cleaning the data


Before the data could be fully processed. Theere were many things in the data that were incosistant.to ease in the evaluation, leap years were removed from the data, and the data had to be presented in a 365 days in a year rather than day and month to ease in the representation 


```python
# removing leap year
df = df[df['Month-day'] != '02-29']

# Converting to individual day
df['Date'] = pd.DatetimeIndex(df['Date']).dayofyear

```
<br/>
<br/>

## Running the Code

This can be run directly in the notebook.
However you may require jupyter-notebook as well.


```bash
sudo apt-get install jupyter-notebook
```


Import the dependencies

```python
% matplotlib notebook
import matplotlib.pyplot as plt
import pandas as pd

#import the data
df = pd.read_csv("Seoul_Temp_data.csv")
```
<br/>
<br/>

## The Data

The data for thThe data comes from a subset of The National Centers for Environmental Information (NCEI) [Daily Global Historical Climatology Network] (https://www1.ncdc.noaa.gov/pub/data/ghcn/daily/readme.txt) (GHCN-Daily). The GHCN-Daily is comprised of daily climate records from thousands of land surface stations across the globe.
<br/>
<br/>
<br/>
<br/>

## Authors


* **King De Lany** - *Initial work* - [DelanyK](https://github.com/DelanyK)



## Acknowledgments

*This project was originally inspired for University of Michigan course for Applied Data Representation in Python

