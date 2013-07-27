### Extract search engine data from the Web and save it to a database ###

![Alt text](http://173.0.133.251/images/GitHub/Sync-Deployment-fulla.jpg "Integrate with SQL and Major Databases")




### BUSINESS RISK ###

Keeping two or more separate databases up to date with each other's data changes can be a daunting topic. 

Whether your database solution is simple or complex, there are five key issues to consider:

<ol>
<li>How similar are the structures of the databases to be kept in synch? If they are identical, you are a step ahead in the game. As they become more dissimilar, syncing becomes more difficult and more abstract.</li>
<li>How often do the databases need to be synced?</li>
<li>How will you resolve situations in which the same data has been modified in both (or more) of your databases since the last sync session? There are a number of approaches from fairly simple to quite complex.</li>
<li>How much effort and/or money are you willing to invest in developing your sync system?</li>
<li>How much effort are you willing to put up with at each sync session?</li>
</ol>


### INTEGRATION APPROACH ###

Our approach to the integration of databases uses the least effort and money i.e. merge replication.

![Alt text](http://173.0.133.251/images/GitHub/approach.gif "Integration Approach")


### DATABASE CONVERSION / SYNCING POSSIBILITY MATRIX ###

![Alt text](http://173.0.133.251/images/GitHub/synch2a.gif "Integrate with Databases")

The table below shows the different types of databases and the possible type of integration:



The full suite of conversion and sync tools can be found here: http://www.dbconvert.com/order.php




### TESTING APPROACH ###

This project includes an ACL script which leverages the new EXECUTE command in ACL Analytics v10 to conduct database conversion between MS SQL database (source) and Access database (destination). The scripts included in the project will:

1.  Run the DBConvert tool (downloadable trial from http://dbconvert.com/convert-access-to-mssql-sync.php) in the script "Integrate_SQL_and_Databases".  The sync progress is shown below:

![Alt text](http://173.0.133.251/images/GitHub/progress.gif "Synchronization Progress")

2.  The software's scheduled service will also perform the conversion at a regular interval.  (See www.dbconvert.com/scheduler-configuration-manual.php for more info.)


Modifications to the scripts may obviously be made to add your own different databases' login credentials, software name and path, etc. The scripts simply illustrate an example of how to conduct a conversion between MS SQL database (source) and Access database (destination).  (For more info, see http://dbconvert.com/faq.php)


### THIRD-PARTY REQUIREMENTS ###

The ACL scripts below rely on external database converters and synchronizers called DBConvert tools (http://www.dbconvert.com).  To run DBConvert tools, your computer must have DBConvert installed. The easiest way to install DBConvert tools on a Windows computer is to download the software from http://www.dbconvert.com.


To learn more about DBConvert, take the video tour:

[![IMAGE ALT TEXT HERE](http://173.0.133.251/images/GitHub/video-img.jpg)](http://www.youtube.com/v/N_tAwAROclE?version=3&hl=ru_RU&rel=0)

[![IMAGE ALT TEXT HERE](http://173.0.133.251/images/GitHub/3rd-party.gif)](http://www.dbconvert.com/order.php)


#### Methodology ####

![Alt text](http://173.0.133.251/images/GitHub/use-methodology.gif "How I Work")

