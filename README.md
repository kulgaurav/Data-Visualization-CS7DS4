# Data Visualization using Plotly(Python) and R

Two visualizations are recreated in this project:
* Florence Nightingale's Rose Chart from the Crimean war (also known as Coxcomb or Polar Area Chart) using Plotly
* Minard’s visualization of Napolean’s Russian Campaign using R

## Rose Chart
### Prerequisites
* Pandas
* [Plotly](https://plot.ly/)

Plotly can be directly installed using pip as:
```
pip install plotly==4.5.2
```
<img src="https://github.com/kulgaurav/Data-Visualization-CS7DS4/blob/master/RoseChart_120degree_radialAxisZoomed.png" width="900" height="500">

<img src="https://github.com/kulgaurav/Data-Visualization-CS7DS4/blob/master/RoseChart.png" width="900" height="500">

The above two visualizations are using the subset (April 1855 to March 1856) of the data. The colored areas (slices of coxcomb) represent Army mortality by three causes. The second image is rotated by 120 degrees zooming along the radial axis. Images depict that death because of zymotic diseases is way more than all other reasons. Colors are to match with the original diagram created by Florence Nightingale. This part uses Python and Plotly (graph objects' Barpolar) to create the figures. Angle for the slices is divided by months, and mortality reasons are stacked on the same base for a given month.

## Minard's Map
### Prerequisites
* r-xlsx
* r-ggrepel
* r-gridExtra
* r-tidyverse

<img src="https://github.com/kulgaurav/Data-Visualization-CS7DS4/blob/master/minardsMap.png" width="900" height="500">

This visualization recreates the Minard’s map. Data provided is split into cities, army, and temperature data frames. The size of the path represents the relative size of the military in the timeframe in that city. Yellow path symbolizes the march towards the attack, and black represents the return journey. The position of the cities is relative and plotted according to the given geographical coordinates.  The temperature graph is using the same axis and hence shares the same time during the return journey of the army. The two plots are merged together using arrangegrobs (arranging graphical objects using gridExtra library of R). The path uses a square line ends, and the plot uses a custom theme that hides axis texts, axis ticks, and panel grid to match closely with the original work of Minard. 


## Built With

* [Jupyter Notebook](jupyter.org)
* [Using the R programming language in Jupyter Notebook](https://docs.anaconda.com/anaconda/navigator/tutorials/r-lang/)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details


