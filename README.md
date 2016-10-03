# Exercise-5
Exercise 5: Analysing NOAA climate data

In this exercise you will be working with a climate data file from the [US National Oceanographic and Atmospheric Administration (NOAA) climate database](https://www.ncdc.noaa.gov/cdo-web/).
The data file [`816295.csv`](Data/816295.csv) comprises daily temperature measurements (in Fahrenheit) from several stations in the vicinity of the town of Ann Arbor, Michigan in the US from 1 January 1926 to 31 December 2015.
Your task is to process this data to calculate average annual temperatures for the summer and winter in each year covered by the data.

This may be a challenging exercise for some of you.
If you are having trouble, you might want to check out the [hints](hints.md).

## Part 1 - Reading and dividing the data file
Your first task is to read in the `816295.csv` data file and divide the data into separate data files for each year of data.
The data file names should follow the format `AA-####.csv`, replacing `####` with the year of the data (i.e., `AA-1926.csv`).
In order to separate each file by year, you will need to check the date of the observation in the data file and use only the year.
You should end up with one data file for each year of data.
To help you with handling the data file, the first 5 lines of the file are displayed below.

```
STATION,STATION_NAME,ELEVATION,LATITUDE,LONGITUDE,DATE,TOBS
GHCND:USC00200230,ANN ARBOR UNIVERSITY OF MI MI US,282.2,42.28333,-83.73333,19260101,34
GHCND:USC00200230,ANN ARBOR UNIVERSITY OF MI MI US,282.2,42.28333,-83.73333,19260102,34
GHCND:USC00200230,ANN ARBOR UNIVERSITY OF MI MI US,282.2,42.28333,-83.73333,19260103,33
GHCND:USC00200230,ANN ARBOR UNIVERSITY OF MI MI US,282.2,42.28333,-83.73333,19260104,39
```

## Part 2 - Calculating annual summer and winter temperatures
After creating the annual data files above, your next task is to calculate seasonal average temperatures for each year.
This should be done by reading in each year's data file and calculating a winter average (combining months January and February) and a summer average (combining months July and August).
Thus for each year, your script should calculate two average temperature values.
These seasonal average temperature values should be appended to corresponding data files (`summer-avg-temps.csv` and `winter-avg-temps.csv`) along with the year in which the average was calculated.
Each line in the file should thus read `<year>,<avg temperature>`.
You are not required to include a header.

## Part 3 - Saving your seasonal average files to GitHub
Lastly, you should save your seasonal average files (`summer-avg-temps.csv` and `winter-avg-temps.csv`) to your GitHub repository for this exercise.
Our plan is to return to using these data files when we learn how to create data plots in Python using [matplotlib](http://matplotlib.org/).
You do not need to save the `AA-####.csv` files to GitHub.

## Optional tasks for advanced users
If you're interested in a challenge, you can try to do the following in your Python script for this week's exercise.

- Use the `glob` module to create the list of files to process in Part 2.
- Write your code in a modular format, creating functions for any parts of the code that are used repeatedly.
- Read the data files line by line, rather than all at once.

## Questions
1. 
2. 
3. 
4. 

# Answers
