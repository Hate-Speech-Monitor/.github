# Hate Speech Monitor

If you're looking for a way to monitor hate speech on your Discord server, look no further. 
This simple bot will help you keep track of all the hateful comments and messages on your server.

## Inspiration
Community platforms like Discord have a responsibility to protect their users from harassment and hate speech. We decided to use expert.ai's hate speech API to develop a bot that would help Discord moderators keep their servers clean and safe.

## What it does
The bot uses the expert.ai API to check every message that is sent on the server against a database of hate speech. If the message is classified as hate speech, the user is logged and the bots alerts the moderator.

## How we built it
The bot is build into discord using python and expert.ai hate speech detection API. the hate speech data from the discord server is logged into a mongodb database and it is viewed on a dashboard built using react

## Challenges we ran into
We faced challenges when trying to integrate expert.ai api with discord bot. Another challenge was to figure out how to create a REST API to access discord data simulatenouly with the bot running.

## Accomplishments that we're proud of
We are able to log hate speech on the discord server and rank user based on hate speech detected.

## What we learned
We learned to build a discord bot and integrate it with python backend to run hate speech detection

## What's next for Hate Speech Monitor for Discord
Next step would be to develop features to automatically flag users,delete hate speech message and take automated actions.
