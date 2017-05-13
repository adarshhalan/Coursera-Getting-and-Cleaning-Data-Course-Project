# Coursera-Getting-and-Cleaning-Data-Course-Project
	
	Coursera-Getting-and-Cleaning-Data-Course-Project  

# This repo was created to finish the assignment for week 4 of Getting and Cleaning Data Coursera course.

	First, download and unzip the data file into your R working directory.
	
	Second, download the R source code into your R working directory.
	
	Finally, execute R source code to generate tidy data file.

# Files

	The code takes for granted all the data is present in the same folder, un-compressed and without names altered.

	CodeBook.md describes the variables, the data, and any transformations or work that was performed to clean up the data.

	Run_analysis.R contains all the code to perform the analyses described in the 5 steps. They can be launched in RStudio by just importing the file.

	The output of the 5th step is called tidydata.txt, and uploaded in the course project's form.

# Data description

	The variables in the data X are sensor signals measured with waist-mounted smartphone from 30 subjects. The variable in the data Y indicates activity type the subjects performed during recording.

# Code explaination

	The code combined training dataset and test dataset, and extracted partial variables to create another dataset with the averages of each variable for each activity.

# New dataset

	The new generated dataset contained variables calculated based on the mean and standard deviation. Each row of the dataset is an average of each activity type for all subjects.

# The code was written based on the instruction of this assignment

	1. Read training and test dataset into R environment. Read variable names into R envrionment. Read subject index into R  environment.
	
	2.  Merges the training and the test sets to create one data set. Use command rbind to combine training and test set
	
	3.  Extracts only the measurements on the mean and standard deviation for each measurement. Use grep command to get column indexes for variable name contains "mean()" or "std()"
	
	4.  Uses descriptive activity names to name the activities in the data set Convert activity labels to characters and add a new column as factor
	
	5. Appropriately labels the data set with descriptive variable names. Give the selected descriptive names to variable columns
	
	6. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject. Use pipeline command to create a new tidy dataset with command group_by and summarize_each in dplyr package
