---
title: Sharing Files
layout: default
nav_order: 5
parent: Post-Event Clean-Up
---

# Sharing Files 

This page is broken down into three sections: 

-	[Creating](#creating-a-.csv-file) a .csv File
-	Returning Files [with](#returning-files-with-mail-merge) Mail Merge
-	Returning Files [without](#returning-files-without-mail-merge) Mail Merge  

## Creating a .csv File 

Before you start, it will be easier to create a csv file for the mail merge process. For this example, we will be using Microsoft Excel on a Microsoft365 Account.

**Note:** If you are not using a software with mail merge, you can ignore this section. 

1. In Excel, create a new workbook with the following columns: 

-	first_name
-	last_name
-	object_title
-	folder_name
-	folder_link

1. In each row, enter the information for each object contributed.
1. Save the file with a .csv file extension. 

## Returning Files with Mail Merge 

This section covers how to send contributors their contributions using a mail merge feature. 

**Note:** For this guide, we will be using Microsoft Outlook and Microsoft Word on a Microsoft365 Account. The process for mail merge is roughly the same across systems, but you might have to Google "insert system mail merge." 

1. To start, the email address from which you are wanting to send the contributions back must be the **default email** account in Outlook. 
	- To set this, navigate to Settings -> Accounts to view all accounts, select the account you want as the default
	- On Mac, use the arrows in the bottom left corner to move the email to the top
	- On Windows, sign-in with the email account you want to use

1. With Outlook still open, navigate to Word and draft the email to send back to contributors 
	- We have a template available for download [here][TemplateLink].
		- To download this template, click the link and then click "View Raw." This will start the download process.
	- In the draft, label the fields that you want to fill in with the names of the column headers in your .csv file.

1. Select "Mailings" in the Ribbon in Word to open up the mail merge.
1. Select "Select Recipients" and then "Use an Existing List."
1. Select your .csv file; this will import your list. 
1. Select the text in the email draft that you want to replace with a field from the .csv file. 
	- Select "Write & Insert Fields"
	- Select "Insert Merge Field"
	- Select the field from your .csv to autofill the text
	**Note:** The name of the field will be the name of the column in your .csv, *not* the text from the rows of contributions. To see that, select "Preview Results." 
	
1. Repeat Step 6 until all of your fields are replaced. 
1. Double check that all of the fields are correctly populated by selecting "Preview Results" and scrolling through a few of the previewed emails.
1. Select "Finish & Merge" and follow the prompts. 

Once these steps are complete, Outlook will create a draft and queue for each email recipient in the .csv file. 

**Note:** Depending on the number of contributions, this will take some time (upwards of 5 to 10 minutes for large mail merges). We recommend not touching Outlook until all the emails have been successfully sent. 

## Returning Files without Mail Merge 

This section covers how to send contributors their files without using a mail merge feature. 

Without mail merge, this is a more tedious process because you will have to draft each email and send them individually. 	
	- We have a template available for download [here][TemplateLink].
		- To download this template, click the link and then click "View Raw." This will start the download process.
		
Simply draft your email in your inbox and copy over the links that you have prepared for each contributor's folder in the online storage platform of your choosing (e.g. Google Drive, Dropbox, etc.). 

**Note:** If you are not using an online storage platform to store the files, you can attach them to the email as a .zip archive from your computer. 

----
[TemplateLink]: https://github.com/mdlandini/idah_toolkit_testing/blob/main/assets/images/Email%20Template%20for%20Sharing%20Files.docx