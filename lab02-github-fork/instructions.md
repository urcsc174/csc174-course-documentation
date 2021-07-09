# Lab 2: GitHub Fork

*Due: Monday, July 12, 2021*

**The goal** of this lab is to *fork* someone else's GitHub repository so you can work on it and make improvements.  Exactly what improvements you make and how good they are, is not important for this lab.  (They will be, later.)  The key thing is to simply get someone else's source code, make some changes, and then publish the result.

*Note: in Friday's class I demonstrated how to add someone as "collaborator" to a repository.  That will be important later in CSC 174 but it's **not** something you need to do for Lab 2. For Lab 2, you just need to do this thing called forking.*

## Step 1: Review Websites using Markdown 

- Create **a markdown file** to capture notes as you review other students' websites
  - Make sure to demonstrate your ability to use markdown appropriately in your document to prove you can do it
  - Be sure to use the GFM standard because you'll be publishing this markdown file in GitHub
  - Include typical college stuff at the top of the document: name, date, name of this assignment, etc., and then use appropriate headings and other typical document-y stuff to make it easy to read
- Go to [http://csc174.org/lab01/](http://csc174.org/lab01/) and review *at least* THREE other students' Lab 1 websites from a VISUAL standpoint
  - You can ignore technical aspects of the websites - things like validation, file structure, etc; only focus on things you can *see*, and your user experience
  - You can review more than three, but three is the minimum
  - The level of detail you describe is not important so long as you capture meaningful observations and make relevant suggestions
  - You can also use the instructor's websites to review (rkostin and rkostin2) but be kind!  (The professor has very thin skin!)
- As you review each website, consider the following topics
  - Color Scheme (suggestion: *Google* that term)
    - do the colors work well?
    - if so, what parts do you like? if not, suggest improvements
  - Layout and box model (incl. navigation)
    - do the elements sit in the viewport in a "normal" or expected way?
    - if not, describe the problems and make suggestions
  - Visual embellishments (borders, background images, etc.)
    - do the extra visual elements add value or distract?
    - make suggestions
  - Standout features (anything impressive)
- Save and hold on to your markdown file.  You'll need it later.

## Step 2: Share Your GitHub User Name

- If you haven't already, create an account in GitHub
- In our CSC 174 Slack Workspace, publish your GitHub username in the **#chatter** channel

## Step 3: Publish Your Lab 1 Website in GitHub

*In Friday's class, we practiced creating a repository.  If you were following along, you may have used your Lab 1 website.  If you did and you named the repo something like "demo" and/or made any changes to it, then DO NOT use that repository for this lab assignment.  We need a clean/new repo with your Lab 1 files for this assignment.  BTW - if you want to delete that demo repo and can't figure out how to do it, ask the instructor in our #help channel in Slack.*

- Create a new repository in GitHub and publish your Lab 1 files there
  - Name the repository: **CSC 174 Lab 1**
  - Required: make sure you make the repo "public"
  - Optional: create a **.gitignore** file with the entries `.DS_Store` and `Thumbs.db` ...and if you discover more files that need to be *ignored*, add them as well (and maybe share what you discovered in our #chatter channel in Slack!)
  - A **readme.md** file is not required for this assignment

Note: whether or not you properly sync this repo to your files on your computer is not important (and the professor can't tell if you did anyway).  For this assignment, we only need access to the *copy* of your Lab 1 files on the GitHub website.

## Step 4: Fork Another Student's Website

- Using the other students' GitHub usernames (from Step 2, above), find their Lab 1 repos and then pick ONE you want to edit based on the notes you wrote as part of Step 1, above
  - Note: you may have written a lot of notes on (at least) three websites - which is good practice! - but you only need to implement a few things on only one website.
- "Fork" the website you chose from its repository in GitHub
  - While looking at a student's website in GitHub, look for the **Fork** button in the top right; click it and then when the process completes, notice you're looking at the same website except it's a copy - in *your* GitHub account
- "Clone" the fork'd website to your own computer
  - Click the green **Code** button and either use the web URL (not demonstrated in Friday's class) or the **Open with GitHub Desktop** selection (recommended)
  - Remember to be careful with the "Local Path" - you need to put it in your *localhost* 
    - BTW - when specifying the "Local Path" you can change the folder name (the end of the path) to whatever makes sense to you (e.g. "lab02")
  - When asked, "How are you planning to use this fork?" ...click "**To Contribute...**"

## Step 5: Make Edits and Commits

At this point you'll find you have the other student's Lab 1 website on your computer.  Open it up in your localhost (using your MAMP, WAMP, or whatever stack you're using) and confirm it's an identical copy of what you saw here: [http://csc174.org/lab01/](http://csc174.org/lab01/)

- Using your notes (from your markdown file), to the best of your ability make ONE change/fix to the website
- Using the GitHub Desktop software, create a "commit" by writing a Summary and (optional) Description, and then click the Commit button
- Repeat these two things (directly above) two more times: edit & commit; edit & commit
  - You can do more, but at the very least make a total of three commits
- Add your markdown file to your local repository - in the root, along with the webpages, then commit that as well
- Finally, "push" the commits to the repo on GitHub (click the **Push Origin** button)

Check your handiwork in GitHub (the website).  

- There, you'll see a message on the page: "This branch is *nn* commits ahead of..." or something like that.  

You don't have to do anything with that now - but just be advised, that's how you can send your "improvements" from your *fork* back to the originator's repository.  

## Step 6: Turn-in the Lab Assignment in Blackboard

To get credit for your work:

- Get the URL of *your* forked copy of the other student's website (make sure you are not looking at the other student's original website!)
- In Blackboard, find the Lab 2 assignment and paste the URL of your repository in the "Write Submission" area and Submit it
