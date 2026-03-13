---
title: "I Accidentally Deleted a Folder in Github and Can't Recreate It"
layout: default
nav_order: 6
parent: Troubleshooting
---

# I Accidentally Deleted a Folder in Github and Can't Recreate It

Unlike your local operating system, Github deletes empty folders.

**Any time that a folder is empty, Github will automatically prune it.** In order to create a new folder, there must be a file in it. 

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

