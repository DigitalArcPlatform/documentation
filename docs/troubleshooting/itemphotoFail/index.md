---
title: "The Photo of My Item Isn't Rendering As Intended"
layout: default
nav_order: 3
parent: Troubleshooting
---

# The Photo of My Item Isn't Rendering As Intended

Check to make sure you have consistent naming in the .md file and the photo file. It's easy to put a hyphen in one file name and an underscore in another:

	File-name.md
	File_name.jpg
	
Because of the underscore in the `File_name.jpg`, the computer will see these as two different items.

# My items aren't showing up in the right order

Items are sorted by alphanumeric order based on the .md file name: Numbers before letters, punctuation before numbers.

Numbers will sort by alphabet, so "1" will be immediately followed by "10", where "01" will sort before "02", and so on to "10". Adding the extra zero before the 1 will let you sort numbers in order up to 99. If you have 100 objects, you'll want two zeroes before single-digit numbers and one zero before double-digit numbers.


