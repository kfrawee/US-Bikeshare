# Explore US Bikeshare Data [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) [![Awesome Badges](https://img.shields.io/badge/badges-awesome-green.svg)](https://github.com/Naereen/badges)


## Overview:
In this project, I will make use of Python to explore data related to bike share systems for three major cities in the United States—Chicago, New York City, and Washington. I will write code to import the data and answer interesting questions about it by computing descriptive statistics. I will also write a script that takes in raw input to create an interactive experience in the terminal to present these statistics.

## Software needed:
- Python 3.x, NumPy, and pandas installed using Anaconda.
- A text editor. *like [Visual Studio Code](https://code.visualstudio.com/)*
- A terminal application.

## Project Details
### Bike Share Data
Over the past decade, bicycle-sharing systems have been growing in number and popularity in cities across the world. Bicycle-sharing systems allow users to rent bicycles on a very short-term basis for a price. This allows people to borrow a bike from point A and return it at point B, though they can also return it to the same location if they'd like to just go for a ride. Regardless, each bike can serve several users per day.

Thanks to the rise in information technologies, it is easy for a user of the system to access a dock within the system to unlock or return bicycles. These technologies also provide a wealth of data that can be used to explore how these bike-sharing systems are used.

In this project, I will use data provided by [Motivate](https://www.motivateco.com/), a bike share system provider for many major cities in the United States, to uncover bike share usage patterns. I will compare the system usage between three large cities: Chicago, New York City, and Washington, DC.

### The Datasets
Randomly selected data for the first six months of 2017 are provided for all three cities. All three of the data files contain the same core **six (6)** columns:

- Start Time (e.g., 2017-01-01 00:07:57)
- End Time (e.g., 2017-01-01 00:20:53)
- Trip Duration (in seconds - e.g., 776)
- Start Station (e.g., Broadway & Barry Ave)
- End Station (e.g., Sedgwick St & North Ave)
- User Type (Subscriber or Customer)

The Chicago and New York City files also have the following two columns:
- Gender
- Birth Year

![nyc-data](https://video.udacity-data.com/topher/2018/March/5aa771dc_nyc-data/nyc-data.png)

### Statistics Computed
I will learn about bike share use in Chicago, New York City, and Washington by computing a variety of descriptive statistics. In this project, you'll write code to provide the following information:

- #1 Popular times of travel (i.e., occurs most often in the start time)
  - most common month
  - most common day of week
  - most common hour of day
- #2 Popular stations and trip
  - most common start station
  - most common end station
  - most common trip from start to end (i.e., most frequent combination of start station and end station)
- #3 Trip duration
  - total travel time
  - average travel time
- #4 User info
  - counts of each user type
  - counts of each gender (only available for NYC and Chicago)
  - earliest, most recent, most common year of birth (only available for NYC and Chicago)
  
### The Files
- [chicago.csv](https://github.com/kfrawee/US-Bikeshare/blob/master/chicago.csv)
- [new_york_city.csv](https://github.com/kfrawee/US-Bikeshare/blob/master/new_york_city.csv)
- [washington.csv](https://github.com/kfrawee/US-Bikeshare/blob/master/washington.csv)

## An Interactive Experience

[![Interactive Experience](https://i.imgur.com/HCi55Am.png)](https://youtu.be/--81WEZH6TQ?t=73 "Bikeshare Project Walkthrough")

The experience is interactive because depending on a user's input, the answers to the questions on the previous page will change! There are four questions that will change the answers:

- Would you like to see data for Chicago, New York, or Washington?
- Would you like to filter the data by month, day, or not at all?
- (If they chose month) Which month - January, February, March, April, May, or June?
- (If they chose day) Which day - Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, or Sunday?

The answers to the questions above will determine the city and timeframe on which I'll do data analysis. After filtering the dataset, users will see the statistical result of the data, and choose to start again or exit.

