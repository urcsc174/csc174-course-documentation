# Project 2: Information Architecture

*Due: Friday, July 23, 2021*

**The goal** of this project is to re-structure the content of the Project 1 websites to meet the standards of good information architecture.

**The purpose** of this project is to demonstrate your understanding of IA, specifically: ontology, taxonomy, and choreography, as it applies to websites, while working in a team of Information Architects

## Establish a New City-Team

For this project, everyone will be an Information Architect in a new city-team, working on a "forked" copy of one of the Project 1 websites.

*Note: it is not unusual in very large organizations working on very large websites to have a team of IAs (or whatever they call them); there is usually one IA with the most experience who acts as the team lead; the rest are junior IAs - but in our case, your team just needs to try to work well together; none of you are "in charge" per se.*

- Go to [our shared Google Sheet](https://docs.google.com/spreadsheets/d/1z0z8gNCR0_-zW18ft0YDoiLPn6z4OTuAM5P8jVIa7cg/edit#gid=0)  and **copy** (do *not* move) your name/email from the **Project 1** city-teams to a *new* (different) city-team for **Project 2**
  - Note: *do not decide too fast*!  There is criteria below that you should know about before deciding where to move.

The requirements for this project will have you and your new teammates come-up with a new information architecture, and then FORCE the content into that new structure.  So it would behoove you to find new team members with content from Project 1 that compliments your content from Project 1.  Things to consider:

- Students that have similar content to yours will be easier to work with in a new, common architecture; look at section headings; lists; photos ...even the amount of words you used
- Students that have similar interests to you will be easier to create a new architecture around; consider your major, clubs, or your cultural identity ...anything you find interesting, whether or not you included it in your original Project 1 content

Then, establish contact with your new City-Team

- When you have a team, follow the same steps as before to create a *new* private channel in Slack and invite the other members

## "Fork" a Repository

For this next step it doesn't really matter who does what, however it would be helpful for someone who was *not* the technician last time to do it this time ...so more people can get more experience

- The team must use a new GitHub repository, based on a "forked" Project 1 repository
  - Your team must choose which repository to fork (copy); decide amongst yourselves which of you worked on a Project 1 website with the best design, in your opinion
  - Once you've decided which website to fork and who does what: in GitHub, in the repo you choose, you'll see the **Fork** button in the top-right; use it to start the process of setting-up a new repo
  - Whoever sets-up the new repository, make sure everyone in your team is added as contributor and can sync it to their localhost on their desktop using the GitHub desktop software

One or more of your team members will have a webpage in the new website you forked.  For the others...

- Delete the webpage(s) belonging to students who are *not* in your new team OR (if this is easier) delete the content but leave the structure of webpages from the students who are *not* in your new team
- Incorporate the new content/webpage(s) so everyone in the new team has a page in the new website
  - Don't forget to purge image files and anything else that no longer belongs in your new website
  - Update the navigation element accordingly
  - Make sure everything continues to validate and work normally

## Create a New Information Architecture

This is the hard part of this project: working with your team you need to decide on a new information architecture that you can achieve

### THE GOAL

The content in the new website must demonstrate your understanding of:

- Ontology
- Taxonomy
- Choreography

...by restructuring the content, by force, as necessary.

- The website must have all the features of the Project 1 website including: a homepage that acts like an index for the rest of the website; a working navigation element; and all the technical requirements such as use of PHP Includes, et cetera

### Suggested Workflow

Note: the process of developing an information architecture will feel like overkill for such a small website!  But remember that process uses the same steps you'd use on a major website project.

Also, this first step (ontology) doesn't really have much to do with websites!  It might be easier to work in a document - like a Google Doc or something like that - to do the IA work.

#### Ontology

1. Identify your classes and create your **triples**

   - Hint: you're all students; you all have majors; some of you have memberships in clubs; interests; et cetera ...make a list of these things; it won't be a long list

   - Don't forget the simple things such as: *your name*, *a photo of yourself* ...anything else?
   - Create your triples; most of these will be simple like:<br>Student has a name<br>Student has a photo<br>Student has a major<br>...stuff like that
   - Expand your triples to include the things you (as a team) decide to include like:<br>Student has work experiences<br>Student belongs to club(s)<br>Student has created portolio items<br>...BTW, you'll notice that just about all your triples will be centered around the "student", but that doesn't necessarily have to be so; try to think of other classes to act as the *Subject*-side of the triple

2. Gather and organize the data to instantiate the triples

   - How and where you organize the data is up to you based on the information you decided on; the key thing is to do it in a way that make it easy to view the actual content, from a high-level when you do the next step...

3. Inspect the content; look for inconsistencies - look for odd-ball content

   - Content belonging to the same triples should look like each other in every way including...
   - Photos should be consistent in terms of their shape (dimensions), and their content (headshots vs. action shots)
   - Paragraphs should have roughly the same density - meaning size; i.e. if one triple has a short description (say, 50 words) and another triple has a larger description (500 words in multiple paragraphs) ...you need to fix that
   - Same thing for lists; if you have them, they should roughly be the same length

Note: for this part (above) get used to the idea of chopping up content and sometimes throwing out good stuff that just doesn't fit; and yes - you'll probably need to gather new content to even-out the triples

#### Taxonomy

This next step *should be* relatively easy.  You just need to decide how to label everything.  And since we're building websites, that means:

- Creating a common **document structure**, from page to page
- Creating a common **document outline**, from page to page
- Using common labels (in our case, filling-in the **words in your heading tags**)

The goal here (and how you'll be graded), is by looking at all three student pages side-by-side.  The parts listed above must be identical on all three pages, especially the third one about words in the H-tags

Note: when filling-in the words in the heading tags, you have a choice: Use a common descriptor, e.g. "Work Experience" ...or whatever you chose, OR use the actual content from each triple, e.g. a student's name ...so long as it's perfectly consistent from page to page.

#### Choreography

This last step is often overlooked ...don't overlook it!  The order of things matters.  You need to decide.

And remember the LATCH framework.  Although you have very little content to work with, how should any of it be grouped?  Location; Alphabet; Time; Category; Hierarchy ...or any other logical method that makes sense for your content.

- On each student page, what comes first? (top, left) ...followed by what?  (further right and/or down)
- From page-to-page, you have to decide who goes first, second, last? ...and why?
  - Even if it's something lame like alphabetical by last name ...so be it.  Just don't forget to decide

#### Create a readme.md file

Your repository (NOT the website) needs to have a **readme.md** file. In it, include at the top:

- Your city-team's name
- Everyone's name

And then explain the following:

- **Classes and relationships** (not the actual triples ...I should be able to see them in the website)
- You don't have to say anything about **Taxonomy** - it's assumed I'll be able to see that simply by looking at the website; however, if there's something you're not sure I'll see or understand, do mention it in the readme
- Decisions about the **choreography**; not only why one page follows another, but within each page, why is the layout as it is?

BTW - remember, the readme.md file (and anything else that isn't part of the actual website) does *not* belong on the class web server!

Also note, there shouldn't be anything else in the **readme** file except what's listed above.  

- If your team wants to use a markdown file to create a to-do list or something like that, create a different file (like **todo.md** ...or something like that)
- BTW in GFM, this code will create a checkbox `- [ ] my to-do item` that you can update like this `- [x] my to-do item` ([see here](https://github.blog/2013-01-09-task-lists-in-gfm-issues-pulls-comments/))

#### Technical Installation

Although you're all IAs in this project, the roles of Visual Designer and Technician are still needed to some degree; it's assumed that you can come together as a team and divvy-up these last steps.

- It's assumed you'll all come together and update and insert your own content in the decided information architecture
- You can all pitch-in and update your own "well" on the home page
- If updates to the CSS needs to be done (probably) maybe one of you - who wasn't a Visual Designer in Project 1 - can do that
- Then, someone needs to shore-up any technical problems, look for mistakes, and then upload the website to the class web server, and check it one more time; maybe one of you - who wasn't a Technician in Project 1 can do that

Remember: all of you will be graded the same initially.  But if a team member fell off the face of the earth or got hit by a bus, we can redistribute the grades after the fact.  Just contact the prof by DM to talk about the process.

## Installation

- One of you must install the website on the class web server using the following web server credentials:

Note: each team will use the same FTP account. Be careful *not* to disturb other teams' files.

```
FTP Server (a.k.a. Hostname): ftp.csc174.org
FTP Port: 21
FTP Username: project2@csc174.org
FTP Password: [same]
```

*Notice above: it's "2" in the username this time - not "1"*

- When you FTP-in to the account, create a folder using the name of your **city-team** and place your website in there

## Submit the Lab

To get credit for your work:

- One of you must submit a link to your website in Blackboard, in: **Project 2: Information Architecture**
- Along with your link write in the **Write Submission** area (*not* the comments box):
  - **Your city-team name**
  - A list of **everyone's name** in your team (including your own)
  - A **link to your team's website** on the class web server
  - A **link to your team's repository** (which should be set to public)
