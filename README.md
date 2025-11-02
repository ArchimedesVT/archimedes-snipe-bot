# Archimedes Snipe Bot

SnipeBot by Archimedes
Official Discord Bot Documentation
Updated August 2025


1. Overview
About
SnipeBot counts and sorts “snipes” (images with tagged users). This is achieved by reading the channel history of the snipe channel from the most recent message up to a hard-coded start date. This method is preferred over live leaderboard updates to account for message edits and deleted messages easily.

Contact Info
SnipeBot is developed and maintained by the Archimedes developer team. Ping the developer role on Discord for immediate support.

2. Commands
/help
Provides an overview of sniping and links this document.
/rules
Responds with sniping rules.
/leaderboard <filter>
Generates and responds with the current leaderboard.
Filters:
sniper (or no filter): Displays the top ten members with the most snipes.
sniped: Displays the top ten members who have been sniped the most.
all: Displays entire leaderboard, sorted by most snipes.
kd: Displays the top ten members with the highest kill/death ratio. An undefeated status is denoted by “UD”.
teams: Displays the top teams, including leadership and alumni, sorted by most snipes. This count includes friendly-fire snipes. 
duos: Displays the top ten member pairs with the most snipes of each other.

/cache
Generates and stores the leaderboard to memory from the set start date. When /leaderboard is used, it will update the leaderboard stored in memory. The purpose of this command is to speed up leaderboard generation.
If prompted with a memory error, use this command.
If the output of /leaderboard is slow, use this command.

3. Developer Guide
Source Code
GitHub: Please commit all changes to the SnipeBot public repository.
To update the bot with new code:
Commit changes.
Use git push in your terminal.
Restart the bot from the Cybrancee dashboard.
Once the Cybrancee server has restarted, use /cache in the snipe channel.

Cybrancee 24/7 Hosting
Discord does not offer 24/7 hosting. In that case, Cybrancee, a third-party hosting site, is used.
Cybrancee services cost $1.49 per month. Remember to cancel or update the payment information after every spring.

Modifying Bot Code
SnipeBot uses discord.js, a Node.js module for Discord bots. Modifying code is easy for anyone familiar with JavaScript and GitHub integration.
Updating bot code is reserved for the developer committee only. To make a request, ping a developer. If you are part of this committee and would like to modify the code, follow these steps to gain the necessary access:
Ask a current developer to add you to the Archimedes Systems Discord Developer Team. When your request is approved, you will be able to access bot settings at discord.com/developers/applications 
For current cred, ask the webmaster.
