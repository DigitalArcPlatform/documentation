---
title: Creating Additional pages
layout: default
nav_order: 2
parent: Customizing the Jekyll Theme
grand_parent: Publishing Your Site
---

# Creating Additional pages

There are three main pages in the DigitalArc template site at XXXXX. Those three pages are visible in the navigation for visitors to click on:
- 
- 
- 

If you want to add a page, we've created a blank template page that you can use, at `/pages/newpageexample.md`

You can either use this page as a guide to make a new file, or you can change the name of this page and its contents to create your new file, which ever seems easiest.

1. Update the name of the markdown file in the field that reads `samplenewpage` above the Edit/Preview tabs (after `/demo/pages/` and before `in main`)
1. Change the value in the line that begins with `title` in the YML front-matter (the stuff between the `---` lines).
1. Keep the `layout: page` line. This adds your web site's navigation, header and footer.
1. Set the permalink value to the web site address you want people to go to. For instance, if your site URL is `digitalarcplatform.github.io` and you want people to see this page at `digitalarcplatform.github.io/about`, change that line to read `permalink: /about`
1. Replace the text here, starting with the large header (the line that starts with `#`) and including this text.


In the `newpageexample.md`, you'll see these instructions repeated, so you can easily modify the file to display new content for your community.

```
---
title: Sample New Page
layout: page
permalink: /newpage
---

# Want to add a new page that doesn't exist?

1. Update the name of the markdown file in the field that reads `samplenewpage` above the Edit/Preview tabs (after `/demo/pages/` and before `in main`)
1. Change the value in the line that begins with `title` in the YML front-matter (the stuff between the `---` lines).
1. Keep the `layout: page` line. This adds your web site's navigation, header and footer.
1. Set the permalink value to the web site address you want people to go to. For instance, if your site URL is `digitalarcplatform.github.io` and you want people to see this page at `digitalarcplatform.github.io/about`, change that line to read `permalink: /about`
1. Replace the text here, starting with the large header (the line that starts with `#`) and including this text.
```