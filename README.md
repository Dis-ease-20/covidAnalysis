# covidAnalysis
 
1. Subset only those rows that have “India” in the “location” column(This subsetted
dataframe has to be used for modelling)
2. Handle Missing values:
a. If there are null values in continuous numerical column, replace the null values by
the mean of that column
b. If there are null values in ordinal numerical column, replace the null values by the
mode of that column
c. If there are null values in categorical column, replace the null values by the mode
of that column
d. If more than 50%the values in a column are null, then drop that entire column
3. Univariate Analysis:
a. Draw histograms of 10 feature columns
b. Find mean, median and mode of each column
4. Bivariate Analysis:
a. Draw scatter plots of target column versus 10 features
b. Draw line plots of target column versus 10 features
5. Convert date column to ordinal
a. Code:
import datetime as dtdf["date"]=pd.to_datetime(df["date"])
df["date"]=df["date"].map(dt.datetime.toordinal)
6. Drop useless categorical columns, and convert useful categorical to numerical by
labelencoder
7. Select “total_cases” column as the target variable
8. Select the other columns as the features(NOTE: the “date” column has to be
compulsorily in the features)
9. Perform train-test split
10. Modelling:
a. Linear Regression
b. Random Forest Regressor
11. Get accuracy
12. Predict Total case for a new date

