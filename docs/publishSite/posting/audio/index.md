---
title: Audio
layout: default
nav_order: 2
parent: Posting Items
grand_parent: Publishing Your Site
---

# Audio

If you plan to include audio interviews with a contribution in your collection, the process is very similar to naming and uploading photos.

***Before you start***: Make sure your audio and transcript files are [named properly first]({{site.baseurl}}/docs/postEvent/naming/) and are saved to your computer; *you cannot upload directly from Google Drive or other file hosting services*. Both audio files (.mp3) and transcript files (with the word "_Transcript" in the file name) are stored in the "assets/transcripts" folder.

- The audio file needs to be named `itemnumber.mp3`.
  - **NOTE:** Currently, DigitalArc only accepts audio files in `.mp3`; if your audio is not formatted as `.mp3`, you will need to [convert it]({{site.url}}{{site.baseurl}}/docs/troubleshooting/#my-audio-isnt-in-a-supported-format-what-should-i-do) to `.mp3` before uploading.
  - **NOTE:** If your audio file is larger than 25MB, you will need to [upload it to YouTube]({{site.url}}{{site.baseurl}}/docs/publishSite/posting/video/) and link to it from there
- If there's an accompanying transcript, it should be a Word doc file (with a `.docx` extension) and should be named `itemnumber_Transcript.docx`.
- *Example:* For an item named `2023-10-14-0001`, your audio file would be named `2023-10-14-0001.mp3` and the text version of the transcript would be named `2023-10-14-0001_Transcript.docx`.

To upload audio and transcript files: 
1. Open the `assets` folder in your Github repo.
1. Open the `transcripts` folder in that `assets` folder.
![How to find the image folder in your DigitalArc repo]({{ site.baseurl }}{{ site.imageurl }}/publishSite/basics/github_screenshot_imagefolderlocation.png)
1. Press the "Add File" button and choose "Upload file".
1. Drag the files you want to upload into the "Drag files" area.
1. Press the "Commit changes" button.
1. In the pop-up window, press the "Commit changes" button again.
