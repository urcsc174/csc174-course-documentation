# Project 1: Information Architecture

*Due: Monday, July 26, 2021* (with extra time if requested ...I'm flexible!)

**The goal** of this project is to take the separate Lab websites and combine them into a unified Information Architecture around which you'll build a new website later.

**The purpose** of this project is to demonstrate your understanding of IA, specifically: ontology, taxonomy, and choreography, as it applies to websites<s>, while working in a team of Information Architects</s> (this semester, you'll work on this project as individuals; **do not collaborate on this project!**)

## Step 1: Review the Lab Websites

Because the class is so small, here are direct links to the latest versions of the existing lab websites: [Phoenix](https://csc174.org/lab06/kwong25/), [Ridgewood](https://csc174.org/lab06/mleone10/), and [Chicago](https://csc174.org/lab06/mprice21/). Review them and take some notes about the following:

- Focus on the content (you won't need to look at code for this project); look for commonalities and differences of the CONTENT across the three websites; focus on the pages, images, and headings; think abstractly
- Take note of *things you like* about any of the websites from a content standpoint (not so much from a visual design aspect)
- Even if content that you like is in only two of the three websites (or even just one of the websites), take note of it; you're going to build your Information Architecture around *things you like*

## Step 2: Create the New Information Architecture

This is the hard part of this project: <s>working with your team</s> you need to decide on a new information architecture that you can achieve.

### THE GOAL

The IA must demonstrate your understanding of:

- Ontology
- Taxonomy
- Choreography

...by restructuring the content, by force, as necessary.  

*Note: because the three websites you have to work with are so very different, you can expect to have to use **a lot** of force to make the IA work.  That's okay for this semester because of our situation.*

### Suggested Workflow

*Note: in the first part of creating an Information Architecture (IA) you are **not** pulling together content yet.  You are only creating a structure for content.  Another way to think about it: you're creating a recipe for gathering the content ...but not the actual content itself.*

The process of developing an information architecture will feel like overkill for such a small IA!  But remember that process uses the same steps you'd use on a major website project.

Also, this first step (ontology) doesn't really have anything to do with websites!  For this part you'll create and turn-in a markdown document (.md file)

#### Ontology

Identify your classes and create your **triples**; write them in a markdown document named **ontology.md**

- Hint: the content you have to work with are all cities; they all have names, and locations; there are photos of their skylines (whether or not the exist in the websites you're working with) ...make a list of the things you want in your IA; this is called **the domain**
- Don't forget the simple things such as: *city name*, *skyline photo* ...anything else?
  - Remember: you literally write down "city name", "skyline photo" ...not the actual city names nor image files
- Create your triples from everything in your domain list; most of these will be simple like:<br>**City** has **a name**<br>**City** has **a skyline photo**<br>**City** is **a major exporter of something**<br>...stuff like that
- Expand your triples to include the things you decide to include like:<br>**City** is **known for its attractions**<br>**Famous people** were **born in the city**<br>...BTW, you'll notice that just about all your triples will be centered around "city", but that doesn't necessarily have to be so; try to think of other classes to act as the *Subject*-side of the triples

#### Taxonomy 

This next step requires you to write HTML and takes you a step closer to real content. 

Keeping your ontology (the .md file) handy for reference, create a .html file named **taxonomy.html**.  Do *not* fill the HTML file with the typical HTML document elements like doctype, etc.  Instead you'll write HTML elements that would appear *within* the BODY tag of an HTML document, but without the BODY tag (or HEAD or anything else) actually being there.

- Create a  **document structure** (using tags like HEADER, ARTICLE, ASIDE, etc.) to represent ONE city; remember, whatever document structure you use, that'll be the same for each city when you actually create a website based on this IA, later.

- Within the document structure create a common **document outline** using H (heading) tags, H1, H2, H3, etc.  

- Within the Heading tags write text to represent the *intent* of the triples from the ONTOLOGY

  - Note: do not simply type your triples!  Be creative here.  For example, if you have a triple like "**Famous people** were **born in the city**" then you might write a heading tag like "\<h2>**Some of Our Famous Sons & Daughters**\</h2>" ...or something like that
  - Remember: the idea is to use your Ontology as a *guide* for the content, not a strict roadmap.  Feel free to add headings and/or restructure or re-order as you see fit.  Just remember, whatever you do will have to be done for ALL three cities equally when you turn this into a website, later.

- In addition to HEADINGS, make placeholders for content.  In effect, write notes to yourself about what you'll need, where.  For example (typically using square brackets):

  - [intro paragraph here - about 50 words]

  - [photo here - city street scene featuring happy-looking people]

  - [city flag and emblem with city motto in caption]

    ...stuff like that

*Again: remember, when you write these things into your taxonomy document, you're in effect committing yourself to getting that content for all three cities when you actually build the website later.*

#### Choreography

This last step is often overlooked ...don't overlook it!  The order of things matters.  You need to decide.

When you created the taxonomy (above) you in-effect, also created a choreography because the content IS in order, top to bottom.  But you need to go back and really think about that order.  Make sure it's in an order that makes sense and you can explain it, later!.

Remember the LATCH framework?  Although you have very little content to work with, ask yourself, how should any of it be grouped?  Location; Alphabet; Time; Category; Hierarchy ...or any other logical method that makes sense for your content.  (BTW, you're not limited to "LATCH" ...the idea is to simply have a rationale for why things are in the order they are, and then follow it when you build the website later.)

## Submit the Files for Credit

To get credit for your work:

- Turn-in both the ontology.md file and taxonomy.html file in Blackboard, in **Project 1: Information Architecture**
