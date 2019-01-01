# automated wikipedia game
finds the shortest connection between any two wikipedia pages. based on the [wiki-game](https://en.wikipedia.org/wiki/Wikipedia:Wiki_Game)

# installation 
```
pip install -r requirements.txt
```

in order to play, open "wikipedia-game.ipynb" in jupyter notebook, select a (for now only German) start and goal page in the config and run the game.

in case your country is censored and you cannot open the standard wikipedia URL, you can change the "base" variable in config to whereever you are accessing wikipedia from.

# sample output

```
LET'S GO: Starting to search the shortest connection between https://de.wikipedia.org/wiki/Zeitzone 
and https://de.wikipedia.org/wiki/Februarumsturz

Round 1 completed without results. Starting round 2.

DONE: The goal page https://de.wikipedia.org/wiki/Februarumsturz can be reached with 2 clicks: 
https://de.wikipedia.org/wiki/Tschechien connects https://de.wikipedia.org/wiki/Zeitzone with
https://de.wikipedia.org/wiki/Februarumsturz.
```

# to do
- improve performance, it is really slow! ideas: enable parallel downloads of pages so it reaches the result quicker (concurrent requests?)
- print out the number of interrogated websites every n seconds
- save and visualize the entire path from start to goal page (anytree?)
- add configs for different languages
- create a random wiki page generator
- shorten/split up the functions to make the code more readable
- make output look nice...
