

Code Book It provides the source of data, describes the variables,data, and any transformations or work you performed to clean up the data.
Data Source

Original data: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip Original description of the dataset: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones
Please go through README.txt file. It contains description of experiment, files in dataset.

Steps to get and clean data and find the average in run_analysis.R There are 5 parts:

    Merges the training and the test sets to create one data set.
    Extracts only the measurements on the mean and standard deviation for each measurement.
    Uses descriptive activity names to name the activities in the data set
    Appropriately labels the data set with descriptive activity names.
    Creates a second, independent tidy data set with the average of each variable for each activity and each subject.

How run_analysis.R implements the above steps:

1) Require knitr, reshape2 and data.table libraries 
2) Path to the test and train data set 
3) Load the features and activity labels 
4) Extract only mean and standard deviation column names and data 
5) Process the data. 

There are two parts processing test and train data respectively 
6) Merge data set 
7) Find the average 
8) Write the data in a txt file
