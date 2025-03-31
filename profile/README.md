# Pena Discord Bot

Pena is a Discord bot that allows users to create, share, and manage sound panels in their Discord servers. It provides an easy way to organize and play various types of sounds like music, game sounds, fun sounds, and movie clips.

## Features

- Slash command support
- Sound panel creation and management
- Multiple sound types (Music, Game, Fun, Movie)
- Server panel integration
- Easy sound management
- Search functionality
- Detailed panel information
- User-friendly interface

## Commands

### Panel Management
- `/create-panel` - Create a new sound panel
  - `name`: Panel name
  - `description`: Panel description
  - `type`: Panel type (Music, Game, Fun, Movie)
- `/delete-panel` - Delete a panel
  - `panel_id`: ID of the panel to delete
- `/edit-panel` - Edit panel information
  - `panel_id`: ID of the panel to edit
  - `name`: New panel name
  - `description`: New panel description
  - `type`: New panel type
- `/panel-rename` - Rename a panel
  - `panel_id`: ID of the panel to rename
  - `new_name`: New name for the panel
- `/panel-info` - View detailed panel information
  - `panel_id`: ID of the panel to view

### Sound Management
- `/add` - Add new sound to panel
  - `panel_id`: ID of the panel to add sound to
  - `name`: Sound name
  - `url`: Sound URL
  - `type`: Sound type (Music, Game, Fun, Movie)
- `/delete-sound` - Delete sound from panel
  - `panel_id`: ID of the panel containing the sound
  - `sound_id`: ID of the sound to delete
- `/sound-rename` - Rename a sound
  - `panel_id`: ID of the panel containing the sound
  - `sound_id`: ID of the sound to rename
  - `new_name`: New name for the sound
- `/add-to-server` - Add panel to your server
  - `panel_id`: ID of the panel to add

### Viewing Commands
- `/my-panel` - View your panels
  - `type`: Filter panels by type (optional)
- `/server-panel` - View server panels
  - `type`: Filter panels by type (optional)
- `/search` - Search for panels and sounds
  - `query`: Search query
  - `type`: Filter by type (optional)
- `/panels` - List all panels
  - `type`: Filter panels by type (optional)
- `/help` - Display help message

## Installation

1. Clone the repository:
```bash
https://github.com/PenaBOT/Pena.git
cd pena-bot
```

2. Install required packages:
```bash
npm install
```

3. Create and configure `.env` file:
```
DISCORD_TOKEN=your_bot_token_here
MONGODB_URI=your_mongodb_uri_here
```

4. Start the bot:
```bash
npm start
```

## Usage

1. Invite the bot to your server with required permissions
2. Create a new panel using `/create-panel`
3. Add sounds to your panel using `/add`
4. Share your panel with others using `/add-to-server`
5. View and manage your panels using various commands
6. Search for panels and sounds using `/search`

## Requirements

- Node.js v16.9.0 or higher
- Discord.js v14
- MongoDB
- Discord Bot Token
- Required Discord Bot Permissions:
  - Send Messages
  - Embed Links
  - Attach Files
  - Connect
  - Speak
  - Use Voice Activity

## Support

If you encounter any issues or have questions, please create an issue in the GitHub repository.

## License

This project is licensed under the MIT License - see the LICENSE file for details. 
