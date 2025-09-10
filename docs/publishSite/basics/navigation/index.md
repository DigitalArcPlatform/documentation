---
title: Navigation Options
layout: default
nav_order: 4
parent: The Basics
grand_parent: Publishing Your Site
---

# Navigation Options

There are two main pages in the DigitalArc template site that are visible to viewers. The files that control these pages are at https://github.com/DigitalArcPlatform/template/tree/main/pages. Those two pages are visible in the navigation for visitors to click on:
- "Our Community" links to the `index.md` file. We used the name "index" because "index.html" is the most common placeholder file for default display if there is no other content in a folder.
- "Our Collection" links to the `collection.md` file. That file automatically creates the digital-exhibit list of community-contributed objects that are created by uploading .md files to the _items folder and adding corresponding images to the `/assets/items/` folder.

You can change the navigation-menu items that appear in the top navigation of your site. For example, if you want to link to an existing "About Us" page on another website, or link to a new page in your community archive, you can.

***Before you start***:1
1. Make sure you leave the field variable-name portion of the line (the part of each line before the colon) the same. Change only the field label (the part after the colon, in quotes).
2. Remember that there's limited space available in the navigation bar. We recommend using short 2-3 word titles and only having 3-4 navigation elements at most.

The current file at `_data/navigation.yml` looks like this:

```
# Site navigation links

- title: Our Community
  url: /
  excerpt:
  image:

- title: Our Collection
  url: /collection
  excerpt:
  image:
```

- The "title" element will display readable text to your site visitors.
- The "url" element will provide the link that users get when they click the readable text
- The "excerpt" and "image" elements are currently not in use but we've added them to make sure that sites using the current DigitalArc template work properly when we do future development work.

To add a navigation link to an existing About Us page at https://digitalarcplatform.github.io/about/, you would copy one of the navigation-item sections and make changes to it, like this:

```
# Site navigation links

- title: Our Community
  url: /
  excerpt:
  image:

- title: Our Collection
  url: /collection
  excerpt:
  image:
  
- title: About Us
  url: https://digitalarcplatform.github.io/about/
  excerpt:
  image:
  
```

