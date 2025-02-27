---
layout: default
title: Patch Notes
permalink: /patch-notes
menu: About
num: 1
type: fullpage
---

#### LioranBoard 2 2022.3.0 CE

###### New Features
- Delete key works in text boxes [Roadie]
- Added option to select a secondary Twitch Client ID [Silverlink] - this is an optional setting for now, but will be required in the future, which will require you to relink Twitch accounts and re-duplicate channel points made with LioranBoard
- Transmitter updated to V6. You can keep using V5 if you do not use the new secondary Twitch Client ID [Christina]
- Added the option to reveal Transmitter in File Explorer [Christina]

###### Improvements
- Automatic Updating works again and is safe to use (only for version 2022.3.0 and up). Huge thanks goes to [Roadie]
- Changed Get HTTP Request to HTTP Request, since it supports other methods too [Christina]
- Changed version formatting to 2022.X.X [LB2 dev team]
- Twitch Scam Train renamed to Twitch Hype Train [Christina]
- Get Twitch Connection command now accepts empty box for Account login name, which will default to the main Twitch account if left empty [Christina]
- Confirmation message for copying multiple commands [wolbee]
- Cleaner Trigger Pull Data dropdown [Sebas]
- Cleaner and additional OBS Triggers [Sebas]
- Due to Twitch Prediction outcomes changing from 2 to 10, the following has changed [Christina]:
	The old Twitch: Create Prediction command was renamed to Twitch: Create Prediction 2 Outcomes (all your previously made commands will still work)
	Added new Twitch: Create Prediction command that accepts an array of outcomes (max 10)
	Get Latest Poll/Prediction command can now retrieve Prediction Outcome 1-10 ID
	Trigger Pull Data command can now retrieve Outcome 1-10 Info
- Made commands that have default JSON code in text boxes taller so the code can be seen [wolbee]

###### UI Changes
- Changed the LB2 icon [LB2 dev team]
- Added default channel to the Channel label in the Twitch Chat Message command, to show which channel the message will be sent to if the channel name is left empty [Christina]
- Text/Label modifications, including clearer descriptions, spelling checks etc. [Christina]
- Changed input box names to better reflect what should be put into them: [Christinna]
	Save Variable As => save the result into a new or existing variable
	Added ms, s, db etc. to relevant boxes 
- Added donation, Discord and documentation buttons [Christina & wolbee]
- Changed copy command icon to the regular copy icon (originally scissors) [Silverlink]
- Changed move command icon to something more recognisable [wolbee]

###### Bug Fixes
- Fixed a bug that stopped you from resizing the text box and changing extension box color when sending extension commands from Transmitter [Christina]
- Fixed a bug with overlappable, non-persistent, non-queuable buttons not working if triggered with the Trigger Button command. [Christina] 
- Fixed a bug where the Command Line command would not show under Windows commands [Christina]
- Fixed a bug that defaulted Fetch OBS Data and Custom Packet to OBSws5 syntax [wolbee]
- Fixed YouTube crash for Member renewal events [Christina]
- Fixed clipboard clearing on LioranBoard start up (only works for text, images still get cleared) [Christina]
- Fixed Get Variable Type command returning undefined for any button variables (which are all objects) [Christina]
- Fixed ini files not properly getting .ini appended when the file name is 3 letters long [Christina]
