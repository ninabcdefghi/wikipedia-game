# automated wikipedia game
finds the shortest connection between any two wikipedia pages. based on the [wiki-game](https://en.wikipedia.org/wiki/Wikipedia:Wiki_Game)

# installation 
```
pip install -r requirements.txt
```

in order to play, open "wikipedia-game.ipynb" in jupyter notebook, choose your config, edit start and goal page and run the game.

in case your country is censored and you cannot open the standard wikipedia URL, you can change the "base" variable in config to whereever you are accessing wikipedia from.

# sample output
```
LET'S GO: Starting to search the shortest connection between https://de.wikipedia.org/wiki/Ernst-Th%C3%A4lmann-Park 
and https://de.wikipedia.org/wiki/Unterhaltung_(Bauwesen)

Round 1 completed without results. Starting round 2.
Stay tuned - 4596 links searched, none matched the goal page so far...

DONE: The goal page https://de.wikipedia.org/wiki/Unterhaltung_(Bauwesen) can be reached with 2 clicks: 
https://de.wikipedia.org/wiki/Denkmalschutz connects https://de.wikipedia.org/wiki/Ernst-Th%C3%A4lmann-Park 
with https://de.wikipedia.org/wiki/Unterhaltung_(Bauwesen). 

In total, 5828 links were searched in 1.0 minutes.
```

# to do
- improve performance. ideas: enable parallel downloads of pages so it reaches the result quicker (threading, concurrent requests?)
- save and visualize the entire path from start to goal page (anytree? networkx?)
- add configs for different languages
- include an optional random wiki page generator
- shorten/split up the functions to make the code more readable
