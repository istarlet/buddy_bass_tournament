# Buddy Bass Tournament 2020

## Introduction
The Buddy Bass Tournament on Williamstown Lake was started in 1985 by twin brothers: Bob and Sam Perry. They held their final tournament season in 2020.  

In this notebook, I'll take a look at the dataset from the Buddy Bass Tournament 2020 Season to try to *insert what I'm going to do here*. I will use the following dataset: dataset/Buddy_Bass_Tournament_2020.xlsx, that I received from my dad, Sam Perry.

## How to Run this Project
<ol>
<li>Install Anaconda if you don't have it installed (https://docs.anaconda.com/anaconda/install/index.html)</li>
<li>Clone this repository from Github https://github.com/istarlet/buddy_bass_tournament/</li>
<li>Open Jupyter Notebook in Anaconda</li>
<li>Open cloned repo and run 'buddy_bass_.ipynb'</li>
</ol>

### Python packages used in this project:
<ul>
    <li>matplotlib</li>
    <li>pandas</li>
</ul>
    
# Project Requirements
## 1. Read Data In
`Read in data from a local csv, excel file, json, or any other file type.`


I read in an excel file with data from my dad's "Buddy Bass Tournament". 

## 2. Manipulate and Clean Your Data
`Use built-in pandas or numpy functions to do things like remove 0’s and null values where they don’t belong in your dataset.`

1. **skiprows** - I used skiprows when reading the datasets in to skip over the title so the dataframe will start at the column headings. 
2. **pd.Series(pd.date_range())** - I created a series from date_range that starts on 06/10/2022 and then every Wednesday for the next 15 periods.
3. **.drop()** - I used drop to remove the "Big Fish/YEar (LBS)" column from the dataframe.

## 3. Analyze Your Data
`Use at least 5 different built-in Python functions to find out something about your data.`

`Do 5 basic calculations with Pandas`

1. **.info()** - I used .info() to display information about the columns including data type and number of missing values, if any
2. **shape** - I used .shape to return the number of rows and columns in the data
3. **.describe()** - I used .describe to display a summary of statistics calculated for each column
4. **.groupby + .sum()** - I used .groupby to group the data by "Month" and calculate the sum for "Number of Boats", "Total No of Fish Caught", and "Total Weight in Pounds" by month
5. **Find tournament dates where number of boats was less than 30** - buddy_bass_2020[buddy_bass_2020["Number of Boats"] < 30]
6. **.median()** - I used .median to find the median number of fish caught 

## 4. Visualize Your Data
`Make 2 basic plots with matplotlib, seaborn, or any other kind of visualization library that you think looks interesting.`

<p align = "center"><img src = "https://user-images.githubusercontent.com/14065849/181111369-90e8fd15-009b-41c0-bee7-a6abfebb61bc.png"></p>
<p align = "center">
  <strong>Fig.1 - Scatter Plot</strong>
</p>

<p align = "center"><img src = "https://user-images.githubusercontent.com/14065849/181373938-1a81a443-0ffe-43c4-841b-cdf99bfa6d4f.png"></p>
<p align = "center">
  <strong>Fig. 2 - Bar Plot</strong>
</p>


## 5. Interpret Your Data and Graphical Output
`Write markdown cells in Jupyter explaining your thought process and code.`

Throughout my Jupyter Notebook you will find comments and markdown cells where I explain my thought process and code.

