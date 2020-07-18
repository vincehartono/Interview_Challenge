# Interview_Challenge

## Part 1 (EDA)

I was given a task to clean up and do Exploratory Data Analysis from a file named logins.json. The file consists of login timestamp with 93,142 rows of data.

The login time ranges from January 1st, 1970 to April 13, 1970. I was stasked to group these login times by 15-minutes interval.

First step I did is to check if there is any missing values in the data and check the types of the input. There are no missing values and the input is in datetime64 data type.

Since it consists of 103 days and there are 96 15-minutes interval per day, it is hard to visualize the data to determine if there is any patterns thus I group it by 3 different groups.

### Group by Date
By grouping the data by date, a trend shows up every 7 bars thus there must be a trend by day of week. 

### Group by Day of Week
By grouping the data by day of week, I can see that weekend (Friday, Saturday, Sunday) have more logins compared to weekdays.

### Group by Hour
By grouping the data by hour, it seems another pattern emerges. I can see that there are more logins during the night starting at 20:00 until 5:00. There is also another high number of logins during noon (11:00 to 12:00)


## Part 2 (Experiment and Metrics Design)

I was given a task to design an experiement to track how efficient toll costs reimbursement in encouraging drivers from Gotham and Metropolis not to be exclusing in hailing passengers just in their respected city.

The key measures of success that I would like to track for this experiment are:
  1. 
