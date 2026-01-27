---
title: File Naming
layout: default
nav_order: 1
parent: Post-Event Clean-Up
---

# File Naming

In order to more easily keep track of the numerous photographs and audio files from a community history gathering event, it will be essential to have a system for standardizing file names. 

If you have followed the system of Object ID stickers which we present in the [Pre-Event Setup]({{site.url}}{{site.baseurl}}/docs/preEvent/preEvent.html) section, this will simplify the process.

In short, we recommend the following system for naming your files: 

- YYYY-MM-DD is the date on which the event is hosted
- XXXX denotes the order in which that items were collected (i.e. 0001 is the first item, 0002 is the second, etc.) 

Hence 2024-03-21-0004 would correspond to the fourth item collected on March 21st, 2024.

## General Guidelines

Should you wish to use a different naming system, it is important to keep the following guidelines in mind:

-	Are the filenames easily identifiable?
-	Are they easily searchable?
-	Are they easy for volunteers of different types to make sense of?

## How to name photos:

You may have one photo of an object or many photos. Naming the files correctly will help when you're ready to build your web site.

For an item ID of `2025-05-31-001-photo`:

1. If there's only one photo, the photo name should be `2025-05-31-001-photo.jpg` or  `2025-05-31-001-photo.png`.
1. If there are multiple photos
	1. use the base item ID as the first part of the photo name.
	1. Then use an underscore.
	1. Then add numbers to the end of each photo

This allows you to control the order in which the photos displays. For example, the first photo in the sequence would be named `2025-05-31-001-photo_01.png` and the second photo on the sequence would be named `2025-05-31-001-photo_02.png`.

The zero before the numbers "1" and "2" in these examples helps the computer sort them in order. The photo with the lowest number will be used as the featured photo on the page with the whole list of items.

## The Importance of Proper File Names 

Not only does having a coherent scheme for your file names make it easier to organize, it is actually a critical part of how the DigitalArc system works. The names that you assign your files **must** match with the names that you assign your [metadata](https://digitalarcplatform.github.io/documentation/docs/publishSite/posting/) markdown files once you upload both of them to GitHub.

For example, the following pair of files will work correctly because they match *exactly*:

![Correct Markdown File]({{site.baseurl}}{{site.imageurl}}/postEvent/naming/correct_md_1.png)
![Correct Image File]({{site.baseurl}}{{site.imageurl}}/postEvent/naming/correct_image_1.png)

However, even small discrepancies will cause the item not to render correctly, such as in the following pair:

![Correct Markdown File]({{site.baseurl}}{{site.imageurl}}/postEvent/naming/correct_md_1.png)
![Incorrect Image File]({{site.baseurl}}{{site.imageurl}}/postEvent/naming/incorrect_image_1.png)

Notice that the image file contains one less 0 than the markdown file. In other cases, the file names may look superficially similar, but will be interpreted by GitHub Pages quite differently: 

![Correct Markdown File]({{site.baseurl}}{{site.imageurl}}/postEvent/naming/correct_md_1.png)
![Incorrect Image File]({{site.baseurl}}{{site.imageurl}}/postEvent/naming/incorrect_image_2.png)

Even though the characters though all the date and item information is correct, the markdown file uses dashes to separate the information, while the image uses underscores. 

The key takeaway is that *your files must match character for character*, otherwise your items will not display properly. 
