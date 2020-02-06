# Getting-and-Cleaning-Data-Course-Project
This repo was created for the course project of Getting and Cleaning Data, a class offered through Johns Hopkins University via Coursera.
* The first step is downloading and unzipping the files and moving them into the desired working directory.
* The source code, run_analysis.R, can also be downloaded into the working directory.
* Executing the source code through an R processor, preferrably RStudio will create the tidy dataset called tidydata.txt.

### Data description
The X data contains information provided from Samsung Galaxy S smartphones, which were attached to participants. The Y data is which activity was being performed while the smartphones were attached.

The data was downloaded from the following link:

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

### Code summarized
The code combines the information in the two datasets and then extracts the mean and standard deviations from each to create the tidy dataset.

### The assignment instructions

1. Merges the training and the test sets to create one data set.
Use command rbind to combine training and test set
2. Extracts only the measurements on the mean and standard deviation for each measurement.
Use grep command to get column indexes for variable name contains "mean()" or "std()"
3. Uses descriptive activity names to name the activities in the data set
Convert activity labels to characters and add a new column as factor
4. Appropriately labels the data set with descriptive variable names.
Give the selected descriptive names to variable columns
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
Use pipeline command to create a new tidy dataset with command group_by and summarize_each in dplyr package


