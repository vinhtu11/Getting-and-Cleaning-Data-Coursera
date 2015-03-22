# Getting-and-Cleaning-Data-Coursera
## Course Project

# Description of run_analysis.R
This script use to:
- Merges the training and the test sets to create one data set.
- Extracts only the measurements on the mean and standard deviation for each measurement.
- Uses descriptive activity names to name the activities in the data set
- Appropriately labels the data set with descriptive activity names.
- Creates a second, independent tidy data set with the average of each variable for each activity and each subject.


# Step by step for this code:
1. Install two libraries "data.table" and "reshape2"
2. Read supporting metadata and loaded into variables named "features" and "activity_labels"
3. Extracts only the measurements on the mean and standard deviation for each measurement. Put it in "extract_features"
4. Load data from test folder (X_test.txt, y_test.txt, subject_test.txt)
5. Make object "test_data" use cbind command
6. Load data from train folder (X_train.txt, y_train.txt, subject_train.txt)
7. Extract only the measurements on the mean and standard deviation for each measurement. Put it in "X_train"
8. Make object "train_data" use cbind command
9. Merge "test_data" and "train_data"
10. Apply mean function to dataset using dcast function and create "tidy_data.txt"
