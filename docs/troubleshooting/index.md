---
title: Troubleshooting
layout: default
nav_order: 7
has_children: false
---

# Overview

As a general rule, when trying to identify what has gone wrong with your website, work backwards from the last change that you made.


## Github Pages Fails to Build Your Site 

Red icons mean the publication step ran into some issues. Visit the [Troubleshooting section of the documentation]({{ site.baseurl }}/troubleshooting/) for guidance on how to use the Actions tab to help figure out what's gone wrong.

## 404 Error

Error 404 means that, as far as your web browser is concerned, the page you are looking for does not exist. Often even minor details can cause this to happen. If you have recently edited a page which now 404s, try the following: 

1. Check to confirm that the YML header for that page is still properly formed.
1. Make sure that any new pages you are referencing in `_data/navigation.yml` are spelled correctly (even down to upper vs. lowercase).
1. Check that the `url` fields in `_data/navigation.yml` correspond to the `permalink` fields in your webpage markdown files.
1. Make sure that there are no special characters interfering (e.g. double/single quotes, extra dashes, backticks etc.) 

## New Page Doesn't Appear in Navigation

Remember, any time you add a new page, you will have to edit the contents of `_data/navigation.yml` to add that page to the navigation bar at the top of the site. See [Navigation Options]({{site.baseurl}}/docs/publishSite/basics/navigation/) for details on how to do that.

## Added Text Isn't Rendering As Intended

Note that markdown is sensitive to certain characters, in particular: `#`, `*`, `-`, and `` ` ``. If you have recently made a change involving any of these characters, make sure that this is intended and, if so, that you have properly escaped the character with either a backtick `` ` `` or backslash `\`. 
