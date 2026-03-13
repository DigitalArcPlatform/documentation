---
title: "There's a 404 Error Where a Page Should Be"
layout: default
nav_order: 4
parent: Troubleshooting
---

# There's a 404 Error Where a Page Should Be

Error 404 means that, as far as your web browser is concerned, the page you are looking for does not exist. Often even minor details can cause this to happen. If you have recently edited a page which now 404s, try the following: 

1. Check to confirm that the YML header for that page is still properly formed.
1. Make sure that any new pages you are referencing in `_data/navigation.yml` are spelled correctly (even down to upper vs. lowercase).
1. Check that the `url` fields in `_data/navigation.yml` correspond to the `permalink` fields in your webpage markdown files.
1. Make sure that there are no special characters interfering (e.g. double/single quotes, extra dashes, backticks etc.) 

