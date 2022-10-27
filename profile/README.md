# Hate Speech Monitor

If you're looking for a way to monitor hate speech on your Discord server, look no further. 
This simple bot will help you keep track of all the hateful comments and messages on your server.

## Inspiration
Community platforms like Discord have a responsibility to protect their users from harassment and hate speech. We decided to use expert.ai's hate speech API to develop a bot that would help Discord moderators keep their servers clean and safe.

## What it does
The bot uses the expert.ai API to check every message that is sent on the server against a database of hate speech. 
1. If the message is classified as hate speech, the user is logged and the bot alerts the moderator. 
2. The bot provides a command to list all the people with the highest offensive language usage in order of severity to make it easier for moderators to deal with them.
3. We also maintain a dashboard where we can view the same information + an additional breakdown of offences. For every user, the dashboard shows the kind of offence and the number of times it has been committed. 

## How we built it
The bot is built into discord using Python (discord.py) and Expert.ai Hate Speech Detection API. The hate speech data from the discord server is logged into a MongoDB database and it is viewed on a dashboard built using React through a backend server built using Flask.

## Challenges we ran into
1. Integrating Expert.ai API with the Discord bot.
2. Creating and running a Flask server that can combine data from Discord Client and MongoDB. 

## Accomplishments that we're proud of
1. We are able to log hate speech on the discord server and rank users based on hate speech detected.
2. We are able to view these reports through a database that makes it easier to detect and deal with the most serious offenders.

## What we learned
We learned to build a discord bot and integrate it with the Python Flask  backend to run hate speech detection

## What's next for Hate Speech Monitor for Discord
The next step would be to develop features to  : 
1. Automatically flag users
2. Delete hate speech messages and take automated actions
3. Send notifications to server admins regarding activity in the server
4. Refine the dashboard authentication to grant access to viewing the data to only authorized people of a server (admins, owners, mods, etc)
5. Expand content scanning to images, gifs, audio, etc
