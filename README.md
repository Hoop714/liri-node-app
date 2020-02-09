# LIRI Node App

---

Welcome to the LIRI Node App! LIRI is the sister to Apple's SIRI App. While SIRI is a Speech Interpretation and Recognition Interface, LIRI is a **Language** Interpretation and Recognition Interface. 

LIRI allows a user to input a command and returns the information that the user is requesting. There are four commands the user may input. Each command is described below.

---
## LIRI Commands

1. **Concert-This**: user inputs a band name/artist into the command line following the concert-this argument. The Axios node module then sends a request to the Bands In Town API. A list of all upcoming concerts for that artist will be returned. If no band name/artist is entered, a message will be received notifying the user. If there are no upcoming events for the artist, the user will be notified as well.

*Command line input*: node liri.js concert-this <'band/artist'>

*Example*:
![image1](https://github.com/Hoop714/liri-node-app/blob/master/images/concert-this.PNG?raw=true)

2. **Spotify-This-Song**: user inputs a song name into the command line following the spotify-this-song argument. The Node-Spotify-API module sends a request to the Spotify API. Information about the song will be returned. If no song is added to the command line, information for 'The Sign' by Ace of Base will be returned. 

*Command line input*: node liri.js spotify-this-song <'song name'>

*Example*:

3. **Movie-This**: user inputs a movie into the command line following the movie-this argument. The Axios node module then sends a request to the OMDB API. Information about the movie will be returned. If no movie is entered into the command line, the information for 'Mr. Nobody' will be returned. 

*Command line input*: node liri.js movie-this <'movie name'>

*Example*:

4. **Do-What-It-Says**: user does not need to input an argument following the do-what-it-says argument. This function sources the random.txt file for a song name. After the information from random.txt is grabbed, the spotify-this-song function is called. Information about the song on the random.txt file is returned.

*Command line input*: node liri.js do-what-it-says

*Example*:


---
## Technologies Used

1. Javascript
2. JSON
3. Multiple Node Modules
   * Node-Spotify-API
   * Axios
   * Moment
   * DotEnv
4. Bands In Town API
5. OMDB API


