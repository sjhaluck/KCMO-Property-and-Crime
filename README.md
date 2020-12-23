# KCMO-Property-and-Crime

## Sources

### Kansas City Data (2010-2019)
The following analysis uses Kansas City, MO Data for Crime and Property Violations in 2015 and 2020.

All crime and property violation data was gathered from [OpenData KC](https://data.kcmo.org/) on December 5, 2020.

All tax and income data was gathered from [IRS Statistics](https://www.irs.gov/statistics/soi-tax-stats-individual-income-tax-statistics-zip-code-data-soi) on December 6, 2020.

Population data was gathered from [ZipAtlas](http://zipatlas.com/us/mo/kansas-city/zip-code-comparison/population-density.htm) on December 12, 2020.

Geopandas tutorial and animation adapted from [Benjamin Cooley](https://towardsdatascience.com/how-to-make-a-gif-map-using-python-geopandas-and-matplotlib-cd8827cefbc8) and [Binod](https://stackoverflow.com/questions/753190/programmatically-generate-video-or-animated-gif-in-python).

## Purpose

### Questions
- What are the comparisons between income, crime, and property violation across zip code?
- What are the recent changes in rate of crime and property violations?
- What is the relationship between income, crime, and property violations?


## Methods

### Packages
- `pandas`
- `geopandas`
- `matplotlib`
- `numpy`
- `PIL > Image`

### Techniques
- combining all crime data into a single table (`concat`)
- normalizing column names (`lower`,`map`, and `replace`)
- investigating values (`value_counts()`)
- cleaning data of duplicate and null entries (`drop_duplicates`, `dropna`)
- formatting variables to appropriate type (`astype`)
- pandas `sort_values` to organize data
- pandas `query` to isolate specific datasets
- pandas `pivot` and `join` to combine datasets
- geopandas `plot` to map different statistics across the datasets
- matplotlib `annotate` to annotate the maps
- geopandas `representative_point` to place annotations correctly on map
- matplotlib `plot` to plot time graphs and bar charts
- `PIL/Image` library to create custom animated GIFs


## Conclusion

### Context
- There is great economic diversity in Kansas City, MO.
- Kansas City uses property violation and fines to punish property violations ranging from trash in the yard to chipping paint.
- Crime rate in Kansas City has remained fairly constant since 2010.
- Property violation rate has nearly doubled over the past decade.

### Findings
- Though crimes and property violations are enforced throughout the city, their prevalence in mostly concentrated in the zip codes with lower income.
- Not only do zip codes with lower income experience more crimes and fines, but the crimes in those zip codes are more personal (higher rate of domestic violence) and more violent (higher rate of firearm use).
- These findings are consistenct across the ten most populous zip codes, accounting for over 50% of the Kansas City population and a range of average incomes.

### Summary
- In Kansas City, a lack of economic resources exposes residents to a series of dangerous and costly consequences.
- While higher property violation enforcement has increased since 2010, it has not brought improved safety to those communities; rather, it has increased their financial burden.
- It is time to reevaluate the property violation enforcement system to find new, innovative ways to bring justice, peace, and safety to those communities that need it the most.
