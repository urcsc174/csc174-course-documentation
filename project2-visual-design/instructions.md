# Project 2: Visual Design

Due: <s>Monday, August 9, 2021</s> *...extended!*

**The goal** of this project is to build a new website built on an Information Architecture created in Project 1.

**The purpose** of this project is to work in a team and demonstrate your understanding of the concepts and technologies we've covered in CSC 174 so far.

## Requirements

As a team you need to:

- Pick an **Information Architecture** created by one of the members of your team, and...
- Flesh-out the content for three cities based on the IA chosen, heavily editing and/or gathering new content as needed
- While the content is being prepared, based on the *mood & feel* of the content **make design choices** that can be explained in terms of the C.R.A.P. principles and good application of typography to make the content usable and readable
  - Note: at least one but no more than three **custom fonts** (from any source, e.g. Google Fonts) must be installed and used on the website
  - All fonts (including non-custom) must be paired well and make sense according to the information architecture
- Also, apply page **layouts** using a Z-pattern (on the homepage) and an F-pattern (on all the subpages), and...
- Implement a new **HTML form** to capture user input that is stored in a new backend database (the form can be based on the design from a previous lab assignment, or completely new), and...
- On a separate webpage from the HTML form, have an **HTML table that displays all the records** from the backend database, and gives the user the ability to edit or delete records
  - The Edit ability can continue to use the separate "renderform" function on a separate webpage for now, but the presentation of the renderform must be styled in a way that looks like it belongs to the same website
- Also, use a **CSS Architecture** (any) to organize the custom CSS
- Also, use a **CSS Framework** (any) to apply basic styles to the website instead of writing them from scratch, and then *customize* the framework styles by using your own separate styles.css and as necessary, an "override.css" file.
- Also in a **readme.md** file, document AND EXPLAIN the rationale for every aspect of the website from the point of view of each role:
  - **Information Architect:** provide the ontology, and taxonomy, and explain the choreography (why things are in the order they are); also cite the source of any copied content
  - **Visual Designer:** explain all design choices - colors, positioning, fonts, etc.
  - **Technician:** provide technical information about the **structure of the data table** on the server (data types and lengths), and the type of **CSS Architecture** implemented, and the **CSS Framework** used; also explain any **PHP Include** choices and any other interesting implementations (your discretion ...anything you're particularly proud of?)
- A **GitHub repository** must exist with all the team members contributing meaningful commits, and plenty of them
- The website needs to be **installed on the class web server**, and operate as expected including but not limited to:
  - HTML and CSS **validation** (within reason)
  - No existence of a file: **error_log** on the web server
  - No files on the web server that are not actually part of the website (common mistake: the **readme.md** file should *not* be on the web server!  Leave that in the repo only!)

## Notes

- There is a new database on the class web server; here are the credentials
  - Test this in your **testmysql.php** file

```
host: 50.87.233.27
username: urcscon3_project02
password: [same]
database: urcscon3_project02
```

- You will need to login to our Bluehost hosting account and find the production version of *phpMyAdmin* (in the "Advanced" area)
- There, in *phpMyAdmin* on the server you'll need to create a new table in the Project 2 database and setup the structure based on the data you need to capture from your HTML form
  - Be sure to include a "counter" or "id" field that uses AUTO_INCREMENT

```
Bluehost login: www.bluehost.com
Password: [same]
...then click "Advanced" in the left column and select "phpMyAdmin"
```

## Suggestion Process

Your team is already established: Miranda; Kyler; Matthew

1. One of you (doesn't matter who), **create a PRIVATE channel in our Slack Workspace** and then invite the other members.  (Do not invite the professor.  This will be your private area to communicate.  The professor will have no visibility into your private channel.)
2. DECIDE: who will assume which role
   - **Information Architect** - to setup, gather, and arrange the content
   - **Visual Designer** - to apply styles to the content
   - **Technician** - to implement the MySQL database and PHP scripts; and to ensure everything works and is coded correctly

Then follow the high-level guidelines from [Lecture 9b. Website Collaboration](https://rochester.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=cb5b7ebc-795d-4b8c-ae93-ad710109851a).

### Other notes and suggestions

The best teams know what's expected of each member, and is able to "stay in their own lane" and let the other members do their job.  Some confusion comes from the following activities.  Although really, your team can do whatever you want, here are some suggestions:

- Everyone needs to constantly watch the private channel in Slack; so you can ask each other questions and stay coordinated for the duration of the project

#### Technician-specific suggestions

- The Technician needs to setup the repo and add the other members as quickly as possible (today would be good!), and then everyone must sync with the repo and be comfortable creating commits and pushing/pulling updates often
- Although the Visual Designer will keep in mind that the CSS needs to be organized, it's the Technician that is responsible (and will be graded on) implementation of a **CSS Architecture**
- Although the Visual Designer will chose a **CSS Framework** to use, it is the Technician that will install it (and be graded on its correct installation); then the Visual Designer can use it as they see fit
- Note: the Technician is dependent on the Information Architect to decide what the HTML form will capture; be sure to get direction from the IA before creating the database table
- If/when the Technician needs to rename files and/or move files and folders around in the repository, follow this procedure:
  1. Send a Slack message to the team telling them to Commit and PUSH your changes to the repo now and then STOP working for a few minutes
  2. When you get confirmation from the team that they've pushed their changes and they've stopped working (or you're sure they're not working now), then...
  3. PULL to make sure you've got everyone's latest changes
  4. Go ahead and move/rename files and folders in your localhost (e.g. create PHP Includes)
  5. Commit and PUSH your changes to the repository
  6. Send another Slack message to the team telling them to PULL the latest changes from the repository (and notice that the files and folders may have changed)

#### Information Architect-specific suggestions

- As soon as the repo is setup, the IA needs to create the "shells" with dummy content as quickly as possible so the other team members have something to work with; do not try to get all the content together before pushing the HTML initially (that won't leave enough time for the team to do their work)
- As soon as practical, be sure to communicate to the team the following:
  - The *mood & feel* of the website --> Visual Designer so they can make color choices, font choices, etc.
  - The specific content of the HTML Form --> Technician so they can setup the table in the database
- NOTE: the IA is only responsible for the content and the HTML tags in all the web pages
  - NOT anything in the HEAD tag of each HTML document except the TITLE tag
  - NOT setting-up PHP Includes
  - NOT even the validation of the HTML
  - But DO make sure you use good, semantically-correct HTML tags (especially H1, H2, etc.) and HTML structure (SECTION, ARTICLE, ASIDE, etc.)

#### Visual Designer-specific suggestions

Note: there is a lot of focus on the Visual Designer for Project 2, but that is not the only thing being graded.  The other team members have an equal stake in Project 2 as well.

- Be sure to get direction from the Information Architect about the *mood & feel* of the website; you'll be graded on the choices you make and how well your choices support the direction
- In the readme.md file, be sure to explain the reasoning behind your design choices (more so than the other team members, you'll be graded on that)

And don't forget, CSS is hard! But the professor is really good at it!  Don't hesitate to ask for help in the #help channel in Slack.  (Often, he'll just give you specific code to try if you just ask!)

## Submission Requirements

This part must be done by the Technician

- Install the website on the class web server


```
FTP Server (a.k.a. Hostname): ftp.csc174.org
FTP Port: 21
FTP Username: project02@csc174.org
FTP Password: [same]
```

NOTE: because there are no other teams/project in CSC 174, just install the website directly in the **project02** folder on the web server

REMEMBER: change the database credentials (in the config file) from the IP number to "localhost"

FINALLY: for the team to get credit for your work, submit a link to your website AND a link to the repositiory in Blackboard, in the assignment: **Project 2: Visual Design**

- NOTE: for Project 2 Blackboard is set so only one team member (the technician) needs to make the submission and that'll automatically count for every member of the team
