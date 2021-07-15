# Lab 3: Four Database Functions, part 1

*Due: Friday, July 16, 2021*

**The goal** of this lab is to add a database read and write functionality to your city website.

*Note: in Wednesday's class I mentioned that you'd need to apply **all four database functions** to your city website.  CHANGE IN PLANS: this lab assignment is now split into multiple parts.  For this part you'll add only two of the four functions (read and write ...or in "CRUD" terms: "<u>c</u>reate" and "<u>r</u>ead", but not "<u>u</u>pdate" nor "<u>d</u>elete" yet)*

## Step 1: Add a Visitors webpage

Assuming you completed the in-class activities from Wednesday, July 14, you should have a working HTML form (called *contact* or something like that) stitched-into the Lab 3 version of your city website, and that HTML form should be able to create records in your localhost database called "lab03"

- Create a new webpage in your Lab 3 website using the same structure and styles as the other pages, and stitch it into the navigation system; call the webpage "Visitors"
- On the Visitors webpage, display an HTML table that pulls data from the *contacts* table in your *lab03* database

- Instead of just unceremoniously dumping the *Contact Us* form and the *Visitors* table into two new webpages without explanation, you need to add some copy (headings and text) as you see fit to make the features on the new webpages *make sense* in the context of your website
  - If you need inspiration, look at similar functions on existing websites anywhere on the Web

## Step 2: Plan Styles and Layout for the new Webpages

Although we haven't covered page design principles yet (coming soon!) try your best to envision a "normal" looking look to the two new webpages: *Contact Us* and *Visitors* (or whatever you chose to call them)

- Create a set of **wireframe diagrams** - just line sketches with boxes - that shows the layout of your existing styles and layout from Lab 3 and how you plan to layout the elements in the two new webpages
  - Don't belabor this exercise - you can simply use paper and pencil ...whatever, just to capture your ideas
  - Look at existing websites with similar elements for inspiration
- FOR CREDIT: share your wireframe diagrams in our #chatter channel in slack
  - If sharing hardcopy drawings, you'll need to take a picture and upload the image; make sure the image is clear and legible
  - Include text with the drawing typed into your post(s) in Slack to describe anything important if you think that'll help communicate your ideas
  - Also include a direct link to your Lab 1 website online (under: [csc174.org/lab01/](http://csc174.org/lab01/))

## Step 3: Style the New Webpages

- Using your own diagrams as a guide, create the styles and layout for the two new webpages in your Lab 3 website on your localhost

Note: you won't be able to publish your Lab 3 website on the class website until we cover how to do that.  It'll involve some new techniques having to do with replicating your localhost database on our Bluehost web server.  Until then you'll turn-in your updated Lab 3 website using the following procedure...

## Step 4: Turn-in the Lab Assignment in Blackboard

To get credit for your work:

- In your localhost, using phpMyAdmin, **export** your Lab 3 database
  - Be sure to click on "lab03" in the database list on the left first, *then* click the **Export** tab to make sure you export only the Lab 3 database (not *all* the databases in your localhost!)
  - Save your exported SQL script to a file named **export.sql** and add it to the root of your Lab 3 folder (along with the website)
- Create a new GitHub repository called **CSC 174  Lab 3**
- Sync your Lab 3 from your localhost to the new Lab 3 repo on GitHub
- In Blackboard, find the Lab 3 assignment and paste the URL of your repository in the “Write Submission” area and Submit it
