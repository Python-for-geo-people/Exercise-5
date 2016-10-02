# Exercise-5
Exercise 5: Analysing NOAA climate data

In this exercise you will be working with a climate data file from the [US National Oceanographic and Atmospheric Administration (NOAA) climate database](https://www.ncdc.noaa.gov/cdo-web/).
The data file [`816295.csv`](Data/816295.csv) comprises daily temperature measurements from several stations in the vicinity of the town of Ann Arbor, Michigan in the US from 1 January 1926 to 31 December 2015.
Your task is to process this data to calculate average annual temperatures for the summer and winter in each year covered by the data.

This may be a challenging exercise for some of you.
If you are having trouble, you might want to check out the [hints](hints.md).

## Part 1 - Reading and dividing the data file
Your first task is to read in the `816295.csv` data file and divide the data into separate data files for each year of data.
The data file names should follow the format `AA-####.csv`, replacing `####` with the year of the data (i.e., `AA-1926.csv`).
In order to separate each file by year, you will need to check the date of the observation in the data file and use only the year.
You should end up with one data file for each year of data.

## Part 2 - Calculating annual summer and winter temperatures
After creating the annual data files above, 

1. Read in data file (provided from NOAA climate database)
2. Split into separate files by year (e.g., AA-1926.csv, AA-1927.csv)
3. Loop over all files by year, read data and calculate average temperatures for winter (DJF) and summer (JJA), append year and mean temperature to new data files (summer-avg-temps.csv, winter-avg-temps.csv)
4. Save data files to GitHub for future use (could be a nice dataset to use for plotting. Could plot daily temperatures and seasonal averages with different symbols, possibly add a trendline)

## Notes
- Add a hints page for the less confident coders
- Add some optional challenges for the more experienced people
  - Using `glob`
  - Use functions for various parts of the code
  - Other things?
