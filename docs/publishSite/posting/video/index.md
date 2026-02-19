---
title: Video
layout: default
nav_order: 3
parent: Posting Items
grand_parent: Publishing Your Site
---

# Video

## Uploading to YouTube

Uploading and maintaining videos in your Github repository or Google Drive can be challenging due to filesize constraints. We recommend [uploading to YouTube](https://support.google.com/youtube/answer/57407?hl=en&co=GENIE.Platform%3DDesktop) so that you can automatically link to the video through the video's URL.


## Linking to Your Video

To get the link to a YouTube video:

1. In YouTube, go to the desired video and press the "Share" button (typically located below the video player).
1. Press the "Copy" button to copy the YouTube link to your clipboard.
	- Note: If the URL it provides contains the flag `?si=`, you may want to consider removing this as well as any text that follows it.
1. Open the corresponding item `.md` file in the `items` folder and look for the lines that start with `externalurl:` and `embedurl:`.
1. Choose how you want your video to appear.
	1. If you want a tiny version of the video to be automatically embedded in the page, paste the copied URL after `embedurl: `.
	1. If you want the video to be linked with the text "For more information, visit....", paste the copied URL after `externalurl: `.

For an example of how this looks, visit [https://digitalarcplatform.github.io/demo/items/Item-3-video.html](https://digitalarcplatform.github.io/demo/items/Item-3-video.html)
