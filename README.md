# Getting-and-Cleaning-Data-Course-Project

  One of the most exciting areas in all of data science right now is wearable computing. Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users. 
  
 The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. 
 
 The experiments have been carried out with a group of **30 volunteers** within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data. 
 
 **The steps I took:**
 
 1- extract zip files
 
 2- Extracting only the measurements on the mean and standard deviation for each measurement.
 
*  with grep()  function and with the help of regular expressions and metacharacters

*  with gsub() I substitute the mean and std with Mean and Std
 
 3- with the help of cbind and rbind I created my final data frame
 
 4- with colnames() I label the data set with descriptive variable names.  
 
 5- with factor()I put  descriptive activity names to name the activities in the data set
 
 6- with melt() from reschape2 package and dcast i created a second independent tidy data set with the average of each variable for each activity and each subject.
 
 7- with write.table i created the tidy_data i submitted
