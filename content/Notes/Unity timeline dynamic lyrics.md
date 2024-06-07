Summary
- Timestamped lines and words that sync up with lyrics
- Full line appears at once, left-to-right fade shows 

Data structure
- Line array
	- Timestamp the line should appear at
	- Transition style to next line (fade / wipe / etc)
	- Word array
		- Timestamp the word should appear at
		- Ease function 
		- Visual effect when word is reached (punch / screenshake / flames / etc)

Hurdles
- Need an efficient system for placing word timestamps
	- First idea: Use unity timeline to align functions
		- Not that readable at runtime
		- Would need to read 2 at a time to know how to perform the ease function properly
	- Hard-code ahead of time?
		- Not really that effective
		- Timeline feature in something like FL studio
		- Slow and tedious having to write everything down
	- MIDI data
		- Easy to read from FL
		- One single note would be enough to dictate where note starts and ends
		- Doesn't handle easing functions + transitions + visual effects
	- Standalone custom application
		- Node or unity
		- If done in unity: provides live demo of how it looks

Mockup

![[Pasted image 20240503004352.png]]