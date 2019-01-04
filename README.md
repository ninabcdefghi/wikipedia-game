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
LET'S GO: Starting to search the shortest connection between https://de.wikipedia.org/wiki/Ernst-
Th%C3%A4lmann-Park and https://de.wikipedia.org/wiki/Kabinettsorder

Round 1 completed without results. Starting round 2.
Stay tuned - 2794 links searched, none matched the goal page so far...

DONE: The goal page can be reached with 2 clicks.

This is the path: Ernst-Thälmann-Park ---> GASAG ---> Kabinettsorder
```

# to do
- include an optional random wiki page generator
- shorten/split up the functions to make the code more readable
