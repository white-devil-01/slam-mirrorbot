# A Guide On How To Customise Bot Further for Personal Use.

1. [Customising Bot /start Message](https://github.com/breakdowns/slam-mirrorbot/blob/master/modificaton.md#Customising-Bot-start-Message)
2. [Changing Bot Commands](https://github.com/breakdowns/slam-mirrorbot/blob/master/modificaton.md#Changing-Bot-Commands)
3. [Changing Max Allowed Downloads & Set Auto Cancel Time If No Seeders Available](https://github.com/breakdowns/slam-mirrorbot/blob/master/modificaton.md#Changing-Max-Allowed-Downloads-and-Set-Auto-Cancel-Time-If-No-Seeders-Available)
4. [Customising Bot Message When Bot Auto Cancels the Torrent Due to No Seeders are Available](https://github.com/iamLiquidX/MirrorX/blob/master/modificaton.md#Customising-Bot-Message-When-Bot-Auto-Cancels-the-Torrent-Due-to-No-Seeders-are-Available)
5. [Customising Bot Stats Message](https://github.com/breakdowns/slam-mirrorbot/blob/master/modificaton.md#Customising-Bot-Stats-Message)
6. [Customising Mirror Status](https://github.com/breakdowns/slam-mirrorbot/blob/master/modificaton.md#Customising-Mirror-Status)
7. [Customising Mirror Progress Bar](https://github.com/breakdowns/slam-mirrorbot/blob/master/modificaton.md#Customising-Mirror-Progress-Bar)
8. [Customising Bot status Message](https://github.com/breakdowns/slam-mirrorbot/blob/master/modificaton.md#Customising-Bot-status-Message)
9. [Customising Bot After Download Complete Message](https://github.com/breakdowns/slam-mirrorbot/blob/master/modificaton.md#Customising-Bot-After-Download-Complete-Message)


# Customising Bot /start Message
:octocat: In Order to Customise Bot Start Message You have to Edit few lines in `__main__.py` file. 

You Can Find `__main__.py` File Here ⬇️
```
slam-mirrorbot/bot/__main__.py
or
https://github.com/breakdowns/slam-mirrorbot/blob/master/bot/__main__.py
```
In Order to Customise the way you want the start Message of Bot,  modify  `line 47` & `line 48` from `__main__.py` file 

🔗 [Line 47 can be Opened from here](https://github.com/breakdowns/slam-mirrorbot/blob/d598144f752a3412da22977b5db88e7169792ae3/bot/__main__.py#L47)


# Changing Bot Commands
:octocat: In Order to Customise Bot Commands, You have to Edit Commands in `bot_commands.py` File.
You Can Find `bot_commands.py` File Here ⬇️
```
slam-mirrorbot/bot/helper/telegram_helper/bot_commands.py
or
https://github.com/breakdowns/slam-mirrorbot/blob/master/bot/helper/telegram_helper/bot_commands.py
```

# Changing Max Allowed Downloads and Set Auto Cancel Time If No Seeders Available
:octocat: In Order to Change Max Allowable Torrents at a Time & Auto Cancel If No Seeders are Available, You Have to Edit `aria.sh` file

### Max Allowed Downloads
You can limit maximum concurrent downloads by changing the value of `MAX_CONCURRENT_DOWNLOADS` in `aria.sh` file. By default, it's set to 7
### Auto Cancel a Torrent 
You can Set the Bot to Auto Cancel a Torrent, If No Seeders are Available by changing the value of `--bt-stop-timeout` in `aria.sh` file. By default, it's set to 1200. ( It means after 1200 Seconds, Torrent will get Auto Cancelled)
### If You Don't want the Bot To Auto Cancel The Torrent If No Seeders Availabe

You Have to remove  `--bt-stop-timeout=1200` from `Line 77` in `aria.sh` file.

🔗 [Line 17 Can be Opened from Here](https://github.com/breakdowns/slam-mirrorbot/blob/d598144f752a3412da22977b5db88e7169792ae3/aria.sh#L7)

# Customising Bot Message When Bot Auto Cancels the Torrent Due to No Seeders are Available
:octocat: In Order to edit Bot Auto Cancel Message, You Have to Edit `aria2_download.py` file.

You Can Find the `aria2_download.py` file Here ⬇️

```
slam-mirrorbot/bot/helper/mirror_utils/download_utils/aria2_download.py
or
https://github.com/breakdowns/slam-mirrorbot/blob/master/bot/helper/mirror_utils/download_utils/aria2_download.py
```
The Line Which You Have to Edit is `Line 65` 
🔗 [Line 66 can be opened from here](https://github.com/iamLiquidX/MirrorX/blob/097a69e3b7aa7e8aad0c91de8b07877933ef6f34/bot/helper/mirror_utils/download_utils/aria2_download.py#L65)

# Customising Bot Stats Message
:octocat: In Order to Customise stats Message, You have to Edit few lines in `__main__.py` file. 

You Can Find `__main__.py` File Here ⬇️
```
slam-mirrorbot/bot/__main__.py
or
https://github.com/breakdowns/slam-mirrorbot/blob/master/bot/__main__.py
```
The Lines Which You Have to Edit are from  `Line 31` to `Line 39` . You can Customise the emojis and Words .
### Note: Don't Change Anything Which is written in `{ }` , Unless you know what you are doing.
🔗 [Line 32 to 40 can be opened from here](https://github.com/breakdowns/slam-mirrorbot/blob/d598144f752a3412da22977b5db88e7169792ae3/bot/__main__.py#L32)

# Customising Mirror Status
:octocat: In Order To Customise MirrorStatus, You Have to Edit `Line 17` to `Line 23` in `bot_utils.py` file.
You Can Find `bot_utils.py` File Here ⬇️
```
slam-mirrorbot/bot/helper/ext_utils/bot_utils.py
or
https://github.com/breakdowns/slam-mirrorbot/blob/master/bot/helper/ext_utils/bot_utils.py
```
🔗 [Line 17 to 23 can be opened from here](https://github.com/breakdowns/slam-mirrorbot/blob/d598144f752a3412da22977b5db88e7169792ae3/bot/helper/ext_utils/bot_utils.py#L17)

# Customising Mirror Progress Bar
:octocat: In Order To Customise Mirror Progress Bar, You Have to Edit `Line 27` ,`Line 84` & `Line 87` in `bot_utils.py` file.
You Can Find `bot_utils.py` File Here ⬇️
```
slam-mirrorbot/bot/helper/ext_utils/bot_utils.py
or
https://github.com/breakdowns/slam-mirrorbot/blob/master/bot/helper/ext_utils/bot_utils.py
```
🔗 [Line 27](https://github.com/breakdowns/slam-mirrorbot/blob/d598144f752a3412da22977b5db88e7169792ae3/bot/helper/ext_utils/bot_utils.py#L27)
In Line 27 Replace `▓` with the character of your Choice. This Character is Seen When Download Completes.

🔗 [Line 84](https://github.com/breakdowns/slam-mirrorbot/blob/d598144f752a3412da22977b5db88e7169792ae3/bot/helper/ext_utils/bot_utils.py#L84)
In Line 84 Replace `▓` with the character of your Choice. This Character will Indicate the Downloaded Part.

🔗 [Line 87](https://github.com/breakdowns/slam-mirrorbot/blob/d598144f752a3412da22977b5db88e7169792ae3/bot/helper/ext_utils/bot_utils.py#L87)
In Line 84 Replace `░` with the character of your Choice. This Character Will Indicate the Incomplete Download Part

![Progress Bar](https://i.ibb.co/CWFLLgS/progress-bar.png)


# Customising Bot status Message
:octocat: In Order To Customise Bot status Message, You Have to Edit `Line 96` to `Line 112` in `bot_utils.py` file.

You Can Find `bot_utils.py` File Here ⬇️
```
slam-mirrorbot/bot/helper/ext_utils/bot_utils.py
or
https://github.com/breakdowns/slam-mirrorbot/blob/master/bot/helper/ext_utils/bot_utils.py
```
### Note: Don't Change Anything Which is written in `{ }` , Unless you know what you are doing.

# Customising Bot After Download Complete Message
:octocat: In Order To Customise Bots Message after Downnload Complete, You Have to Edit `Line 148` to `Line 176` in `mirror.py` file.
You Can Find `mirror.py` File Here ⬇️
```
slam-mirrorbot/bot/modules/mirror.py
or
https://github.com/breakdowns/slam-mirrorbot/blob/master/bot/modules/mirror.py
```
🔗 [Line 148](https://github.com/breakdowns/slam-mirrorbot/blob/d598144f752a3412da22977b5db88e7169792ae3/bot/modules/mirror.py#L148)


### *This is Just a Small Guide using which small small Customisations can be made in Mirror Bot.*
### *I Hope It is Helpful to Beginners.*
### *If I Missed any Part, You can request for that.*
