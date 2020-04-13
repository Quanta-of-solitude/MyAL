# MyAL

This is used to  scrape data from My Anime List site (https://myanimelist.net/). Used to get data to implement in anime search results, as well as get description after performing  valid search.


# Functions

- animeData("Anime Name") : Returns the anime data as a dictionary
- animeSearch("Anime Name") : Search for the valid anime result name (shows top 7 names)

## Installation (https://pypi.org/project/MyAL/0.3/)
```
pip install MyAL
```

## Requirements
- beautifulsoup4
- requests

## USAGE

```python
import MyAL

data = MyAL.MALdata()
datas = data.animeData("Naruto")

print(datas)
```

## OUTPUT

```python
{'users': '877,205 users', 'rating': '7.88', 'rank': 'Ranked #709', 'inf': ["Moments prior to Naruto Uzumaki's birth, a huge demon known as the Kyuubi, the Nine-Tailed Fox, attacked Konohagakure, the Hidden Leaf Village, and wreaked havoc. In order to put an end to the Kyuubi's rampage, the leader of the village, the Fourth Hokage, sacrificed his life and sealed the monstrous beast inside the newborn Naruto.\n\r\nNow, Naruto is a hyperactive and knuckle-headed ninja still living in Konohagakure. Shunned because of the Kyuubi inside him, Naruto struggles to find his place in the village, while his burning desire to become the Hokage of Konohagakure leads him not only to some great new friends, but also some deadly foes.\n\r\n[Written by MAL Rewrite]"], 'add': ['Episodes:  220  \nAired:  Oct 3, 2002 to Feb 8, 2007  \nBroadcast:    Thursdays at 19:30 (JST)      '], 'image': 'https://cdn.myanimelist.net/images/userimages/thumbs/11081_thumb.jpg?t=1575939600'}
```

