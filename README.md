This is a PowerShell script to send a notification email to users whose passwords are going to expire in 14 days or less. An email will be sent to the users within the expiration time frame daily until their passwords have been changed. Any passwords which have expired over 30 days are ignored. This can be adjusted via the main script file.

In order for this script to work properly the following three files need to be stored locally. The file paths are defined in the .ps1 file.

Credentials.Json

Email Body.html

O365-sendMail-V3.ps1

Using Windows Task Scheduler, schedule the ps1 file to run daily.

The script will pull 365 credentials for the sending email from the .json file, the body of the emails from the .html file, then send an email to any users who meet the criteria.

## Please check the script files carefully, there are sections which need to be manually adjusted based on your environment. These sections have been outlined. ##
