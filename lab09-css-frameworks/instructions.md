# Lab 9: CSS Frameworks

*Due: Monday, August 2, 2021*

**The goal** of this lab is to take your Lab 5 files and style them using an off-the-shelf CSS Framework, and then customizing the framework so it looks unique.

**The purpose** of this lab is to learn the process for using a CSS Framework so you don't have to write all your styles from the ground up, every time you start a new project.  Also: to learn how to customize the styles from a framework in the most efficient way that "future protects" the web site from versions of the framework that will come later.

## Step 0: Select a CSS Framework

-  Read the article: [10 Best CSS Frameworks for Front-End Developers (Thankur, May 15, 2020)](https://geekflare.com/best-css-frameworks/)
  - Pay close attention to the pros and cons of each; if you're new to this topic, look for ones that are easy to learn
- Make a selection; pick a CSS Framework and go to its website to learn how to apply it to a website
  - If they provide demo files, download and play with them to get a feel of how they work in a "plain vanilla" environment

## Step 1: Copy and Prepare the Files

*Note: with the city "visitors" application (or whatever you called it), there are only THREE files that actually put content in the viewport of the user's web browser.  It's on those files only, you will apply a CSS Framework.*

- Copy all your Lab 5 files to a new folder; call it **lab09**
- Open the following files (only) for editing:
  - **the visitors HTML form** ...the one for users to fill out ("Sign Our Guest Book" ...?)
  - **the visitors HTML table** ...the one that lists who filled out the HTML form ("Guest Book" ...?)
  - **the "renderform"** ...the un-styled HTML form used by the *update* script when the user clicks the *Edit* link

## Step 2: Install and use a CSS Framework

*The actual steps to install a CSS Framework depend on the framework you've chosen.  The hard part of this lab assignment - and the hard part about using frameworks generally - is learning how to use it!  So if this part takes you a while, that's normal.*

- After you've picked a CSS Framework and learned how to install and use it (from Step 0), apply what you've learned to the city visitors application.  Focus on just simple formatting and basic layout.

All CSS frameworks will direct you to link to their CSS.  

- Also for this lab assignment, you can add and move elements around.  Because a lot of CSS Frameworks have some simple content in their examples, feel free to flex off those examples and add things to the phonebook application as you see fit.  Remember: the focus on this lab assignment is to try out and *play* with a CSS Framework to get experience.

Note: this could take a lot of time; just try to cut through it quickly and learn as you go.

- Suggestion: look for tutorials; create a "plain vanilla" test webpage first; then apply the parts that make sense to your Lab 9

## Step 3: Customize the Framework

You need to make *some* customizations to the CSS Framework you've installed so all CSC 174 Lab 9s look different from each other.  You can:

- Change colors
  - use a good pallet - don't randomly pick colors
- Apply appropriate background colors and/or images
  - make sure you don't reduce the readability and usability of the website
- Anything else, interesting or different that you can apply to differentiate your website and make it look unique
  - ...that includes maybe adding a little content so you can do something with it

### Implement an overide.css file

- In the file system, create a new CSS file named: **override.css** in lab 9
- In the HTML of your files, BELOW all the other CSS \<link> tag(s) for your framework, create a new \<link> to the **override.css** file

- Using your browser's **inspector tools** figure out what CSS classes you need to override to incorporate your *custom styles*
- Write those CSS properties in your **override.css** file as needed to complete your design

## Turn It In

When your Lab 9 files seem to be working/looking correct, install the lab on our class web server.

- Open your FTP software and login using the following web server credentials, below.<br>*Note: everyone will use the same FTP account. Be careful not to disturb anyone elses' files.*

```
FTP Server (a.k.a. Hostname): ftp.csc174.org
FTP Port: 21
FTP Username: lab09@csc174.org
FTP Password: [same]
```

- When you FTP-in to the account, create a folder using your first initial and last name (e.g. **rkostin** place your application files in there
- REMEMBER: on the class web server, change the server information in the **connect-db.php** file<br>from: `$server = '50.87.233.27';` <br>to `$server = 'localhost';`
  - ...because the relationship between the PHP files and the MySQL database on the class web server is "local" 
- And of course, go to our CSC 174 section in Blackboard and submit a link to your lab files in the lab assignment named: **Lab 9: CSS Frameworks**
