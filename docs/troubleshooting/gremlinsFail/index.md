---
title: "There are Weird Characters On My Page"
layout: default
nav_order: 5
parent: Troubleshooting
---

Several kinds of characters can create issues.

- If you see a weird black-outlined box instead of an actual character, you might have a file with an emojis, characters with accents (cedillas, acute and grave, etc.), or a file written in languages that make use of characters beyond the 26-letter English alphabet. Using "UTF-8" characters can help. Check this [UTF-8 Character List](https://www.w3schools.com/charsets/ref_utf_reference.asp) for a copy-paste of a wide variety of characters that will display propelrly inst

- Note that markdown is sensitive to certain characters, in particular: `:`, `#`, `*`, `-`, and `` ` ``. If you have recently made a change involving any of these characters, make sure that this is intended and, if so, that you have properly escaped the character with either a backtick `` ` `` or backslash `\`. 

- Curvy quotes and curvy apostrophes need to be replaced with straight double quotes and single apostrophes.

