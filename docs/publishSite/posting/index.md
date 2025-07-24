---
title: Posting Items 
layout: default
nav_order: 3
parent: Publishing Your Site
has_children: true
---

# Posting Items

The item IDs you chose during the event are the single most important piece of prep work for posting items.

The item IDs assigned during the event are used to name two sets of files, each of which belongs in a specific folder:
1. The first is a single text-only file that contains text-based information about each piece in your community archive. See ***Item Text Files*** below. These should be stored in the `_items` folder. If the item ID was `2025-05-31-001-photo`, this text file will be called `2025-05-31-001-photo.md` .
1. The second are the photo or photos that were taken of the object. See ***Photo Files*** below. It's likely that you've named the photos already (see [Naming Files after the Event]({{ site.baseurl }}/docs/postEvent/naming/)

## Create an Item Text File

The meta-data that you prepped using contributor sign of information in the post processing phase will give you all of the information you need to fill out the text file.

1. Use a word processor (Microsoft Word, Google Docs, Mac Pages, etc.) to edit the information in your item text file first. (See "Anatomy of an Item Text File" below for an in-depth guide)
1. Open the `_items` folder in your Github repo.
1. Press the "Add File" button and choose "Create New File"
![How to Create New File in Github]({{ site.baseurl }}{{ site.imageurl }}/publishSite/basics/github_screenshot_addnewfile.png)
1. Find the "Name your file" field and enter the file name. (In our example, `2025-05-31-001-photo.md`)
![How to edit file names and contents in Github]({{ site.baseurl }}{{ site.imageurl }}/publishSite/basics/github_screenshot_editfilenamecontents.png)
1. Find the "enter file contents here" field. Copy and paste the information from your word processor into that field 
1. Press the "Commit changes" button.
1. In the pop-up window, press the "Commit changes" button again.

### Anatomy of an Item Text File

#### Example

```
---
layout: item
format: document
title: "ACLS Digital Justice Development Grant"
contributor: "DigitalArc Platform Team"
group: "IUB-OC"
externalurl: https://www.acls.org/recent-fellows/?program_id=40090&_project_year=2024
embedurl: 
creationdate: 2024-05-22
type: "website"
shortdesc: "This is an example of how to include a document (scanned or screencaptured). The development of the DigitalArc Toolkit was funded by an ACLS Digital Social Justice grant in 2024."
categories: [ News Articles, Web Pages ]
tags: [  ]
---
```

#### Explanation of each part of the example

##### Three hyphens

At the top of the example item text file, you'll see three hyphens `---` .  These tell the system that builds your website that there's *metadata* or information about an object that's used to build the web site, coming up. The first line of ever item file needs to be these three hyphens, without any extra spaces or characters after the hyphens.

##### Layout

The next line is starts with "layout" and has the word "item" after the colon. This says, "Please use the layout that DigitalArc has customized to automatically display item photos, transcripts, and item info". This line is also helpful for understanding the other lines of metadata.

##### Other "variables"

Each metadata line has a variable--"layout"--and a value for that variable. That is, the variable before the colon says "this is a placeholder"; whenever the web site system sees a reference to "layout", it will replace that reference with the actual value that comes after the colon ("item" in this case).

The lines that follow these first three hyphens are variables and values that hold the object info that you prepped in post-processing, including things like "item name" and "contributor name".

##### Three more hyphens

After the metadata, there's another set of three hypens. Like the hyphens that start each item file, these need to be on their online with no spaces before or after

##### Adding more detail

If you don't want to write any additional information after the last three-hypen line, you don't need to.

If you do have other information that you'd like to include, press "enter" or "return" to add a blank line after the metadata-closing hyphens and then type whatever you want. The text that you display here will show to the user below the photos on the website. That text is formatted using "markdown", which is a simple text-based way to tell the computer to make text look the way you want it to.
- `# big header`
- `## medium header`
- `**bold**`
- `*italic`
- To make bullet points, put a hyphen and a space at the beginning of each line that should have a bullet point: `- bullet point text`
- To make a numbered list, put a 1, a period and a space at the beginning of each line that should have a number, and the computer will auto-number the list for you: `1. number one. 1. number two.`