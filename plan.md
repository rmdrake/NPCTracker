# Single File HTML Application Plan

## Project Overview
Create a single file HTML application with embedded CSS and JavaScript that serves as a NPC character tracker for tabletop RPG games.

## Application Requirements
- Opens in modern web browsers
- Beautiful design
- Character creator
- Ability to add, edit, and remove characters
- Character management (id, name, class, level, maxHP, HP, Notes)
- Responsive design that works on full screen desktops and mobile devices
- Must have a layout that adjusts to the width of the browser to maximize display space
- Local storage persistence for character data
- Pull down menu that lists characters by name and jumps to their card when selected
- Character cards without scroll bars
- Visual indicators for character status (half HP orange, quarter HP red, 0 or less HP dark shading + strikethrough)
- Interactive HP adjustment controls
- Support HP values greater than maxHP and less than 0
- HP bar that shows integer percentage of HP
- Notes text field that supports markdown
- Notes shown as rendered markdown in character cards
- Alphabetical sorting of characters
- Import and export character data to/from JSON files
- Import from json file to add characters to existing list and ensuring unique id
- Export to json file
- Dark Mode support
- Dark mode toggle

## Main Layout
Top (Sticky Header)
- Title, Table of contents pull down, Return to Top Button (Left Aligned)
- Import Button, Export Button, Delete All Button, Color Theme pull down, Dark Mode Button (Right Aligned)

Center (Adjusts to screen width)
- Character Creator
	+ Name Text Box, Class Text Box, Level Number Box, Current HP Number Box, Max HP Number Box
	+ Notes Text Field (Vertically adjustable)
	+ Save Button, Cancel Button

Bottom
- Character Cards (Cards adjust to fill screen width and try to maintain width of 550 to 640 px)
	+ Name (Left Aligned), Level (Right Aligned)
	+ Class
	+ HP / MaxHP
	+ HP Display Bar
	+ buttons for: -10 HP -1 HP, +1 HP, +10 HP
	+ Notes displayed in markdown (Top Aligned) (Height of card expands to fit contents)
	+ Edit (Lower Left Aligned), Delete (Lower Right Aligned)

## Color Themes
- Four main Color Themes
    + Space: a grey theme (Default)
    + Ocean: a blue theme
    + Desert: a brown and orange theme
    + Forest: a green theme
- Colors must respect and be aesthetic to both light and dark modes.

## Import Export
Character data must be encapsulated in json for import and export using the exact following data structure as an example:
{
    "id": "",
    "name": "",
    "class": "",
    "level": 0,
    "maxHP": 0,
    "HP": 0,
    "notes": ""
},

## File Structure
- Single HTML file with embedded CSS and JavaScript
- All code contained in one file
- Marked.js allowed for Markdown Rendering
