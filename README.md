# DataScience Task
### Author: Hadeel Sameh Hassan

## Discribtion:
1. **Import dataset**
    CSV file was imported using `pandas.read_csv('drinkMenu.csv')`
2. **Data preparation**
    * **Remove duplicates**
        A search for dublicates was done using `drinkMenu_df.duplicated()` methode and No dublicates were found.
    * **Fill null values**
        A search for Null values was done using `drinkMenu_df[i].isnull().any()` and resulted in finding missing values in "Caffeine (mg)" column with values (varries ,Varries).
        Firstly, the values were replace by `np.nan` to be accessable by the method used to fill Null values.
        Secondly, `drinkMenu_df["Caffeine (mg)"].fillna()` method was used to fillna with median beacause the distibution is skewed as was shown by the histogram.
    * **Drop unnecessary Columns**
        "Saturated Fat (g)" , " Dietary Fibre (g)" , "Vitamin C (% DV)" columns were dropped because there values are almost zeros.

3. **Data Visualisations: Using plots to answers this questions**
    * **Q1. Which drink has the highest calories from the dataset?**

        `Seaborn.catplot` was used to plot "Calories" Vs. "Beverge" Columns.The drink with highest calories is " White Chocolate Mocha (Without Whipped Cream)".

    * **Q2. Highest Sugar Drink ?**

        `Seaborn.catplot` was used to plot "Calories" Vs. "Beverge" Columns.The highest Sugar Drink is " Java Chip (Without Whipped Cream) ".



## Libraries Used :
* pandas : importing Dataset and dealing with dataframe (`pip install pandas`)
* matplotlib : drawing Histogram to determine best way to fill Null values (`pip install matplotlib`)
* numpy : Converting "Varies" to "NaN" (`pip install numpy`)
* seaborn : Visualize Data to Answer Q1 and Q2 (`pip install seaborn`)


## User Instructions :
* User only needs to have any IDE (Offline or ONline) that supports `.ipynb` Ex:(ANaconda jupyter notebooks , Google Colab,.....) to open `DataScience_Task_HadeelSameh.ipynb` file.

* Results are already displayed and comments are written.


