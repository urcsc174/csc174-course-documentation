# Prep for Lab 3

To prepare for Wednesday, July 14, you need to create the following on your localhost.

- In your file system on your computer, in your localhost document root, create a new folder named **lab03**

- In the lab03 folder, create a "plain vanilla" (CSS-less, simple) HTML Form to capture some user contact information that has something to do with the city website you built as part of Lab 1
	- This webpage with the HTML form won't actually be part of your city website yet; we'll stitch that together later; for now it just needs to be a plain HTML (not even PHP) webpage
	- You can refer back to the CSC 170 lab where we did something like this (probably lab #12 or thereabouts depending on when you took CSC 170)
	- The bare-minimum fields in your HTML form needs to have: at least three text fields, for example but not necessarily:
	     - First Name
	     - Last Name
	     - Email
	
	    ...and/or maybe some other simple text fields

	- Note: unlike what you did in CSC 170, your form does not need checkboxes nor radio buttons, nor a message field ...we just want to keep it simple for now so just set it up to capture simple text fields
	
- In your localhost installation of MySQL (using phpMyAdmin of course), create a database and associated user; call it **lab03**

- In the lab03 database, create a table named **contacts**
	- the number of columns you'll need is the number of fields you created in your HTML form, *plus one more* for the counter

- In the contacts table, setup an **id** field (or "counter" or whatever you want to call it) as Type: **INT(11)** and have it set as **PRIMARY KEY** and **AUTO_INCREMENT** ("A_I")

- Continue setting up the contacts table to capture all the fields you setup in your HTML form
	- for all your text fields, be sure to use Type: **varchar** and a size (number) that makes sense for each field

- Using the demo files from today's class (Monday, July 12) - the "intro-mysql2" files - copy the **config.php** file and the **insert.php** file to your lab03 folder

- Edit the files as needed to make them work with your HTML Form and MySQL database
	- NOTE: in the HTML form, set the FORM tag to `action="insert.php"`
	- In the **config.php** file, enter the database credentials to make them work with your new user and database in MySQL
	  - Hint: use your **testmysql.php** file to make sure you got the database credentials right!
	- In the **insert.php** file where we manually hardcoded variables on lines 8, 9, and 10, swap them out using this code (from CSC 170, Lab 13)...
	
	`$_______________ = Trim(stripslashes($_POST['_______________']));`
	...if you need help figuring out what to replace the blanks with, don't hesitate to ask in the #help channel in Slack
	
- Continue editing the **insert.php** file; edit the SQL statement in section "**2. Perform database query**" to make the SQL code work with what you built in the MySQL database by changing:

  - The table name
  - The field names in the table (be careful! case sensitive!)
  - The variable names you created in the lines above

In your localhost with MAMP or MAMP for Windows running, use your HTML form to send data to your database.  Hopefully you'll get the success message.  If not, figure it out.  If you hit a brick wall, use the #help channel in Slack.

To see the new data in the database, use phpMyAdmin or the professor's **dbtester.php** file in the **intro-mysql** folder.