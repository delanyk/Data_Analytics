# Korean Weather Phenomena and Trends Project

This project intends to show the weather phenomena and trends from three cities from different geographical points in South, Korea. It presents the annual extreme temperate trends, weather pollution, and rainfall. The left side is displayed in a violin plots to easily see the distribution of rainfall, polution and temperature per day. Graphs in the center show the mean as a solid line over the course of year plotted by month with monthly ranges of the highs and lows overlayed.The third column of graphs show the number of days with extreme conditions given a respective category.

##  Results
![alt Korean Weather Trends](https://raw.githubusercontent.com/delanyk/Data_Analytics/master/Korean_Weather_Trends/Annual_trends_korea.jpg)


## Prerequisites
You will need numpy, matplotlib, pandas and seaborn

```bash
pip install numpy
pip install matplotlib
pip install pandas
pip install seaborn
```


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
import numpy as np
import seaborn as sns
```


## The Data

The data for this project was collected from the [Korean National Weather Service](http://www.kma.go.kr/eng/index.jsp), a publically funded and open data collection. The data was collected for the years 2008 to 2017.


## Authors

* **King De Lany** - *Initial work* - [DelanyK](https://github.com/DelanyK)


## Acknowledgments

*This project was originally inspired for University of Michigan course for Applied Data Representation in Python

