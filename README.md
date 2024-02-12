<h1 align='center'>Favorita Stores Sales Forecasting: Time Series Analysis</h1>

<h2>Business Understanding</h2>

This is a time series forecasting problem. In this project, our goal is to predict store sales on data from Corporation Favorita, a large Ecuadorian-based grocery retailer.

Specifically, to build a model that more accurately predicts the unit sales for thousands of items sold at different Favorita stores.

The training data includes dates, store, and product information, whether that item was being promoted, as well as the sales numbers. Additional files include supplementary information that may be useful in building your models

<h2>Data Preparation & Understanding</h2>

This section focuses on how the data used for this project was sourced and the columns of all the datasets used in this project.

<h3>Data Preparation</h3>

The dataset used for this project was sourced from three different places namely; Microsoft SQL Server, GitHub, and Onedrive.

<h3>Data Understanding</h3>

train.csv

* The training data, comprising time series of features store_nbr, family, and onpromotion as well as the target sales.

* store_nbr identifies the store at which the products are sold.

* family identifies the type of product sold.

* sales gives the total sales for a product family at a particular store at a given date. Fractional values are possible since products can be sold in fractional units (1.5 kg of cheese, for instance, as opposed to 1 bag of chips).

* onpromotion gives the total number of items in a product family that were being promoted at a store at a given date.

test.csv

* The test data, having the same features as the training data. You will predict the target sales for the dates in this file.

* The dates in the test data are for the 15 days after the last date in the training data.

transaction.csv

* Contains date, store_nbr and transaction made on that specific date.

sample_submission.csv is not relevant in this project.

Stores.csv

* includes city, state, type, and cluster.

* cluster is a grouping of similar stores.

oil.csv

* Daily oil price which includes values during both the train and test data timeframes. (Ecuador is an oil-dependent country and its economical health is highly vulnerable to shocks in oil prices.)

holidays_events.csv

* Holidays and Events, with metadata

- NOTE: Pay special attention to the transferred column. A holiday that is transferred officially falls on that calendar day but was moved to another date by the government. A transferred day is more like a normal day than a holiday. To find the day that it was celebrated, look for the corresponding row where type is Transfer.

- For example, the holiday Independencia de Guayaquil was transferred from 2012-10-09 to 2012-10-12, which means it was celebrated on 2012-10-12. Days that are type Bridge are extra days that are added to a holiday (e.g., to extend the break across a long weekend). These are frequently made up by the type Work Day which is a day not normally scheduled for work (e.g., Saturday) that is meant to payback the Bridge.

- Additional holidays are days added to a regular calendar holiday, for example, as typically happens around Christmas (making Christmas Eve a holiday).

- Additional Notes

Wages in the public sector are paid every two weeks on the 15th and on the last day of the month. Supermarket sales could be affected by this.

A magnitude 7.8 earthquake struck Ecuador on April 16, 2016. People rallied in relief efforts donating water and other first need products which greatly affected supermarket sales for several weeks after the earthquake.

<h2>Exploratory Data Analysis</h2>

This section encompasses how the dataset was explored to identify inconsistencies, trends, and patterns in the dataset to help us adequately deal with them in the data cleaning section.

<h2>Data Cleaning</h2>

This section encompasses all the changes and corrections that were needed to have a consistent dataset to enable a better analysis and prediction model.

<h2>Modelling and Evaluation</h2>

A total of five models were built and evaluated with the RMSLE metric and the best model was selected for hyperparameter tuning.

<h2>Conclusion</h2>

This section encompasses all the insights and final predictions on our test dataset using the model.


### Author
Prince Kwabena Amoako Aduyaw
