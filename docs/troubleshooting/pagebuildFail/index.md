---
title: "Github Pages Fails to Build Your Site"
layout: default
nav_order: 1
parent: Troubleshooting
---

There are generally a few things that can result in publishing errors.

1. Repository name is different from username
1. One of the required 3-hyphen lines, at the beginning or the end of the metadata that's at the beginning of each file is missing. If you see a table at the top of the page content when you view it in the "Code" tab, that means your file is properly formatted. If you can actually see the three hyphens, look closely at the metadata to make sure it's properly formatted.
    1. No missing hyphen
    2. No spaces before or after the hyphens
    3. No line return before the first set of 3 hyphens 
1. There's an extra quote or colon in the "front matter" metadata that is between the three hyphens.

## Repository Name is Different from Username

Your repository must be named based on the username of your GitHub account, otherwise *the website will not build properly.* Note, however, that this can easily be remedied:

1. Go to your GitHub repository
1. Go to the "Settings" tab
1. Under General, you will see a field for your repository name
1. Click the box and rename your repository to `[yourusername].github.io`
1. Click "Rename"
   1. Note that you may need to click "Rename" a second time, as the first click may simply check to verify that the new name is available
  
Once you've finished, go to the "Actions" tab to check the build progress.

## One of the required 3-hyphen lines is missing

Every `.md` file in your site has two sets of 3 hyphens (`---`), as the first line of the .md file and as a divider between the "front matter" metadata and the main part of the .md file. These need to be positioned and typed exactly.

Check each recent file and look at both instances of the 3-hyphen lines
1. Does each line of hyphens have exactly 3 hyphens?
1. Is there a blank line before the first set of 3 hyphens? Remove the blank line.
1. Is there a blank line after the second set of 3 hyphens? Add one by adding a line return.
1. Are there spaces or tabs before or after either set of 3 hyphens? Remove them.

## There's an extra quote or colon in the "front matter" metadata

There are two characters that can create problems for the metadata between the two sets of hyphens: quotes and colons.

Each front-matter line is the name of a type of information, a colon, and the actual information that gets used. For instance, the title of a page is set in this front matter:

	title: Title of Page

If the page title actually has a colon in it, that can break the publish. Add quotes around the whole title to make the second colon show up as a colon instead of being something the computer reads as a computational marker.

	title: Title of Page: this is a page that does something

	title: "Title of Page: this is a page that does something"

Too many quotes can also be an issue. If the page title has quotes around it, and there are also quotes in the title, that can create a problem. Use apostrophes as quotes inside the double quotes

	title: "Title of Page: "Some word" is in quotes"

	title: "Title of Page: 'Some word' is in quotes"

