INTRODUCTION

The script  run_analysis.R performs the 5 steps described in the course project's definition.
   • First, all the similar data is merged using the  rbind()  function. 
   • Then, only those columns with the mean and standard deviation measures are taken from the whole dataset. After extracting these columns, xData subset based on the logical vector to keep only desired columns, mean() and std()
   • Used descriptive activity names to name the activities in the data set taken from activity_labels.txt 
   • Finally, we generate an independent tidy data set with the average of each variable for each activity and each subject 

VARIABLES
  • x_train ,  y_train ,  x_test ,  y_test ,  subject_train  and  subject_test  contain the data from the downloaded files.
  • x_data ,  y_data  and  subject_data  merge the previous datasets to further analysis.
  • names(xDataSet_mean_std) Extracts only the measurements on the mean and standard deviation for each measurement.

  • Same approach taken with the activity names through the  names(yDataSet)  variable.
  • singleDataSet <- cbind(xDataSet_mean_std, yDataSet, subjectDataSet) Merges and combines all data sets into single one.
  • Finally, Data2 contains the ordered, relevant averages.
