# Getting and Cleaning Data - Final Project

## This script:
* Downloads the ZIP file
* Unzips the ZIP file to the current working directory
* loads the testing data (subjects, x, and y)
* loads the training data(subjects, x, and y)
* loads the 'features' and 'activity labels' dimensions
* combines the x, y, and subject data sets between test and train
* removes columns within the x data set that don't contain 'mean()' or 'std()'
* smooshes x, y, and subjects together (using cbind)
* adds nice names to the combined data set
* pivots the data from wide to long
* calculates out the mean of the subject and activity for each column of x
* writes the data out to a .txt file (tidy_data_means_output.txt)