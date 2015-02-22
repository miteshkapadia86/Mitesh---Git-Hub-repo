# Introduction to Course Project

The script `run_analysis.R`performs the 5 steps described in the course project assigment
How `run_analysis.R` implements those 5 steps:
1. Checks if the file exists, otherwise it downloads;
2. Checks if the file has already been extracted to the directory;
3. Load both test and train data;
4. Load the features and activity labels;
5. Extract the mean and standard deviation column names and data;
6. Process the data;
7. Merge and creates data set: 
8. The result is saved as "./tidy-dataset.txt", a 180x68 data table (181 with column name), where as before, the first column contains subject IDs, the second column contains activity names (see below), and then the averages for each of the 66 attributes are in columns 3...68. There are 30 subjects and 6 activities, thus 180 rows in this data set with averages.


# Variables used in Project
1. Variable Names	                                                         Description
2. fileURL 	                                                -used to store file URL to download
3. dataFileZIP	                                                -used to store local zip data file
4. dirFile 	                                                -used to store directory
5. tidyDataFileAVGtxt	                                        -used to store directory and filename (.txt) of the clean/tidy data
6. x_train,
X_test, 
y_train, 
y_test, 
subject_train, 
subject_test	-used to read train and test data
7. x, y, z                                                         -used to combines data table (train vs test) by rows
8. features                                                        -used to Read features labels
9. activities                                                      -used to Read activity labels
10. index_features                                                  -used to Search for matches to argument mean or standard deviation (sd)  within each element of character vector