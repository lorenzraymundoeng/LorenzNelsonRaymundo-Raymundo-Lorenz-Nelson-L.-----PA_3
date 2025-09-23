# Programming Assignment 3 | Raymundo, Lorenz Nelson L.
#### This is my submission for PA3 (Experiment 3 | Python Data Analysis)
This repository contains two Jupyter Notebooks (`Raymundo_Pandas-P1.ipynb` & `Raymundo_Pandas-P2.ipynb`) that demonstrate two programming exercises using the **Pandas** library.

Before we proceed, remember to import the pandas library to your notebook. This is a very important step because it will let you access all PANDAS functions.
```Python
import pandas as pd
```

#### Part 1: Cars Dataset Analysis with Pandas
The first exercise in this programming assignment shows how to load a .csv file into a dataframe named cars and then display the first and last five rows of the dataframe.\
To do this, we must first download the .csv file and save it to the same directory as your notebook. 

Download `cars.csv`

After that, we can now load it into our notebook by typing:
```Python
# To load the .csv file,
cars = pd.read_csv('cars.csv')
# To display the entire dataframe,
cars
```
In order to display the first five rows of the dataframe, we use the .head() function. 
```Python
cars.head()
```
And to display the last five rows of the dataframe, we use the .tail() function.
```Python
cars.tail()
```

#### Part 2: Extracting information using Subsetting, Slicing, and Indexing Operations
The second exercise in this programming assignment shows how to extract information from the previous dataframe using `Subsetting`, `Slicing`, and `Indexing`\
For task 2a, we must display the first five rows with odd-numbered columns.\
To do this, we can use integer-location-based indexing or iloc
```Python
# Select all odd-numbered columns using iloc with step = 2 starting from index 1
odd = cars.iloc[:, 1::2] # ':' means select all rows, '1' is the starting index, and '::2' means step by 2.

# To display the first five rows with odd-numbered columns, we use the .head() function
result = odd.head()

# To display,
result
```
For task 2b, we must display the row that contains the ‘Model’ of ‘Mazda RX4’\
To do this, we must look at the dataframe and see at which index 'Mazda RX4' is. For this, we use slicing
```Python
# Since Mazda RX4 is at the first row,
cars[0:1] #starts at index 0 (first row) and ends before index 1 (second row). 0 (inclusive), 1(exclusive)
```
For task 2c, we are asked how many cylinders the car model ‘Camaro Z28’ has.\
To do this, we can use .loc, an indexer used for label-based selection by row and column labels.
```Python
# Locate the row(s) where the 'Model' column equals 'Camaro Z28', and only show the 'Model' and 'cyl' (cylinders) columns
cars.loc[cars['Model'] == 'Camaro Z28' , ['Model', 'cyl]]
```
For task 2d, we are asked to determine how many cylinders and what gear type do the car models ‘Mazda RX4 Wag’, ‘Ford Pantera L’ and ‘Honda Civic’ have.
To do this, we can also use .loc
```Python
# We can see from the dataframe that the 'Mazda RX4 Wag' is at index 1; 'Ford Pantera L' is at index 28; 'Honda Civic' is at index 18,
cars.loc[[1,28,18],['Model', 'cyl', 'gear']]
```

#### Pre-requisites
- Python 3.0 or later

#### Installation
These codes were created on Jupyter Notebook. Make sure to install Anaconda Navigator and access Jupyter Notebook. It's all for free! Alternatively, you could use VS Code to run the code.

## How to Run
1.  Download the `Raymundo_Pandas-P1.ipynb` & `Raymundo_Pandas-P2.ipynb` files.
2.  Start the Jupyter Notebook server:
3.  Your web browser will open, upload `Raymundo_Pandas-P1.ipynb` & `Raymundo_Pandas-P2.ipynb`, and then click on them both to open and run the notebooks.
