# Buddy Bass Tournament 2020

## Introduction


## How to Run this Project
Please make sure that you have Python installed locally before proceeding. 

Clone or download this repository 
https://github.com/istarlet/buddy_bass_tournament

From the terminal 

- `jupyter notebook` 


## 1. Read Data In
`Read in data from a local csv, excel file, json, or any other file type.`


Read in five excel files with data from my dad's "Buddy Bass Tournament". 

## 2. Manipulate and Clean Your Data
`Use built-in pandas or numpy functions to do things like remove 0’s and null values where they don’t belong in your dataset.`


skiprows - I used skiprows when reading the datasets in to skip over the title so the dataframe will start at the column headings. 

pd.Series(pd.date_range()) - I created a series from date_range that starts on 06/10/2022 and then every Wednesday for the next 15 periods.

.drop() - I used drop to remove the "Big Fish/YEar (LBS)" column from the dataframe.

## 3. Analyze Your Data
`Use at least 5 different built-in Python functions to find out something about your data.`

`Do 5 basic calculations with Pandas`

## 4. Visualize Your Data
`Make 2 basic plots with matplotlib, seaborn, or any other kind of visualization library that you think looks interesting.`

## 5. Interpret Your Data and Graphical Output
`Write markdown cells in Jupyter explaining your thought process and code.`



