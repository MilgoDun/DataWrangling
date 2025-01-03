# DataWrangling
The process of preparing Data for analysis.
Deal with missing data

How should you deal with missing data?

    Drop data
    a. Drop the whole row
    b. Drop the whole column
    Replace data
    a. Replace it by mean
    b. Replace it by frequency
    c. Replace it based on other functions

You should only drop whole columns if most entries in the column are empty. In the data set, none of the columns are empty enough to drop entirely. You have some freedom in choosing which method to replace data; however, some methods may seem more reasonable than others. Apply each method to different columns:

Replace by mean:

    "normalized-losses": 41 missing data, replace them with mean
    "stroke": 4 missing data, replace them with mean
    "bore": 4 missing data, replace them with mean
    "horsepower": 2 missing data, replace them with mean
    "peak-rpm": 2 missing data, replace them with mean

Replace by frequency:

    "num-of-doors": 2 missing data, replace them with "four".
        Reason: 84% sedans are four doors. Since four doors is most frequent, it is most likely to occur

Drop the whole row:

    "price": 4 missing data, simply delete the whole row
        Reason: You want to predict price. You cannot use any data entry without price data for prediction; therefore any row now without price data is not useful to you.
