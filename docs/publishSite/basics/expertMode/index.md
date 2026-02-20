---
title: Expert-Mode Quick Account Setup
layout: default
nav_order: 7
parent: Setting Up Your Site
grand_parent: Publishing Your Site
---

# A 5-step web-site creation overview

If you are comfortable with Github and technology in general, this quick 5-step overview will lead you through creating an account, configuring your account, and publishing to the web.

If you get stuck anywhere, the "Setting Up Your Site" and "Troubleshooting" sections will help you identify common issues quickly.

## Step 1: Create an account
{: .subheadline }

**Create a new Github.com account by following the directions [here](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github)**

1. Your Github username should be the name people will search for to find your community. For instance, a community group called "New City Community Archive" would choose the username "newcitycommunityarchive"
2. The "free" option will mean people can see, but not edit, the files that run your web site.

## Step 2: Create a project inside your new account 
{: .subheadline }

<!--**Make a copy of our template community-archive site by following this video: [https://youtu.be/aDQZ1lcpMn0](https://youtu.be/aDQZ1lcpMn0){:target="_blank"}**-->

1. Visit [`https://github.com/DigitalArcPlatform/template`](https://github.com/DigitalArcPlatform/template)
1. Press the "Use this template" button
1. Choose "Create a new repository"
1. Name your repository `yourusername.github.io` (where *yourusername* is the username you chose when you created your Github account). In our example, where the username is `newcitycommunityarchive`, you would name your repository `newcitycommunityarchive.github.io`.
1. Set the new repository to be Public. *This doesn't mean everyone who sees your files can edit them.* It means that people can see both the pretty version of your website and the files that Github uses to build the pretty web site, but *only you or the people you give your log-in to can make changes.*

## Step 3: Configure the look and feel of your new project
{: .subheadline }

<!--**Customize the `_config.yml` with your community information by following this video: [https://youtu.be/UR3RSXWGpJo](https://youtu.be/UR3RSXWGpJo){:target="_blank"}**-->

The `_config.yml` file contains settings for exhibit info, font, and color choices that affect the entire web site.

1. Gather information about your community, that includes
	- What you want to call the site
	- Who the main contact person will be
	- How do you want your site to look?
		- [Choose your fonts and colors from a preset list]({{ site.baseurl }}/docs/publishSite/basics/typefaceColor/)
1. Put these pieces of community info into our "Configuration File Generator" at [https://digitalarcplatform.kalanicraig.com/MakeConfigFile/](https://digitalarcplatform.kalanicraig.com/MakeConfigFile/)

Once you've downloaded your config file:
1. Find the "Code" navigation tab in your new Github repository.
1. Find the `_config.yml` from the list of files in your repository. All of the main settings for your site are in this file.
1. Look for the pencil icon on the right-hand side of the page. Press it to enter "edit" mode.
1. Select all of the contents of the _config.yml file in the Github editor.
1. Open the config file you generated on our web site (You can use Word or Google docs or Notepad).
1. Select all of the contents of the file and use the "Copy" command (CTRL-C on Windows or ⌘-C on Mac) to put that text into your clipboard.
1. Switch back to the _config.yml file in Github.
1. Replace the contents of the config file from our template repository with the contents of the downloaded config file by using the "Paste" command (CTRL-V on Windows or ⌘-V on Mac)
1. Scroll down and look for the green "commit" button. Press it to save your configuration file.
1. Press the green "Commit" button on the pop-up screen.

## Step 4: Create an item to display
{: .subheadline }

<!--**Add your first item by following this video: [https://youtu.be/LoFCewSXC7c](https://youtu.be/LoFCewSXC7c){:target="_blank"}**-->

Each item in the collection has an item ID (no spaces or punctuation) with one or more files associated with it (e.g. `0001.md`).

1. Open the `_items` folder and look at one of the example items. Get a feel for what you need to gather about each item.
2. Each item should have its own unique filename.
   - We like `YYYY-MM-DD-ItemNo` (so the 4th item collected on May 15, 2022, would be `2022-05-15-004`)
3. Each item will have its own information file in the `_items` folder (2022-05-15-004.md) and a photo in the `/assets/items/` folder (2022-05-15-004.jpg or 2022-05-15-004.png).
  - The file for each item in the `_items` folder has a bunch of information about each item in the first few lines. Each line has a field type (e.g. `author`), and then a colon, and then the info that goes in that field surrounded by double quotes (`author: "Drew H"`). You can get more information about what goes in these item fields in the [Metadata: Line by Line]({{ site.baseurl }}/postEvent/metadata/) section of this documentation.

## Step 5: Set up your project to publish to the web
{: .subheadline }

<!--**Publish your site using Github Pages by following this video: [https://youtu.be/MC7\_-Cx-i_E](https://youtu.be/MC7_-Cx-i_E){:target="_blank"}**-->


1. Find the "Settings" link on the top-right bar of your repository's info page
2. Find the "Pages" link on the left-hand side of your repository's settings page.
3. Look for a text box with a green or blue background at the top that says "Your site is published" or "Your site is ready to be published".
  - If you see a green box, you're ready to go. Click on the link!
  - If you see a blue box, wait 5 minutes and reload the page. It should be green now, and you can click on the link.
  - If you don't see either message, look for the drop-down menu that says "Branch", choose the "main" branch and press "Save" to publish your site in Github Pages.
4. Follow the publication process in real time by looking for the "Actions" tab (in the same line as the "Code" tab near the top of the Github page)
	- Click on Actions.
	- Find the "All Workflows" header.
	- Each time you make a change to your site, you'll see a "workflow run" line for that change. To the left of the line for that workflow run, there's an icon.
		- Green icons mean the publication step ran and everything should now be visible at your site's URL.
		- Yellow icons mean the publication step is still running.
		- Red icons mean the publication step ran into some issues. Visit the [Troubleshooting section of the documentation]({{ site.baseurl }}/troubleshooting/) for guidance on how to use the Actions tab to help figure out what's gone wrong.



