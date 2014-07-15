##### Getting and Cleaning Data Course Project #####

This code book that describes the variables, the data, and any transformations or work that you performed to clean up the data.


    1. Merges the training and the test sets to create one data set.
    
        After setting the source directory for the files, read into tables the data located in
          - features.txt
          - activity_labels.txt
          - subject_train.txt
          - x_train.txt
          - y_train.txt
          - subject_test.txt
          - x_test.txt
          - y_test.txt

        Assign column names and merge to create one data set.


    2. Extracts only the measurements on the mean and standard deviation for each measurement. 
    
        Create a logcal vector that contains TRUE values for the ID, mean and stdev columns and FALSE values for the others.
        Subset this data to keep only the necessary columns.


    3. Uses descriptive activity names to name the activities in the data set.
    
        Merge data subset with the activityType table to cinlude the descriptive activity names.
        
    
    4. Appropriately labels the data set with descriptive variable names. 
    
        Use gsub function for pattern replacement to clean up the data labels.
    
    
    5. Creates a second, independent tidy data set with the average of each variable for each activity and each subject. 
    
        Per the project instructions, we need to produce only a data set with the average of each variable for each activity and subject.


The source data for this project can be found here: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 

