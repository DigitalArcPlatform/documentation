---
title: Changing the Way Metadata Labels Display
layout: default
nav_order: 1
parent: Customizing the Jekyll Theme
grand_parent: Publishing Your Site
---

# Changing the Way Metadata Labels Display

You can change the labels that display in front of the metadata that's at the bottom of each item page. For example, if your community is multilingual, you can display metadata labels in several languages.

***Before you start***: Make sure you leave the field variable-name portion of the line (the part of each line before the colon) the same. Change only the field label (the part after the colon, in quotes).

The current file at `_data/metadata.yml` looks like this:

```
# Input or alter the string after each field to change how that item is displayed in metadata tables on each item page.
# You can create your own metadata attributes by following the model below. Note that any new groups will require modification of the html layout for items in order to display correctly.
fields: 
  title: "Title"
  creator: "Creator"
  contributor: "Contributor"
  creationdate: "Date"
  type: "Type"
  shortdesc: "Short Description"
  group: "Group"
  categories: "Categories"
  tags: "Tags"
  teammember: "Team Member"
  contributorquote: "Contributor Quote"
```

If you want to display metadata labels in both English and Spanish, your metadata.yml file might look like this:

```
# Input or alter the string after each field to change how that item is displayed in metadata tables on each item page.
# You can create your own metadata attributes by following the model below. Note that any new groups will require modification of the html layout for items in order to display correctly.
fields: 
	title: "Título/Title"
	creator: "Creador/Creator"
	contributor: "Colaborador/Contributor"
	creationdate: "Fecha/Date"
	type: "Tipo/Type"
	shortdesc: "Descripción corta/Short Description"
	group: "Grupo/Group"
	categories: "Categorías/Categories"
	tags: "Etiquetas/Tags"
	teammember: "Miembro del equipo/Team Member"
	contributorquote: "Cita del colaborador/Contributor Quote"
```