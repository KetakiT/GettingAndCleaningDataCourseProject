
# Cleaning the data

* Files with same number of columns are merged using rbind() which result into x_data, y_data and subject_data.
* Only columns with mean and standard deviation measures are taken.
* Correct column names are extracted from features.txt.
* Activity data is addressed with values 1:6
* Activity names and IDs are taken from activity_labels.txt
* Average measures for each activity and each subject is computed using ddply and colMeans function - 30 subjects * 6 activities = 180 rows

# Variables

* x_train, y_train, x_test, y_test, subject_train and subject_test - get training and test sets from files
* x_data, y_data and subject_data - merged x, y and subject data from above data sets
* features - correct column names for x_data
* mean_and_std_features - numeric vector extracting only columns with std and mean in their names
* activities - correct column names for y_data
* all_data - merged x_data, y_data and subject_data
* average_data - relevant averages for each variable for each activity and each subject
