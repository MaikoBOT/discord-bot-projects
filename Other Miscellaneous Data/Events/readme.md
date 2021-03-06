# Retrieve the user who unreacted a reaction!

This event does exactly what the name states! This custom event will run when the user unreacts an reaction and saves it to a useable DBM variable for later use. You can also have actions runned alongside the event!  

![Gif Preview](https://thumbs.gfycat.com/TotalObedientLeafcutterant-size_restricted.gif)

_**DO NOT MODIFY THE EVENT TRIGGER IF YOU DON'T KNOW WHAT THE HECK YOU'RE DOING!**_  

# FAQ

Q. The second time I unreact, the bot doesn't register it!  
A. That seems to be a problem, however you can warm the listeners up by reaction/unreacting it.  

Q. Where do i put my actions when someone unreacts?!?  
A. Go to the `MessageReactionRemoved` event and you can add your own actions between the arrows indicated.  

Q. Is this compatible with Wrex's `On Non-Cached Reactions`?  
A. Yes! This has been tested and seems to work fine with reactions on old messages. Remember, it's faster once it's cached.  

Q. I got this error message: `MaxListenersExceededWarning: Possible EventEmitter memory leak detected. x messageReactionRemove listeners added. Use emitter.setMaxListeners() to increase limit`. Should I be concerned?  
A. This message comes from the Node.JS engine and should only appear once per bot session. This warning just shows that there are a lot of listeners active and has been capped at a certain limit.  

# Lists of outputtable variables.

The following variables will be outputted:

 - Temp Variable  
	• `rediEvent.MemberID` 		- Returns the UserID of the person who unreacted.  
	• `rediEvent.Member` 		- Returns the Member Object. This variable can be used in the `Store Member Info` source variable.  
	• `rediEvent.ReactionObj`	- Returns the Reaction Object. This variable can be used in the `Store Reaction Info` source variable.

Note: `rediEvent.Member` returns a GuildMember class. This means that you can do anything server related to this variable such as banning, nicking, add roles/del roles etc.
