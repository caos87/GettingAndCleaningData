# How it works
1. Using rbind() function, we merge the data from corresponding "train" and "test" files (with the same number of columns) from the orginal data set.
2. We extract the columns with names "std()" and "mean()" in the column names. Then we put them together into one single data set named "x_data" and correct the column names.
3. Correct column names according to "activity_lable.txt"
4. Rename the entire data set, some of whose column names are too abstract.
5. Create a new dataset including averages of each subject and activity and name it "average_data.txt"

# Variables
1. x_train, y_train, x_test, y_test, subject_train and subject_test contain data from the corresponding datasets from the original files
2. x_data, y_data and subject_data merge the (subsets of) original datasets
3. features contains the correct names for the x_data dataset, which are applied to the column names stored in mean_and_std_features. Activities variables are handled the same way.
4. all_data merges x_data, y_data and subject_data.
5. "average_data.txt" contains the means asked for by the project.
