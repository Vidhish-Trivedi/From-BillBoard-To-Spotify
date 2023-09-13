# From-BillBoard-To-Spotify
## Features
- A terminal-based application which creates playlists of top 100 songs according to Billboard on Spotify.  
- This program takes a date as input from the user, then using Beautiful Soup, it scrapes the Billboard hot-100 songs for the week with that date.  
- Using the data collected, the program then searches spotify for those songs and adds them to a playlist linked to the user's account (Authorization Required!).

## Requirements and Running the Project
- The project uses the following libraries as dependencies (can be sourced from https://pypi.org/)
    - bs4 (BeautifulSoup)
    - spotipy (https://pypi.org/project/spotipy/)
    - os (usually part of Python 3.x installations)
    - requests (usually part of Python 3.x installations)
    - dotenv (to load environment variables)

- Before you can use the application, you will need to create an application on the Spotify developer's portal (https://developer.spotify.com/).
- To allow the program to create a new playlist in your account, you will need to set up a `.env` file in the project root as follows:
```
    CLIENT_ID=YOUR_SPOTIFY_CLIENT_ID
    CLIENT_SECRET=YOUR_SPOTIFY_CLIENT_SECRET
```

- Once the dependencies are installed and the environment variables are set, you can run the game by:
```
python main.py
```

## Scope For Improvement
- The project currently uses a very naive match of deciding if two songs are similar, this can be improved upon.

## Authors
- [@Vidhish-Trivedi](https://github.com/Vidhish-Trivedi)
