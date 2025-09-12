---
title: Making Your Site Public
layout: default
nav_order: 5
parent: Publishing Your Site
---

# Making Your Site Public 

GitHub has a feature called "Pages" that will turn any Github site into a public website.

Turning that feature on is very easy:

1. Find the "Settings" link on the top-right bar of your repository's info page.
2. Find the "Pages" link on the left-hand side of your repository's settings page.
3. Look for a text box with a green or blue background at the top that says "Your site is published" or "Your site is ready to be published".
  - If you see a green box, you're ready to go. Click on the link!
  - If you see a blue box, wait 5 minutes and reload the page. It should be green now, and you can click on the link.
  - If you don't see either message, look for the drop-down menu that says "Branch", choose the "main" branch and press "Save" to publish your site in Github Pages.
4. Follow the publication process in real time by looking for the "Actions" tab (in the same line as the "Code" tab near the top of the Github page).
	- Click on Actions.
	- Find the "All Workflows" header.
	- Each time you make a change to your site, you'll see a "workflow run" line for that change. To the left of the line for that workflow run, there's an icon.
		- Green icons mean the publication step ran and everything should now be visible at your site's URL.
		- Yellow icons mean the publication step is still running.
		- Red icons mean the publication step ran into some issues. Visit the [Troubleshooting section of the documentation]({{ site.baseurl }}/troubleshooting/) for guidance on how to use the Actions tab to help figure out what's gone wrong.
