Reproducible Research: Peer Assessment 1

Loading and preprocessing the data

1. Load the data (i.e. read.csv())

if(!file.exists('activity.csv')){
  unzip('activity.zip')
}
activityData <- read.csv('activity.csv')
2. Process/transform the data (if necessary) into a format suitable for your analysis

#activityData$interval <- strptime(gsub("([0-9]{1,2})([0-9]{2})", "\\1:\\2", activityData$interval), format='%H:%M')