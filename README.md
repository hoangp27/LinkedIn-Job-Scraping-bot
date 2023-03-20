# LinkedIn-Job-Scraping-bot

In 2022, while looking for my first Data Analyst job after graduation, I have to painfully perform a daily mediocre task of scrolling through every single Data Analyst posting on LinkedIn, Glassdoor, Indeed, etc. It was  that moment that I stumbled upon the idea of creating a Web Scraping bot to do all the manual work.

## Procedure

The overall process should be something like this:

1. Using Selenium package, the bot would access this link: 
https://ca.linkedin.com/jobs/search?keywords=Data%20Analyst&location=Canada&locationId=&geoId=101174742&f_TPR=r86400&position=1&pageNum=0 
(this link shows all the Data Analyst postings in Canada on LinkedIn within the latest 24 hour (for those looking for other position you can use different links!)

2. The bot would loop through every single record, find relevant elements, and retrieve these data into table format.

3. The data will be written on to a google sheet file, which is live connected to Tableau Public dashboard that automatically update on any change of the data.

4. Finally, with Window Task Scheduler, the Python bot will automatically run daily (as a batch file) at a specific time. This will automate the whole process (almost).

##
