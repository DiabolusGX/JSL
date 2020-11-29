# JSL Bot
JSL Bot - Multipurpose discord bot

###### **Useful Links**
| [Invite Bot](https://bit.ly/jsl-default) | [Support Server](https://bit.ly/jsl-support) | [Vote JSL](https://bit.ly/jsl-bot) | [Trello](https://bit.ly/jsl-trello) |


[![Discord Bots](https://top.gg/api/widget/699505785847283785.svg)](https://top.gg/bot/699505785847283785)

-----

### Before you start
***Do not literally type out <> \[\] | etc. (Unless Mentioned)***
- **Aliases:** \[foo | bar\] means that you can use either foo or bar.
- **Optional:** \[foo\] means that this argument can be ignored.
- **Required:** \<foo\> means that you must use this argument for the command to work.
- ***If you want to remove config you changed, set it's value to `none` like `.booster message none`***
*Commands marked with*
- `*` can be unlocked for 12 hours after you [Vote JSL Bot.](https://bit.ly/jsl-bot 'Vote on top.gg')
- `**` can unly be used in NSFW channels.

### Setup
Starting with bot setup?

You can start with `.help setup` to see what configurations you can edit & you want to set.

**Note** : 
- *You can remove any config anytime by setting it's value to `none`*
  
    *ex : `.setup bot none` will remove bot channel.*

Name | Example | Usage
------- | ------------ | -------
prefix | `.setup prefix jsl.` | Sets new prefix. Prefix can't have *space*. 
bot channel | `.setup bot <channel>` | Only admins can use bot-commands outside *bot channel* If you don't want this, set value to `none`(default). You can mention the channel or use channel id.
welcome | `.setup welcome <channel>` | To get welcome messages when someone joins. Use `.help welcome` to edit welcome configs. You can mention the channel or use channel id.
mod channel | `.setup modchnl <channel>` | To get log of JSL Bot Moderation Command used. You can mention the channel or use channel id.
coins channel | `.setup general <channel>` | To enable [Economy Module](#Economy), members will get coins in this channel. You can mention the channel or use channel id.

-----

# Commands
Here are the categories the commands are divided in :
Click on category to get available commands with example and usage.
- [Utility](#Utility)
- [Fun](#Fun)
- [Music](#Music)
- [Other](#Other)
- [Economy](#Economy)
- [Mods](#Mod)

### Utility
Various utility commands and modules are one of the main features of JSL Bot.
Check the table to get available commands with their proper usage and examples.
Name | Example | Usage
------------ | ------------- | -------------
steam | `.steam <game \| user \| link \| groups \| play ...>` | Steam module is covered saperatly [Over Here](#Steam)
movie | `.movie now you see me` | Searches for available Moves. You can then respond with the `number` next to the result to get that Movie info.
tvshow | `.show Lucifer` | Searches for available TV Series. You can then respond with the `number` next to the result to get information on that TV Show.
trailer | `.trailer ` | Searches for available trailers on YouTube. You can then respond with the `number` next to the result to get YouTube URL of that Trailer.
booster | `.booster <message \| image \| role \| embed \| stats \| preview>` | Send custom message in [System Message Channel](https://prnt.sc/vrurxn) when someone boosts your server & add custom role. 
bin | `.bin <paste \| get> <Data \| Paste ID>` | You can easily save data to Pastebin and get an URL or get the data using the paste id (end part of url).
gif | `.gif celebration` | Sends a gif related to provided keyword else It'll send a random trending gif.
ascii | `.ascii <query>` | Convert your query to ascii-art.
reddit | `.reddit pcmasterrace` | Search a subreddit for you and returns a random popular post.
short | `.short https://top.gg/bot/699505785847283785` | Shorten the given URL.
image** | `.image steam` | Shows Image related to provided keyword.
urban** | `.urban bots` | Search your query on Urban Disctionary.

### Steam
Get steam game info, user info, recent played games, common games and friends that has perticular game.

You can start with `.steam setup` to make your profile privacy settings work with bot & other 3rd party websites.

- I suggest you to link your steam profile using `.steam link` so that users can diretly mention you instead of typing your steam url or steam user id.
- For `steam game` command You can respond with the `number`(1, 2, 3...) *next to the result* to get information about that game. 
   
    **OR** You can directly use `AppID` like `.steam game 1085660` to quickly get game info.


Name | Example | Usage
------------ | ------------- | -------------
user | `.steam user Y0kenB` | Shows you details of provided steam user.
owned | `.steam owned Y0kenB` | Shows owned games of provided steam user.
recent | `.steam recent Y0kenB` | Shows recently (last 14 days) played games.
groups | `.steam groups Y0kenB` | Shows all steam groups users has joined.
common | `.steam common DiabolusGX Y0kenB` | Shows *common owned* games of 2 users.
game | `.steam game Destiny 2` | Searches game on steam and shows you the available info.
link | `.steam link DiabolusGX` | Links your discord to your steam account.
play | `.steam play Destiny 2` | Shows list of your friends on steam that owns this game.
groupinfo | `.steam groupinfo ESL` | Shows you information available on mentioned steam group.

-----

### Music

- Make sure bot has requires permissions (i.e `JOIN`, `SPEAK`, `USE_VOICE_AVTIVITY`) in the Voice Channel hwere you want to listen to music :)
- The additional `.sound` command has some cool sound effects that you can play. 
- `.help sound` to see available sound effects and play like : `.sound drum-roll`

Bot will Join Voice Channel and leave as soon as song or soundeffect is over.


Name | Example | Usage
------------ | ------------- | -------------
play | `.play perfect` | Plays the song or playlist from youtube (including livestreams),  soundcloud, bandcamp, twitch, vimeo, mixer,  direct file links.
search | `.search moonlight` | Searches youtube for videos matching your query. You can then respond with the *number* next to the result to enqueue that result.
queue | `.queue` | Shows the queue, paginated and the full duration of the playlist.
np | `.np` | Shows the current song being played
skip | `.skip` | Skips if you have *DJ Role* or if you requested the song, voteskips otherwise.
pause | `.pause` | Pause the song.
resume | `.resume` | Resume the song.
loop | `.loop` | Switch b/w repeating the playlist and current song.
lyrics | `.lyrics` | Shows lyrics of currently playing song or the song you entered. You have to respond with the *number* to the result to get lyrics.
volume | `.volume 75` | Changes the volume between 1 and 100% (100 is pretty loud as you can probably tell)
leave | `.leave` | Disconnects the bot from the voice channel and clears the queue.

-----

### Economy

Economy module can be enabled from [Setup](#Setup) command.
- i.e `.setup general <channel>` You can mention the channel or use Channel ID.
- Users will get coins only in `general` channel.

Other available Economy Commands are : 

Name | Example | Usage
------------ | ------------- | -------------
cions | `.coins [user]` | Shows your or mentioned user's coins (if any).
pay | `.pay @DiabolusGX 2020` | Sends `x` coins to mentioned user's account.
work | `.work` | You can work every 12 hr and get upto 250 coins.
shop | `.shop <rep | chicken> [quantity]` | Buy reputation points or chicken to take part in cock-fight.
fight | `.fight 100` | Bets 100 on your chicken. You win & earn 100 else cock dies
buy | `.buy <1 | 2 | 3>` | Buy from server shop that you can setup using `.buysetup`
items | `.items [user]` | Shows your or mentioned user's inventory.
rep | `.rep @DiabolusGX` | gives 1 reputatation point to mentioned user.


To setup server shop (`.buysetup`) :
- To set name of 1st item : `.buysetup role1 name Epic Role`
- To set value/price of 1st item : `.buysetup role1 value 10000`
- To remove, set value to `none` like `.buysetup role1 name none`

**You can setup upto 3 items using `buysetup`**


-----
