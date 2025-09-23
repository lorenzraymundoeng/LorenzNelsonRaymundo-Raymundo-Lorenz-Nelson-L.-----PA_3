# Programming Assignment 3 | Raymundo, Lorenz Nelson L.
#### This is my submission for PA3 (Experiment 3 | Python Data Analysis)
This repository contains a  two Jupyter Notebooks (`Raymundo_Pandas-P1.ipynb` & `Raymundo_Pandas-P2.ipynb`) that demonstrates two programming exercises using the **Pandas** library.

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
The second exercise in this programming assignment shows how to load

## Together, these notebooks provide a foundation for working with real-world datasets using pandas.

## How to Run

To run the notebook, you need to have **Anaconda Navigator** installed and open **Jupyter Notebook**.

1.  Download the `Raymundo_Pandas-P1.ipynb` & `Raymundo_Pandas-P2.ipynb` files.
2.  Start the Jupyter Notebook server:
    ```bash
    jupyter notebook
    ```
3.  Your web browser will open, upload `Raymundo_Pandas-P1.ipynb` & `Raymundo_Pandas-P2.ipynb`, and then click on them both to open and run the notebooks.
