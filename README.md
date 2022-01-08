# Movie-Revenue-Correlation-Project
- Downloaded an pre-existing datasets from kaggle regarding famed movies of the previous four decades
- Overlooked the dataset for missing data and the type of data
- Cleaned data to display corrected movie release years, delete duplicate entries, 
- Visualized the data to check correlation of Budget vs Revenue
- Visualized the data again to check the correlation between Directors vs Revenues

## Resources
**Jupyter Notebook Version:** 6.4.5

**Packages:** Pandas, Seaborn, Numpy, Matplotlib

**Dataset soruce:** https://www.kaggle.com/danielgrijalvas/movies

**The guide that was used:** https://www.youtube.com/watch?v=iPYVYBtUTyE&ab_channel=AlexTheAnalyst

## Data Overlook

The dataset was first overlooked for any missing data and type of data on each column. For missing data, although there were overall a low number of missing data, 
they were replaced with the number 0. The data ctypes in each columns were mostly in floats and objects

![githublarge](https://github.com/SNamStar/Movie-Revenue-Correlation-Project/blob/main/first%20import.PNG)

## Data Cleaning

The dataset than cleaned to make it more usable during modeling process. The following actions were taken:

- Changed the data type of Budget, Gross, and Vote columns from float to int
- Created "yearcorrect" column by comparing "year" and "released" columns
- Deleted at duplicate data

# Data Visualization of Budget vs Revenue

A scatter plot was made to check for correlation between budget and revenue
![githublarge](https://github.com/SNamStar/Movie-Revenue-Correlation-Project/blob/main/bvr.PNG)

And Pearson model was created for alternative view of this data:
![githublarge](https://github.com/SNamStar/Movie-Revenue-Correlation-Project/blob/main/bvrp.PNG)

# Data Visualization of Director vs Revenue

To explore of the directors affected the revenue of the movies, I first had to give numeric values to some columns of the dataset
![github-small](https://github.com/SNamStar/Movie-Revenue-Correlation-Project/blob/main/numerized.PNG)

This data was then used for Pearson modeling

![github-small](https://github.com/SNamStar/Movie-Revenue-Correlation-Project/blob/main/allp.PNG)

The relation value was also made into a list in a descending order

![githublarge](https://github.com/SNamStar/Movie-Revenue-Correlation-Project/blob/main/lista.PNG)

# Conclusion

Pearson method shows that budget and gross are indeed highly related, at 0.75 (1 being perfect relation). For Director vs Revenue, Pearson method shows that director and gross are NOT related. Budget and Gross revenue still has the closest relation, with votes vs gross coming in second place
