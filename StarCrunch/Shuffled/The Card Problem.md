## Problem
I'm not sure how to implement cards. I was originally thinking about doing it the same way as I did in Forsaken, where each type of card gets instantiated and registered once, but now, I'm not sure if this is the best way. There is also the problem of recursive effects and listening for events in order when multiple cards are in play.

## Solutions
- [ ] Trigger/Effect system like [libreforge](https://github.com/Auxilor/libreforge).
- [ ] Custom event listener with custom priority.
	- No "listen to all" event type in Bukkit, meaning we'd have to listen to every event as cards need them.
	- Not very performant. e.g. we listen to something like a move event, we loop over every card in play, which is useless, especially if only one event requires the move event, just a waste.