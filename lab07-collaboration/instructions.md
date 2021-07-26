# Lab 7: Website Collaboration

*Due: Wednesday, July 28, 2021*

**The goal** of this lab is to build three websites collaboratively.

**The purpose** of this lab is to learn how to work as a team in the roles of IA, Designer, and Technician and understand how it's possible to build websites faster (and eventually easier) than working alone using  common industry tools:

- **Localhost** - to work independently
- **GitHub** - to sync your independent work with the rest of the team
- **Slack** - to communicate with each other remotely and asynchronously

## Development Process

*Given the unique nature of this summer's class, your team is already established: Miranda; Kyler; Matthew. Also, instead of everyone picking an initial role for themselves, everyone will perform **every** role in a "round robin" fashion.*

### Technician Role

- Following the process outlined in the lecture video about the *Development Process*, everyone needs to perform the role of Technician and **setup a repository** with a readme.md file, and then add the other team members as GitHub "collaborators"
  - Name the repository you create: **Lab 7 - *firstname*** (using your first name)
  - Note: the GitHub usernames of your teammates can be found in our #chatter channel in Slack
  - NOTE: this step needs to be completed by end-of-day TODAY, Monday, July 26

### Information Architect Role

- Then, everyone needs to perform the role of **Information Architect** in someone else's repository as follows:

  - **Miranda**, setup the HTML content in **Kyler**'s repo
  - **Kyler**, setup the HTML content in **Matthew**'s repo
  - **Matthew**, setup the HTML content in **Miranda**'s repo

  - Requirements:
    - Using the city content from Lab 6 ([csc174.org/lab06](https://csc174.org/lab06/)), create THREE HTML documents, each representing one city and consolidate all city content into them (each city will be a single, long webpage)
    - Add a new index file (index.html) to act as a front page for the three HTML documents (make it very CSC 170-like with headings, short intro paragraphs, and links)
    - Create a simple navigation element (unstyled, unordered list) in each HTML file to allow the user to go from page to page

  - HINT: keep it simple; do not work with PHP includes at this point
  - NOTE: this step needs to be completed by end-of-day on Tuesday, July 27

### Visual Designer Role

- Then, everyone needs to perform the role of **Visual Designer** in someone else's repository as follows:
  - **Miranda**, style the content in **Matthew**'s repo 
  - **Kyler**, style the content in **Miranda**'s repo
  - **Matthew**, style the content in **Kyler**'s repo
  - NOTE: this step will take some time and effort
    - You need to create a single set of CSS styles that works for ALL the city webpages, plus the new index page
    - You can start with any existing set of CSS - your own (from Lab 6) or someone else's, or start from scratch
    - You can manipulate the HTML as needed to make your CSS work
  - Requirements:
    - All four webpages must look like they belong to a single, unified website from a design stand point
    - The navigation element must be identically styled and positioned on all four webpages
  - NOTE: this step needs to be completed by end-of-day on Wednesday, July 28

### Technician Role, again

- Finally, everyone needs to work on their own repository again in the role of Technician

  - Clean-up the HTML and CSS - make sure everything passes validation (with reason)
  - Impose a CSS Architecture (a methodology), if it wasn't there already
  - Factor-out redundant code (within reason) into PHP Includes and install a menu highlighter solution as needed

- Install the website on the class web server

  Note: each team will use the same FTP account. Be careful *not* to disturb other teams' files.

```
FTP Server (a.k.a. Hostname): ftp.csc174.org
FTP Port: 21
FTP Username: lab07@csc174.org
FTP Password: [same]
```

## Submit the Assignment

To get credit for your work, submit a link to your website in Blackboard, in the assignment: **Lab 7: Website Collaboration**
