---
title: Creating Additional pages
layout: default
nav_order: 2
parent: Customizing the Jekyll Theme
grand_parent: Publishing Your Site
---

# Creating Additional pages

In the [Navigation Options]({{ site.baseurl }}{{ site.imageurl }}/publishSite/basics/navigation) section of this documentation, we noted the two main pages that display in the DigitalArc template (the "Our Community" index.md file, and the "Our Collection" collections.md file, both in the `pages` folder of the main Code section.)

If you want to add a page with your own content, there's a placeholder new-content-example page, which you can use as starting point to make your own pages, at `/pages/samplenewpage.md`

You can either use this page as a guide to make a new .md file, or you can change the name of this page and its contents to create your new file, whichever seems easiest.

1. Update the name of the markdown file in the field that reads `samplenewpage` above the Edit/Preview tabs (after `/demo/pages/` and before `in main`).
![image]({{ site.baseurl }}{{ site.imageurl }}/publishSite/customizing/newPage/GithubRenameFile.png).
1. Change the value in the line that begins with `title` in the YML front-matter (the stuff between the `---` lines).
1. Keep the `layout: page` line. This adds your website's navigation, header, and footer.
1. Set the permalink value to the website address you want people to go to. For instance, if your site URL is `digitalarcplatform.github.io` and you want people to see this page at `digitalarcplatform.github.io/about`, change that line to read `permalink: /about`.
1. Replace the text here, starting with the large header (the line that starts with `#`) and including this text.

In the `samplenewpage.md`, you'll see these instructions repeated, so you can easily modify the file to display new content for your community.

```
---
title: Sample New Page
layout: page
permalink: /newpage
---

# Want to add a new page that doesn't exist?

1. Update the name of the markdown file in the field that reads `samplenewpage` above the Edit/Preview tabs (after `/demo/pages/` and before `in main`)
1. Change the value in the line that begins with `title` in the YML front-matter (the stuff between the `---` lines).
1. Keep the `layout: page` line. This adds your website's navigation, header, and footer.
1. Set the permalink value to the website address you want people to go to. For instance, if your site URL is `digitalarcplatform.github.io` and you want people to see this page at `digitalarcplatform.github.io/about`, change that line to read `permalink: /about`
1. Replace the text here, starting with the large header (the line that starts with `#`) and including this text.
```
