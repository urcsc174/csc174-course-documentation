# Lab 5: Remote Web Application

*Due: Wednesday, July 21, 2020*

**The goal** of this lab is to take the database application you created on your localhost in Lab 4, and reconfigure it so it uses a remote database (on the class web server); and also create a version of Lab 4 (called "Lab 5") that runs on the class web server.

## Part 1: Localhost Files and Remote Database

### Step 1: Export Your Database Table

- In phpMyAdmin, **export** your table (not the database) from your local phpMyAdmin to an SQL file by first clicking on your database table ("contacts") and then using the Export function

*On your localhost, you created a database that had only one table in it: your "contacts."  When you move your data to the class web server, we'll all be using the same database therefore we all need to have uniquely named tables. So...*

- Open the exported SQL file (from the step above) and **search and replace** all instances of `contacts` with a prefix that uses your first initial and last name like this: `rkostin_contacts`

Save and close the file and put it aside. You'll need it soon.

### Step 2: Login to Bluehost

*Be careful when you're logged-in to our Bluehost account.  We all share this account.  Don't screw it up please!*

- Go to [www.bluehost.com](https://www.bluehost.com)

- Login with domain: **csc174.org**<br>And password: **[see the #announcements channel in Slack]**
  - NOTE: please try and get the login right.  If you screw it up multiple times in a row, we will <u>all</u> get locked out!

- Once logged-in, click **Advanced** in the side-menu

Then put this web browser tab with your connection to Bluehost aside.  You'll need it later.

### Step 3a: Test Your Connection to the Remote Database

- Open your file: **testmysql.php** file in your localhost and change the login information to these new login settings.  
  - Host: **50.87.233.27**
  - Database user: **urcscon3_lab05**
  - Database password*: `**********`
  - Database name: **urcscon3_lab05**

\* *Replace the `**********` above with the password listed in the #announcements channel in Slack.*

- Save the file and then open it in a web browser (using localhost).
  - Maybe you'll get the "Connection OK" message in the viewport because your IP number is already registered with Bluehost; if so, skip to Step 4
  - Or, if after a long wait you get the "Connect Error (1045)" message, do the following step to setup remote access...

### Step 3b: Setup Remote Access to the Remote Database

You can skip this step if you got the "Connection OK" message in the previous step.  Else do the following.

- Figure out the IP number of your current computer connection to the Internet
  - You can simply Google for it like this: [https://www.google.com/search?q=my+ip](https://www.google.com/search?q=my+ip) 
  - Copy your public IP address
- Go back to the web browser tab open to Bluehost and the "Advanced" area
- Scroll down to click the **Remote MySQL** chicklet
- Under *Add Access Host* paste your IP number in the "Host" field
- In the Comment field, add your name and maybe some other identifier information
  - Keep in mind, your host address is different every time you connect your computer at a new location, so maybe you want to add your current location to the Comments field
  - BTW - if you move around a lot, like go to multiple coffee shops, you can register multiple IP numbers using this system
- Click the **Add Host** button
- Go back to your web browser pointed at **testmysql.php** and refresh it;  you should get the "Connection OK" message in the viewport
- In the web browser tab pointed to Bluehost, click **cpanel** in the submenu to go back to the Advanced page with all the "chicklets"

### Step 4. Import Your Lab 4 Database Table to the Remote Server

1. In Bluehost, in the Advanced area, scroll down to click the **phpMyAdmin** chicklet (or you'll probably find a link to it along the left-side, under "frequently used features")
2. In the left-side bar, click the name of our Lab 5 database, **urcscon3_lab05**
3. Click the **Import** tab in the top area
4. Click the **Choose File** button and select your edited SQL file from Step 1.
5. Scroll down and click the **Go** button

Hopefully, you'll see a long list of green messages.  If so, proceed to the next step.

### Step 5: Use the Remote Database with your Local Web Application

- On your computer, in your file system, copy your entire Lab 4 folder to a new folder named **lab05** (or whatever you're naming your lab folders)

- In your Lab 5 files, open the following PHP files in your code editor
  - **visitors.php** (or whatever you called your webpage that displays the HTML Table)
  - **update.php**
  - **insert.php**
  - **delete.php**


- In those four open files (above) search for every instance of "**contacts**" in those PHP files and replace them with the new table name based on your first initial and last name, example "**rkostin_contacts**"
- Save and close those files

- Edit the **config.php** file and change the database connection variables to the same information used in step 3a, above; save and close the config.php file

- Test the Lab 5 Application in your localhost
  - Make some additions, edits, deletions ...whatever
  - In the phpMyAdmin that's on the Bluehost web server (*not* your localhost) "browse" your table on the remote server; you should see your additions, edits, and deletions there
  - Notice that your Lab 4 files are no longer editing your localhost database

## Part 2: Remote Files and Remote Database

For this part you need to FTP your Lab 5 Application to the class web server and make sure it continues to work.

- IMPORTANT: back a backup copy of your **config.php** file.  Rename the copy something like **config.bak**
- Edit the **config.php** file (not the backup). Change the `$server` information from `50.87.233.27` back to `localhost`
- Open your FTP software and login using the following web server credentials, below.<br>*Note: everyone will use the same FTP account. Be careful not to disturb anyone elses' files.*

```
FTP Server (a.k.a. Hostname): ftp.csc174.org
FTP Port: 21
FTP Username: lab05@csc174.org
FTP Password: [see the #announcements channel in Slack for the password]
```

- When you FTP-in to the account, create a folder using your first inital and last name (e.g. **rkostin** place your Lab 4 application files in there

Test the remote version of your remote application on the class web server: 

`csc174.org/lab05/flastname/`<br>...where *flastname* is the folder name you just created in the step above

## Turn It In

- When the remote application and database is working, login to our CSC 174 area in Blackboard and go into the "Labs Assignments Turn-in" area
  - Find the assignment: **Lab 5: Remote Web Application**
  - Copy and paste the URL of your application into "Write Submission" 
  - Submit the assignment
