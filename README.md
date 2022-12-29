# How To Use Time Tracker

1.. Download the folder and save it to local with unzipped

2.. Open the dist/time_tracker

3.. The app will start executing

4.. Firstly you need to sign in with google. And then you are redirected to main timer window.

5.. Now to start the timer. Click on the Start button beside the Work-Development.

6.. After clicking on the start the Time tracking will be started.

7.. You can find log files into folder named time_tracker_2.0 
          LOG : /home/time_tracker_2.0
	
8.. Under the log folder you may find the 4 kind of log 
	- minute_drill_down : Every Minute activity
	- 10minutes_reporting.log : Every 10 min history and also reports by EOD about total work 
	- hourly_reports.log : Every Hour activity (Stores Working and idle Minutes)
	- daily_reports.log : Working time and Idle time For the Day
	- session_reports.log : logs when user is login & logout
	- error_logs.log : Logs When Error comes in Tracking user activity


# DATABASE STURCTURE

1..users
	- Users Information
	- Columns (ID, NAME, EMAIL, KEY)
	- Primary Key ID

2..10_minutes_report
	- To track user's work after every 10 minutes and when timer is stopped
	- Columns (ID, USERID, CREATED_AT, 10Minutes_STARTED_AT, 10Minutes_ENDED_AT, TIMER_TOTAL_TIME, WORK_TIME, IDLE_TIME)
	- Primary Key ID

3..Session_report
	- Log Out Report
	- Columns (ID, USERID, CREATED_AT, LOGIN_AT, LOGOUT_AT, TOTAL_TIME, WORK_TIME, IDLE_TIME)
	- Primary Key ID and Foreign Key UserID

4..Daily_Report
	- when time is stopped it will update work time and idle time of users
	- Columns (ID, USERID, CREATED_AT, WORK_STARTED_AT, WORK_STOPPED_AT, TOTAL_TIME, WORK_TIME, IDLE_TIME)
	- Primary Key ID and Foreign Key UserID

5..Hourly_Report 
	- To track user's work after every hour and when timer is stopped
	- Columns (ID, USERID, CREATED_AT, HOUR_STARTED_AT, HOUR_ENDED_AT, TOTAL_TIME, WORK_TIME, IDLE_TIME)
	- Primary Key ID
