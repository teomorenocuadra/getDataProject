## Tidyng up Activity Data

### Project Scope and Deliverables

The purpose of this project is to demonstrate ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis. You will be required to submit:

Tidy data set as described below.
Link to a Github repository with your script for performing the analysis called run_analysis.R.
Code book that describes the variables, the data, and any transformations or work that you performed to clean up the data called CodeBook.md.
README.md in the repo with your scripts. This repo explains how all of the scripts work and how they are connected.

One of the most exciting areas in all of data science right now is wearable computing - see for example this article. Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users. The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained:

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

Here are the data for the project:

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

You should create one R script called run_analysis.R that does the following: 01 Merges the training and the test sets to create one data set. 02 Extracts only the measurements on the mean and standard deviation for each measurement. 03 Uses descriptive activity names to name the activities in the data set. 04 Appropriately labels the data set with descriptive variable names. 05 From the data set in step 04, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

### The Tidying Data Script

#### Step 00: Getting & Reading Raw Data

Downloads the source data pack. Unzips the source data pack. Reads the relevant data from the pack.

#### Step 01: Merging the Training and the Test Sets to Create One Data Set

Adds column names to activity training and test data sets. Adds column names to participant (Subject) training and test data sets. Adds column names to measurement variables on training and test data sets using labels from the features data set. Merges Activity, ParticipantNumber (Subject) and Measurements for training and test data sets. Merges the training and test datasets to create one.

#### Step 02: Extracting Only the Measurements on the Mean and Standard Deviation for Each Measurement

Names the columns of the features data set. Extracts measurements that include the mean and the standard deviation. Creates a subsetting vector. Subsets the data set.

#### Step 03: Using Descriptive Activity Names to Name the Activities in the Data Set

Replaces the 6 activity code numbers with descriptive names. 

#### Step 04: Appropriately Labelling the Data Set with Descriptive Variable Names

Replaces abbreviations with full words for the quantitative variables names.

#### Step 05: Creating an Independent Tidy Data Set with the Average of Each Variable by Activity and Subject

Summarizes the data set. Calculates variable averages by Activity and ParticipantNumber (Subject). Sorts the tidy data set by Activity and ParticipantNumber (Subject). Saves the tidy data set into a text file Tidy.txt.


