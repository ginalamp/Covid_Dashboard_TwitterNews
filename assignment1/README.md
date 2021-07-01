# ISM Data Analysis
ISM Honours Data Analysis block

Johanna Engelhard and Gina Lamprecht

# Assignment 1

[Graph Allocation spreadsheet](https://docs.google.com/spreadsheets/d/1thUrLAOECz5pQ8OlmwxMl1a2i2PxGF3Oj1CnxEZAU8g/edit?usp=sharing)

Data still needed:

* check timelines
* table mapping province abbreviation to full name (could do this by hand?)

Notes on Data that we have:

* Tests, deaths, recoveries : covid19za_timeline_testing.csv
* Timeline only April and May 2020 : covid19za_provincial_cumulative_timeline_testing.csv
* South African hospital admissions -> za_national_hospital_admissions.csv (from nisc)
* [rt South Africa](https://github.com/dsfsi/covid19za/blob/master/data/calc/calculated_rt_sa_provincial_cumulative.csv) -> calculated_rt_sa_provincial_cumulative.csv
* [Global hospital admissions JSON](https://github.com/owid/covid-19-data/blob/master/public/data/internal/megafile--hospital-admissions.json)
* [Global github repo](https://github.com/owid/covid-19-data/tree/master/public/data)
* [South African github repo - most current sources](https://github.com/dsfsi/covid19za)
* [South Africa bunch of data](https://ourworldindata.org/coronavirus/country/south-africa) - extracted South African rows (was super big and took long to download, but has most complete statistics (basically everything we need other than lockdown and population data it seems) - which helps with timelines) in file: owid-covid-data_SouthAfricaExtracted_big.csv
* [Covid Lockdown Levels as text - might need scraping](https://www.gov.za/covid-19/about/about-alert-system)
* [Population per city - needs admin_name grouping and summing](https://simplemaps.com/data/za-cities) - in za_population_per_city.csv

Additional (extra) - if the big file doesn't cover it well enough
* [Excess Mortality github global](https://github.com/owid/covid-19-data/blob/master/public/data/excess_mortality/README.md)
* [Excess Mortality South Africa](https://data.humdata.org/dataset/financial-times-excess-mortality-during-covid-19-pandemic-data)

# Graph Formatting
* [Flexdashboard](https://pkgs.rstudio.com/flexdashboard/) - [Basic Row and Cols](https://blog.rstudio.com/2016/05/17/flexdashboard-easy-interactive-dashboards-for-r/)
* [General good resource](http://zevross.com/blog/2014/08/04/beautiful-plotting-in-r-a-ggplot2-cheatsheet-3/)
* [Add commas to y-axis labels](https://stackoverflow.com/questions/37713351/formatting-ggplot2-axis-labels-with-commas-and-k-mm-if-i-already-have-a-y-sc)
* [Set y axis breaks](https://stackoverflow.com/questions/22818899/setting-y-axis-breaks-in-ggplot)
* [Add specific date labels](https://www.r-graph-gallery.com/279-plotting-time-series-with-ggplot2.html)
* [Decimal formatting with scales library](https://scales.r-lib.org/reference/number_format.html)
* [Set x/y axis cartesian limits](https://ggplot2.tidyverse.org/reference/lims.html)
* [Create manual legend](https://stackoverflow.com/questions/17148679/construct-a-manual-legend-for-a-complicated-plot)
* [Manual legend columns with filling](https://stackoverflow.com/questions/58089506/ggplot2-change-fill-for-color-legend-when-fill-also-used-in-aesthetic)

## Background research
[Excess mortality](https://ourworldindata.org/excess-mortality-covid)
[Doubling rates](http://njcmindia.org/uploads/11-3_141-143.pdf)
## Instructions etc
### Overview
* Due 29 June 2021
* An analysis of COVID-19 spread in South Africa
* R markdown notebook
* Need to reproduce what is in a given page
    - Mediahack.co.za
    - All data content and graphs should be reproduced
* Notebook include wrangle, process data, create graphs
* Headings, descriptions, logical flow

### Get data
* NICD, Wordometer
* Csv’s on dataset
* Will need multiple data sources (province numbers, overall numbers, vaccinations) - combine to create overall dataset

### Assessing
* Proportion of the visualisations that you can produce, and the extent to which they correspond to the shown figures (colours don’t matter)
* How closely be able to reproduce?
* General organisation and organisation and quality of code: cleaning and wrangling data (shouldn’t be convoluted)
* Organisation of code producing the figures
* Create one theme and apply to all figures
* General structure and presentation
    - Headings
    - Explanation
    - Commented code
    - Coherent notebook
    - Introductions
* “Our report is accurate to the 23rd of June”
    - If code is written well enough, then you should be able to run it on the last day with the new data

### Questions to start with
* What data is needed?
* Where to get data?
* What format data?
* How much data do we need?
* Pivoting longer/wider


