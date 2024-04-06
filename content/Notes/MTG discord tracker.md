
### Goals
- Create a discord bot that can sit in discord video calls and display the following information **via a dynamic website:**
	- Display the board of whoever's turn it is
	- Overlay important variables like life and counters
	- Provide controls to the player whose turn it currently is
		- Deal damage or commander damage to player
		- Similar to how playgroup.gg handles it
		- Pass turn

### Scope
- Most important features
	- Display screen of current player
	- Have way to declare winner, either through website or discord bot controls
### APIs
- Discord
	- Can video streaming be relayed outside of discord?
	- Might be impossible to display in a separate web app - will look into
- Scryfall
	- Can easily fetch info on cards
	