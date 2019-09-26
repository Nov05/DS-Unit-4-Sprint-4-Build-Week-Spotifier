# Data Science

Nov05/flask-spotify    
forked from Build-Week-Spotify-Song-Suggester/Data-science   
DS Unit 4 Sprint 4 Build Week Spotify   

## :point_right: Go to the app   
https://spotifier-app.netlify.com/     
https://5d8c991142a75800078cbcb4--spotifier-app.netlify.com/

## :point_right: Marketing page   
https://spotifier.netlify.com/    

【Note】     
Some of the songs in the app database are no longer active on Spotify, some might not be available in the area you are now. So far in the US, the following songs are playable through the app.     
**An Ember In The Ashes (ASOT 874)**      
**Old Town Road**    
**Waiting for U**    
etc.    
<img src='https://github.com/Nov05/pictures/blob/master/pic001/2019-09-26%2010_19_59-Microsoft%20Edge.jpg?raw=true' width=700>  

## Architecture

React Frontend + Java Backend + PostgreSQL on AWS  

## Deliverables  

Build Week repo      
https://github.com/Build-Week-Spotify-Song-Suggester    
Plotly 3D Scatter Notebook (by Josh Fowlkes)      
https://plot.ly/~beyond_brawn/1/running-the-model/#/    
<img src="https://github.com/Nov05/pictures/blob/master/gifs/ezgif.com-video-to-gif.gif">  
PostgreSQL database hosted on AWS (by Nov05)     
<img src="https://github.com/Nov05/pictures/blob/master/pic001/2019-09-26%2013_37_58-Microsoft%20Edge.png?raw=true">   

## Project   

**PROJECT NAME**  
Spotify Song Suggester

**PITCH**   
Build an app to enable users to browse and visualize audio features of over 116k spotify songs.

MVP: User can search for a specific song and see its audio features displayed in a visually appealing way. The app also identifies songs with similar audio features.

Stretch goal: The app hits the Spotify API to enable the user to search for any song on the platform.

**MVP**  
DS:     
- Build a model to recommend songs based on similarity to user input (I like song x, here are n songs like it based on these similar features)  
- Create visualizations using song data to highlight similarities and differences between recommendations.  

**Web:**  
- user registration/login flow  
- User can save their favorite songs to their profile in the Web backend
- Once the user has their favorites saved the DS API can make suggestions based on the audio features of their favorites.
- User can request suggested songs based on what they are in the mood for ( acousticness, danceability, duration, energy, etc)
- User can edit and delete their favorites.  

**STRETCH**  
DS:
- Create animations of your visualizations
- Highlight commonalities across the X most popular songs in the dataset

Web:
- When the user has a large number of favorites, find a way to visualize the audio features the user likes the most in an attractive way.

**DESIGN LINKS / DATA SETS**   
Dataset: https://www.kaggle.com/tomigelo/spotify-audio-features  

**TYPE**  
Data Science Hybrid Apps  
**DATA ENGINEER**  
Harsh Desai  
Josh Fowlkes  
**MACHINE LEARNING ENGINEERS**  
*
**WEB UI DEVELOPER**  
Theresa Jackson  
**WEB REACT I**  
Dylan Mestyanek  
Johnathan Shoff  
Uzoamaka Grace Anyanwu  
**WEB REACT II**  
Matthew Masters  
**WEB BACKEND (JAVA)**  
Vicky Yue  
Preston Middleton  

## Logs 

2019-09-23 repo forked   
2019-09-26 app components hosted and ingegrated    

## Information  

Plotly Dash Live Updating Components   
https://dash.plot.ly/live-updates

Integrate Plotly Dash Into Your Flask App    
https://hackersandslackers.com/gaining-full-control-over-plotly-dash/   

https://gobrief.com/   
free unlimited time zoom calls so you dont have to restart every hour   

https://airtable.com/shrXJLrenkHpSRWiV/tbln1vdyJbN0Nmte5  
build week project list   

Reference repo   
https://github.com/bw-spotify/data-science

Backend endpoints   
Vicky Yue:21-red: 03:18   
```
----- E N D P O I N T S -----   
Endpoints that do not say ‘No Auth Required’ or Log In/Register/Log Out will all require authentication
Register   
POST - https://spotify-song-suggester.herokuapp.com/createnewuser   
--- parameters ---   
- username   
- password   
*Log In*   
GET - https://spotify-song-suggester.herokuapp.com/login   
--- takes in ---   
- username   
- password   
Log Out   
GET - https://spotify-song-suggester.herokuapp.com/oauth/revoke-token   
Get All Tracks (for testing) - No Auth Required   
GET - https://spotify-song-suggester.herokuapp.com/tracks/tracks   
- Limit 10 per page   
Get Track By Name (trackid) - No Auth Required   
GET - https://spotify-song-suggester.herokuapp.com/tracks/track/{name}   
Save/Favorite Track by Name (trackid)   
POST - https://spotify-song-suggester.herokuapp.com/tracks/save/{trackid}   
Get User’s Saved/Favorited Tracks   
GET - https://spotify-song-suggester.herokuapp.com/tracks/savedtracks   
Get Suggested/Recommended Tracks by Name (trackid) - No Auth Required   
GET - https://spotify-song-suggester.herokuapp.com/tracks/recs/{trackid}   
- returns 10 similar songs with song details   
Remove Song From Saved/Favorited   
DELETE - https://spotify-song-suggester.herokuapp.com/tracks/remove/{trackid}   
```   
    
    
