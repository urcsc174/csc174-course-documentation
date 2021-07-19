# Lab 4: Four Database Functions, part 2

*Due: Wednesday, July 21, 2021*

**The goal** of this lab is to add the other database functions: *update* and *delete* to your city website.

## Step 1: Update the Contact Us webpage

From Lab 3, when the user filled out the HTML form and submitted it, we dumped a plain-text message in front of the user.  We must fix that...

- Upon successful completion of the Contact Us form (or whatever you call it), the user should be re-directed to the Visitors webpage (or whatever you call it) to see the results of their data entry
  - 
  - Hint: in the **insert.php** file you can delete the entire HTML and the embedded PHP blocks (with the "if/else" statement) completely, and join all the PHP in the **insert.php** file into one PHP block.  
  - Then add this line to the PHP block, right above the closing `?>` to send the user to the other webpage...

```php
header("Location: ../_________.php");
```

...the blank (above) should reference your Visitors webpage (or whatever you call it)

## Step 2: Update the Visitors webpage

Assuming you completed **Lab 3** successfully and you are familiar with the in-class sample files [**intro-mysql4**] then you should be able to figure out the following...

- Update the HTML table in the "visitors" webpage (or whatever you call it) into include the "Functions" columns (Edit and Delete)
  - Hint: look at the code in the **read.php** file from the **intro-mysql4** folder
    - Note: don't mindlessly copy & paste code from the intro-mysql4 files.  You need to study it and then just use the parts that makes sense in this context (for instance, you don't need the "Add a new record" link - that wouldn't make sense)
  - BTW - when using the **intro-mysql4** code, notice that the variable name in the *while* loop is different! (**\$data** vs. **\$row**). Depending on how you edit your code you might end-up with a mismatch.  Just look out for that.  Use \$data *or* \$row - not both.  You have to be consistent.
  - Also note that the paths to the script files might need to be edited based on how you're arranging the files in your file system.  Hint: if you have your script files in a subdirectory named **scripts** (like you should) then...
    - To navigate from an HTML file TO a script you have to use `"scripts/_____php"` (or something like that)

Make sure the READ function of your database still works normally (even if the "Edit" and "Delete" functions don't work yet)

## Step 3: Add the Delete and Update Functions to the Visitors webpage

The exact code you need to edit to add the *delete* and *update* functions to your visitors webpage depends on a lot of custom factors based on your own website and how you're structuring your file system.  So instead of specific instructions, here are the requirements you need to fulfill (below).  If you need help or get stuck - just use the #help channel in Slack to get help.

- Using the files from the [**intro-mysql4**] demo files as a guide, add the *delete* function to the "Delete" links in the visitors table
  - Upon completing the delete function, the user should be brought right back to the visitors table
- Using the files from the [**intro-mysql4**] demo files as a guide, add the *update* function to the "Edit" links in the visitors table, and note...
  - It's okay to have the Update function use the *renderform* from the [**intro-mysql4**] files as-is.  You do not need to style the *renderform* - it just needs to work correctly.  We'll make it look better later.
  - Upon Submit or Cancel, the *renderform* should take the user back to the visitors page

## Step 4: Turn-in the Lab Assignment in Blackboard

To get credit for your work:

- In your localhost, using phpMyAdmin, **export** your Lab 3 database (again)
  - Be sure to click on "lab03" in the database list on the left first, *then* click the **Export** tab to make sure you export only the Lab 3 database (not *all* the databases in your localhost!)
  - Save your exported SQL script to a file named **export.sql** and add it to the root of your Lab 3 folder (along with the website)
- Create a new GitHub repository called **CSC 174  Lab 4**
- Sync your Lab 4 from your localhost to the new Lab 4 repo on GitHub
- In Blackboard, find the Lab 4 assignment and paste the URL of your repository in the “Write Submission” area and Submit it
