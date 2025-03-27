---
title: Web Site Creation Quick Start Guide
layout: default
nav_order: 1
permalink: /quickstart
---

# Web Site Creation Quick Start Guide

## Before you get started
{: .subheadline }

Check out our example site at [https://digitalarcplatform.github.io/demo](https://digitalarcplatform.github.io/demo), which has example items of several different types--photos, document scans, videos--so you don't have to start from scratch.

The 5 steps below will guide you through making a copy of our example site and customizing it for your community.

## Step 1
{: .subheadline }

**Create a new Github.com account by following this video: [https://youtu.be/plg5QomrHHg](https://youtu.be/plg5QomrHHg){:target="_blank"}**

1. Your Github username should be the name people will search for to find your community. For instance, a community group called "New City Community Archive" would choose the username "newcitycommunityarchive"
2. The "free" option will mean people can see, but not edit, the files that run your web site.

<!---
1)The audio of the videos is mono and a bit annoying when listening through headphones.
-->


## Step 2
{: .subheadline }

**Make a copy of our template community-archive site by following this video: [https://youtu.be/aDQZ1lcpMn0](https://youtu.be/aDQZ1lcpMn0){:target="_blank"}**

1. Visit [`https://github.com/DigitalArcPlatform/template`](https://github.com/DigitalArcPlatform/template)
2. Press the "Use this template" button
3. Choose "Create a new repository"
4. Name your repository `yourusername.github.io` (where *yourusername* is the username you chose when you created your Github account)

## Step 3
{: .subheadline }

**Customize the `_config.yml` with your community information by following this video: [https://youtu.be/UR3RSXWGpJo](https://youtu.be/UR3RSXWGpJo){:target="_blank"}**

The `_config.yml` file contains settings for exhibit info, font, and color choices that affect the entire web site.

1. Gather information about your community, that includes
	- What you want to call the site
	- Who the main contact person will be
	- How do you want your site to look? We have several preset choices for [colors]({{ site.baseurl }}/docs/colors/) and [fonts]({{ site.baseurl }}/docs/fonts/)
2. Open our "Configuration File Generator" at [https://digitalarcplatform.kalanicraig.com/MakeConfigFile/](https://digitalarcplatform.kalanicraig.com/MakeConfigFile/) and transfer your choices to this file.
3. Open the file that you just downloaded, select the entire contents of the file and use the "copy" command to put that information into your clipboard.
4. Find the `_config.yml` from the list of files in your repository. All of the main settings for your site are in this file.
5. Press the "pencil" button or "edit" button.
6. Select the entire contents of the _config.yml file and paste over it with the contents of the file you just downloaded.
7. Scroll down and look for the green "commit" button

## Step 4
{: .subheadline }

**Add your first item by following this video: [https://youtu.be/LoFCewSXC7c](https://youtu.be/LoFCewSXC7c){:target="_blank"}**

Each item in the collection has an item ID (no spaces or punctuation) with one or more files associated with it (e.g. `0001.md`).

1. Open the `_items` folder and look at one of the example items. Get a feel for what you need to gather about each item.
2. Each item should have its own unique filename.
   - We like `YYYY-MM-DD-ItemNo` (so the 4th item collected on May 15, 2022, would be `2022-05-15-004`)
3. Each item will have its own information file in the `_items` folder (2022-05-15-004.md) and a photo in the `/assets/items/` folder (2022-05-15-004.jpg or 2022-05-15-004.png).
  - The file for each item in the `_items` folder has a bunch of information about each item in the first few lines. Each line has a field type (e.g. `author`), and then a colon, and then the info that goes in that field surrounded by double quotes (`author: "Drew H"`). You can get more information about what goes in these item fields in the [Metadata: Line by Line](https://community-archive.kalanicraig.com/docs#metadata-line-by-line) section of the [Theme Docs](https://community-archive.kalanicraig.com/docs).

## Step 5
{: .subheadline }

**Publish your site using Github Pages by following this video: [https://youtu.be/MC7\_-Cx-i_E](https://youtu.be/MC7_-Cx-i_E){:target="_blank"}**


1. Find the "Settings" link on the top-right bar of your repository's info page
2. Find the "Pages" link on the left-hand side of your repository's settings page
3. Look for a text box with a green or blue background at the top that says "Your site is published" or "Your site is ready to be published"
  - If you see a green box, you're ready to go. Click on the link!
  - If you see a blue box, wait 5 minutes and reload the page. It should be green now, and you can click on the link.
  - If you don't see either message, look for the drop-down menu that says "Branch", choose the "main" branch and press "Save" to publish your site in Github Pages.
  
<!---
The publishing step needs a bit of more elaboration. I followed the steps to do it myself and when I saw the message “your website is ready to be published”, I was still looking for something like a “publish” button to click on, not knowing that all I needed to do is to wait for the page to gets published.
-->