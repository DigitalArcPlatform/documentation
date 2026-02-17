---
title: Troubleshooting
layout: default
nav_order: 7
has_children: false
---

# Overview

As a general rule, when trying to identify what has gone wrong with your website, work backwards from the last change that you made.

# Github Pages Fails to Build Your Site 

Red icons mean the publication step ran into some issues. There are a few things you can do to make error checkign easier.

1. While you're learning, *commit changes to 1 file at a time* and check the Actions tab to make sure your changes successfully published.
1. Open up the error reporting completely to see if a specific file is named as a problem.

There are generally a few things that can result in publishing errors.

1. Repository name is different from username
1. One of the required 3-hyphen lines is missing
1. There's an extra quote or colon in the "front matter" metadata

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

# 404 Error

Error 404 means that, as far as your web browser is concerned, the page you are looking for does not exist. Often even minor details can cause this to happen. If you have recently edited a page which now 404s, try the following: 

1. Check to confirm that the YML header for that page is still properly formed.
1. Make sure that any new pages you are referencing in `_data/navigation.yml` are spelled correctly (even down to upper vs. lowercase).
1. Check that the `url` fields in `_data/navigation.yml` correspond to the `permalink` fields in your webpage markdown files.
1. Make sure that there are no special characters interfering (e.g. double/single quotes, extra dashes, backticks etc.) 

# New Page Doesn't Appear in Navigation

Remember, any time you add a new page, you will have to edit the contents of `_data/navigation.yml` to add that page to the navigation bar at the top of the site. See [Navigation Options]({{site.baseurl}}/docs/publishSite/basics/navigation/) for details on how to do that.

# The Photo of My Item Isn't Rendering As Intended

Check to make sure you have consistent naming in the .md file and the photo file. It's easy to put a hyphen in one file name and an underscore in another:

	File-name.md
	File_name.jpg
	
Because of the underscore in the `File_name.jpg`, the computer will see these as two different items.

# My items aren't showing up in the right order

Items are sorted by alphanumeric order based on the .md file name: Numbers before letters, punctuation before numbers.

Numbers will sort by alphabet, so "1" will be immediately followed by "10", where "01" will sort before "02", and so on to "10". Adding the extra zero before the 1 will let you sort numbers in order up to 99. If you have 100 objects, you'll want two zeroes before single-digit numbers and one zero before double-digit numbers.


# There are Weird Characters interspersed in my text.

Several kinds of characters can create issues.

- If you see a weird black-outlined box instead of an actual character, you might have a file with an emojis, characters with accents (cedillas, acute and grave, etc.), or a file written in languages that make use of characters beyond the 26-letter English alphabet. Using "UTF-8" characters can help. Check this [UTF-8 Character List](https://www.w3schools.com/charsets/ref_utf_reference.asp) for a copy-paste of a wide variety of characters that will display propelrly inst

- Note that markdown is sensitive to certain characters, in particular: `:`, `#`, `*`, `-`, and `` ` ``. If you have recently made a change involving any of these characters, make sure that this is intended and, if so, that you have properly escaped the character with either a backtick `` ` `` or backslash `\`. 

- Curvy quotes and curvy apostrophes need to be replaced with straight double quotes and single apostrophes.

# I Accidentally Deleted a Folder in Github/How Do I Create a New Folder in Github?

Unlike your local operating system, Github will not let you create empty folders; **any time that a folder is empty, Github will automatically prune it.** In order to create a new folder, there must be a file in it. 

There are two ways to create a new folder in Github:

## First Way

- Create a new folder with your desired name on your local machine
- Go to Github and navigate to the folder one level above where you want this folder to be located 
- Click on the menu in the top right, and choose "Upload files"
- Drag and drop the folder from your local machine into the upload field
	- *Be sure to commit changes* 
	- This will upload the entire folder and its contents to your Github repository 

## Second Way

- Go to the folder in which you want to create a subfolder
- Create a new file
- In the file name field, type the name that you want your new folder to have, followed by a forward slash `/`
	- e.g. `newFolder/`
- Then, create a placeholder file in order to prevent the folder from being empty
	- e.g. `placeholder.md`
	- *Be sure to commit changes*
- Now, you can populate the folder with the files that you intend
- **Only after you have put your own files in** can you delete the placeholder file

# I Committed My Changes, but My Page Looks the Same

If you've spent a lot of time refreshing your website, your web browser has most likely cached a number of the files that it needs to properly display your website. In other words, *your changes are live, but your browser is still displaying the old version.*

Thankfully this is easily resolved by "hard" refreshing the page using one of the following key command depending on your operating system: 

- Windows: CTRL + SHIFT + R
- MacOS: COMMAND + SHIFT + R

This will bypass your broswer's cache and pull new data to load your website. 

# My Audio Isn't in a Supported Format; What Should I Do? 

There are a number of common file types for audio (e.g. .wav, .flac, .m4a) Currently, *DigitalArc only supports `.mp3` audio uploads.* If you have non-.mp3 audio that you want to use, you will have to convert it using third-party software. Two of the most widely-used and freely available options are: 

- [Audacity](https://www.audacityteam.org/), an open source and easy-to-use audio editor which supports a number of formats
- [FFmpeg](https://www.ffmpeg.org/), an open source tool for converting both audio and video in a wide array of formats
  - **NOTE:** FFmpeg is recommended for more experienced users as it is meant to be used via command line

As always, *before manipulating/editing your files, be sure to make a backup!*
