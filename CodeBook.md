# Tidy data set description

## The variables in the tidy data

x_train, y_train, x_test, y_test, sub_train,  sub_test, variables_names and activity_lables contain the data from the downloaded files.
x_total, y_total and sub_total merge the previous datasets to further analysis.
features contains the correct names for the x_total dataset, which are applied to the column names stored in mean_and_std_features, a numeric vector used to extract the desired data.
A similar approach is taken with activity names through the activity_lables variable.
total merges x_total, y_total and sub_total in a big dataset.
Finally, averages_data contains the relevant averages which will be later stored in a .txt file. ddply() from the plyr package is used to apply colMeans() and ease the development.

Tidy data contains 180 rows and 68 columns. Each row has averaged variables for each subject and each activity.

## Only all the variables estimated from mean and standard deviation in the tidy set were kept.

mean(): Mean value
std(): Standard deviation
The data were averaged based on subject and activity group.

## Subject column is numbered sequentially from 1 to 30. Activity column has 6 types as listed below.

	WALKING
	WALKING_UPSTAIRS
	WALKING_DOWNSTAIRS
	SITTING
	STANDING
	LAYING


## The tidy data contains 6 rows (averaged based on activity) and 68 columns (66 variables and activity labels).

	"activitylabel"
	"subject"
	"tBodyAcc-mean()-X"
	  "tBodyAcc-mean()-Y"
	  "tBodyAcc-mean()-Z"
	  "tBodyAcc-std()-X"
	  "tBodyAcc-std()-Y"
	  "tBodyAcc-std()-Z"
	  "tGravityAcc-mean()-X"
	  "tGravityAcc-mean()-Y"
	  "tGravityAcc-mean()-Z"
	  "tGravityAcc-std()-X"
	  "tGravityAcc-std()-Y"
	  "tGravityAcc-std()-Z"
	  "tBodyAccJerk-mean()-X"
	  "tBodyAccJerk-mean()-Y"
	  "tBodyAccJerk-mean()-Z"
	  "tBodyAccJerk-std()-X"
	  "tBodyAccJerk-std()-Y"
	  "tBodyAccJerk-std()-Z"
	  "tBodyGyro-mean()-X"
	  "tBodyGyro-mean()-Y"
	  "tBodyGyro-mean()-Z"
	  "tBodyGyro-std()-X"
	  "tBodyGyro-std()-Y"
	  "tBodyGyro-std()-Z"
	  "tBodyGyroJerk-mean()-X"
	  "tBodyGyroJerk-mean()-Y"
	  "tBodyGyroJerk-mean()-Z"
	  "tBodyGyroJerk-std()-X"
	  "tBodyGyroJerk-std()-Y"
	  "tBodyGyroJerk-std()-Z"
	  "tBodyAccMag-mean()"
	  "tBodyAccMag-std()"
	  "tGravityAccMag-mean()"
	  "tGravityAccMag-std()"
	  "tBodyAccJerkMag-mean()"
	  "tBodyAccJerkMag-std()"
	  "tBodyGyroMag-mean()"
	  "tBodyGyroMag-std()"
	  "tBodyGyroJerkMag-mean()"
	  "tBodyGyroJerkMag-std()"
	  "fBodyAcc-mean()-X"
	  "fBodyAcc-mean()-Y"
	  "fBodyAcc-mean()-Z"
	  "fBodyAcc-std()-X"
	  "fBodyAcc-std()-Y"
	  "fBodyAcc-std()-Z"
	  "fBodyAccJerk-mean()-X"
	  "fBodyAccJerk-mean()-Y"
	  "fBodyAccJerk-mean()-Z"
	  "fBodyAccJerk-std()-X"
	  "fBodyAccJerk-std()-Y"
	  "fBodyAccJerk-std()-Z"
	  "fBodyGyro-mean()-X"
	  "fBodyGyro-mean()-Y"
	  "fBodyGyro-mean()-Z"
	  "fBodyGyro-std()-X"
	  "fBodyGyro-std()-Y"
	  "fBodyGyro-std()-Z"
	  "fBodyAccMag-mean()"
	  "fBodyAccMag-std()"
	  "fBodyBodyAccJerkMag-mean()"
	  "fBodyBodyAccJerkMag-std()"
	  "fBodyBodyGyroMag-mean()"
	  "fBodyBodyGyroMag-std()"
	  "fBodyBodyGyroJerkMag-mean()"
	  "fBodyBodyGyroJerkMag-std()"


## variable units

Activity variable is factor type. Subject variable is integer type. All the other variables are numeric type.