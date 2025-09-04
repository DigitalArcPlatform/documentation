---
title: Metadata Clean-Up
layout: default
nav_order: 4
parent: Post-Event Clean-Up
---

# Metadata Clean-Up

Before you prepare to publish your site, it is important to think about metadata you want to be associated with your images and other content.

## What is Metadata? 

Metadata is a set of tags which contain relevant, searchable information about your files. 

For example, a photograph of an Orioles baseball cap from the 1980s could be tagged with the following: 

- 1980s
- Memorabilia
- Baseball 
- Orioles 

## Keeping Track of Your Metadata

By far, the easiest way to keep track of your metadata before setting up your site is to use spreadsheet software such as Excel or Google Sheets, depending on your specific data collection procedures. 

### Categories 

When thinking about how to tag your data and files, consider setting up some broad categories related to the materials you've gathered. 

For instance: 

- Clothing 
- Music 
- Collectible 
- News 

In the end, the categories will depend on the nature of the items photographed and stories collected during the event. 

* Note that for your metadata categories as well as the particular metadata for a given file, there are certain text characters that you should avoid, such as double quotes ("") and colons (:). If quotes are absolutely essential, use single quotes (')  instead.

### Particulars 

The metadata for a specific item will, naturally, be particular to that item. This will include unique, indentifying details, and may include information related to the individual who submitted it. 

**If a participant has opted not to have their name included, be sure that you do NOT include any personal data about the individual(s) who submitted the item.** 

## Preparing Your Metadata Before Making Your Website

The first step in making a website is to prepare word-processing documents (Word, Google Docs, text files) that have all of the info you'll need to get your website up and running.

While you don't need to start building your site yet, it helps to understand how to format the information above into a structure that will make building your site easier. We'll cover how to use these metadata fields to actually build a web site in the section on [Posting Items]({{site.url}}{{site.baseurl}}/docs/publishSite/posting/) when you're ready to [Publish Your Site]({{site.url}}{{site.baseurl}}/docs/publishSite/)

Each item on your site will need the following information at minimum.

```
---
layout: item
format: document
title: "ACLS Digital Justice Development Grant"
author: "DigitalArc Platform Team"
contributor: "DigitalArc Platform Team"
creator: "DigitalArc Platform Team"
creationdate: 2024-05-22
type: "website"
shortdesc: "This is an example of how to include a document (scanned or screencaptured). The development of the DigitalArc Toolkit was funded by an ACLS Digital Social Justice grant in 2024."
categories: [ News Articles, Web Pages ]
---
```

Some items may have more metadata fields, or blank information, like so:

```
---
layout: item
format: document
title: "ACLS Digital Justice Development Grant"
author: "DigitalArc Platform Team"
contributor: "DigitalArc Platform Team"
group: "DigitalArc Grant Startup"
creator: "DigitalArc Platform Team"
externalurl: https://www.acls.org/recent-fellows/?program_id=40090&_project_year=2024
embedurl: 
creationdate: "May 22, 2024"
type: "website"
shortdesc: "This is an example of how to include a document (scanned or screencaptured). The development of the DigitalArc Toolkit was funded by an ACLS Digital Social Justice grant in 2024."
categories: [ News Articles, Web Pages ]
teammember: 
---
```

### Metadata line by line

Metadata starts and ends with a line that has three dashes and nothing else. (the dash next to the "zero" key on your keyboard). *If something goes wrong with an item, the first thing to check is to make sure there's no space after the three dashes.*

- `layout: item`: This never changes
- `format: photo`:  This controls the list of checkboxes that show on the right hand page of your main collection page. While you can  are 3 item formats that you're likely to encounter
	- photo (includes photos of objects or people)
	- document (includes scans of documents like memos, letters or newspaper articles)
	- media (includes embedded audio or video created by members of the community)
	- outsidelink (includes social media posts, newspaper articles that need to be linked outside of the community-archive site).
- `title: "ACLS Digital Justice Development Grant"`: The title of the item
- `author: "Michelle Dalmau, Kalani Craig, Vanessa Elias, Jazma Sutton"`: This can be blank. It's used only if the item is a written/audio/video contribution and author and creator are different than the person who contributed the item.
- `contributor: "Michelle Dalmau, Kalani Craig, Vanessa Elias, Jazma Sutton"`: The person or people who contributed the item to the collection.
- `group: "DigitalArc Grant Startup"`: If you're sorting your archive into family or content groups, this metadata field helps make that easier.
- `creator: "DigitalArc Platform Team"`: The creator of the item (a brand, a person, a collective). If you want to list both authors and a publisher or a collective name for a group of authors, the creator metadata field makes that easier.
- `externalurl: https://www.acls.org/recent-fellows/?program_id=40090&_project_year=2024`: If the item originated as an outside link or has a social-media link that you want to link to, put that link here
- `embedurl: `: If the item page should have an embedded video from YouTube or another video/audio link, put that link here
- `creationdate: "May 22, 2024"`: When was the item created? Dates like "circa 1985" work well.
- `type: `: If the community is using full metadata, this item type should be based on Library of Congress item types, which is more specific than the format metadata field above.
- `shortdesc: "This is an example of how to include a document (scanned or screencaptured). The development of the DigitalArc Toolkit was funded by an ACLS Digital Social Justice grant in 2024."`: This is the short description that shows up on the all-items list page
- `categories: [ News Articles, Web Pages ]`: This metadata field controls the filter buttons that show up on the main collection page. What categories is your community using to group items by type? Separate these by commas.
- `teammember: `: If a team-member did considerable work prepping an item or helping a contributor, they can be credited here.
