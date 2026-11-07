You can try this on my [Project Test Drive](https://rmdrake.github.io/ryanmdrake/testdrive.html).

# NPC Tracker

A single-file HTML application for creating and tracking Non-Player Characters (NPCs) in tabletop role-playing games.

## Features

- **Character Management**: Create, edit, and delete NPC characters with name, class, level, HP, and notes
- **HP Tracking**: Visual HP bar with color indicators (normal, low health, critical)
- **Responsive Design**: Works on desktop and mobile devices
- **Local Storage**: All data persists in your browser
- **Import/Export**: Easily share character data with JSON files
- **Multiple Themes**: Choose from Space, Ocean, Desert, or Forest color themes
- **Dark Mode**: Support for both light and dark color schemes
- **Markdown Support**: Notes field supports Markdown formatting

## Usage

1. Fill in character details in the creator section
2. Use the HP adjustment controls to update character health
3. Navigate between characters using the dropdown menu
4. Export or import character data using the buttons in the header

The application runs entirely in your browser with marked.js dependency.

## Technical Details

This is a single-file HTML application with embedded CSS and JavaScript. It uses:
- localStorage for data persistence
- Marked.js for Markdown rendering
- Responsive grid layout for character cards
- Theme switching with CSS variables

## Files

- **npctrack.html**: The WebApp, just open in a browser
- **npc_characters.json**: A file containing example characters that can be imported for instant gratification.
- **plan.md**: The development plan used for guiding AI assistance.

