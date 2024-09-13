---
title: Making Your Site Public
layout: default
nav_order: 5
parent: Publishing Your Site
---

# Making Your Site Public 

The objective of this page is to lay out how to get your website up and running on Github Pages by using some template materials that we have created. 

## Before You Start 

Check out the example site [**here**](https://idahatiu.github.io). This has example items of several different types such as photos, document scans, and videos. 

The steps below will guide you through making a copy of this example site and customizing it for your community. 

## Step 1

If you have not already, create a new Github account by following [**this video](https://youtu.be/plg5QomrHHg)

1. Your Github username should be the name that people will use to search for your archive. For instance, a community group called "New City Community Archive" would choose the username "newcitycommunityarchive"
1. The "free" option will mean that people cna see, but not edit, the files that run your website. 

## Step 2

Make a copy of our template community-archive site by following [**this video**](https://youtu.be/aDQZ1lcpMn0)

1. Visit https://github.com/idahatiu/idahatiu.github.io
1. Press the "Fork" button 
1. Rename your repository "USERNAME.github.io" where USERNAME is the username you used for your community github account

## Step 3

### Using the Form 

For ease of setup, we have developed a page which will generate a configuration file for your website. To use it, follow [**this link**](https://community-archive.kalanicraig.com/ConfigForm/) and fill out the relevant fields.

### Setting Up Your Own Config File 

Customize the _config.yml with your community information by following [**this video**](https://youtu.be/UR3RSXWGpJo)

The _config.yml file contains the settings for exhibit information, fonts, and color choices which affect the entire website.

1. Select the _config.yml from the list of files in your repository.
1. Click the pencil button to edit the file
	1. Information about your community is on lines 42-63. To leave a line blank, put two double quotes together with no spaces: ""
	1. Choices for colors and fonts are on lines 77-93
1. Scroll to the bottom and use the "Commit" button (Github's equivalent of a "Save" button)

## Step 4

Add your first item to your site by following [**this video**](https://youtu.be/LoFCewSXC7c)

Each items in the collection should have an item ID (without spaces or punctuation) and one or more markdown files associated with it (e.g. 0001.md)

1. Open the _items folder and look at one of the example items. Get a sense for what you need to gather about each item. 
1. Each item should have a unique filename (e.g. YYYY-MM-DD-ItemNum)
1. Each item will have its own information file in the _items folder (e.g. 2022-05-15-004.md) and a corresponding photo in the /assets/items/ folder  
	- The file for each item in the _items folder has information about each item in the first few lines. Each line has a field type (e.g. author), followed by a colon, and then the information for that field in double quotes (e.g. author: "Mike M").
	
## Step 5

Publish your site using Github Pages by following [**this video**](https://youtu.be/MC7_-Cx-i_E) 

1. Find the "Settings" link on the top-right bar of your repository's info page 
1. Fine the "Pages" link on the left-hand side of your repository's settings page
1. Look for a text box with a green or blue background at the top that says "Your site is published" or "Your site is ready to be published"
	- If you see a green box, you're ready to go. Click on the link to view your site! 
	- If you see a blue box, wait for 5 minutes and reload the page. It should be green now, and you can click on the link.
	- If you don't see either message, look for the drop-down menu that says "Branch," choose the "main" branch and press "Save" to publish your site in Github Pages.