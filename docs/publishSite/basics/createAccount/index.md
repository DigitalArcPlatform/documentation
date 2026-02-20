---
title: Create a Github Account
layout: default
nav_order: 1
parent: Setting Up Your Site
grand_parent: Publishing Your Site
---

# Before you get started
{: .subheadline }

Get to know the files in our example site, which has example items of several different types--photos, document scans, videos--so you don't have to start from scratch.

- Sample site as site visitors see it: [https://digitalarcplatform.github.io/demo](https://digitalarcplatform.github.io/demo)
- The files that make the samplesite run: [https://github.com/DigitalArcPlatform/demo](https://github.com/DigitalArcPlatform/demo)

# Create a Github Account

Before you create your account, it helps to understand how Github usernames will be seen by your website visitors.

Your Github username will be included in the website address people will use for to find your community, so choose it carefully.

- Example Github username: newcitycommunityarchive
- Example community-archive website address: newcitycommunityarchive.github.io

The "free" option will mean people can see, but not edit, the files that run your web site.

Ready? *Create a new Github.com account by following the directions [here](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github)**

# Create a project inside your new account 
{: .subheadline }

GitHub uses "repository" to describe the place where all of the files for a single project are stored.

You're going to copy a repository that we've already made, so that you have example files to work from rather than having to create files from scratch.

1. Visit [`https://github.com/DigitalArcPlatform/template`](https://github.com/DigitalArcPlatform/template)
1. Press the "Use this template" button
1. Choose "Create a new repository"
1. Name your repository `yourusername.github.io` (where *yourusername* is the username you chose when you created your Github account). In our example, where the username is `newcitycommunityarchive`, you would name your repository `newcitycommunityarchive.github.io`. ***Your github username must be exactly the same as the first part of your repository name, and ".github.io" must appear after your repository name.***
1. Set the new repository to be Public. *This doesn't mean everyone who sees your files can edit them.* It means that people can see both the pretty version of your website and the files that Github uses to build the pretty web site, but *only you or the people you give your log-in to can make changes.*

# Research your configuration choices 
{: .subheadline }

<!--**Customize the `_config.yml` with your community information by following this video: [https://youtu.be/UR3RSXWGpJo](https://youtu.be/UR3RSXWGpJo){:target="_blank"}**-->

Your new "repository" or "place where all your files are stored" `_config.yml` file contains settings for exhibit info, font, and color choices that affect the entire web site.

The next few sections of documentation will cover each one of these things one by one, but reading through this first before you start trying to make changes will help you get your bearings.

***If you get lost look for the `Code` button toward the ***

## # Get to know your _config.yml file

One file in your newly copied web sit controls a lot of the information on the site: `_config.yml`. You can generate one at [https://digitalarcplatform.kalanicraig.com/MakeConfigFile/](https://digitalarcplatform.kalanicraig.com/MakeConfigFile/)

1. Gather information about your community, that includes
	- What you want to call the site
	- Who the main contact person will be
	- How do you want your site to look?
		- [Choose your fonts and colors from a preset list]({{ site.baseurl }}/docs/publishSite/basics/typefaceColor/)
1. Put these pieces of community info into our "Configuration File Generator" at [https://digitalarcplatform.kalanicraig.com/MakeConfigFile/](https://digitalarcplatform.kalanicraig.com/MakeConfigFile/)

# Apply your configuration choices 

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

