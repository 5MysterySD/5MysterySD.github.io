---
title: TeleLeechX Bot
date: 2022-07-12 03:20:00 +0200
categories: Project
tags: ["telegram", "python", "telegram-bot"]
image: 
---

## Tele-LeechX

🇹🇷 Telegram Leech bot supports 4GB files

Do you want [Source Code?](https://github.com/5MysterySD/Tele-LeechX)

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://github.com/5MysterySD/Tele-LeechX)

## About

A Powerful Pyrogram Based Telegram Leech Bot Modded by `MysterySD` to directly Leech to Telegram, with Multi Direct Links Support for Enhanced Leeching.
You can enter your user session for 4gb upload. it's automatically understands you are premium and uploads files greater than 2 GB.

Deploy from main repo's readme. There is a guide.
Bot commands will auto-setting by bot.

## Features

### From This Repo

- Fully non-credit repo (For protect repo from ban etc.)
- Fixed a lot of things and strings
- Fixed restart
- Added heroku restart, kill
- Fixed userbot file upload
- Fixed log sending for owner
- Dynamically gets repos latest code from github
- Heroku will never sleep

### From Original Repo

- Google Drive link cloning using gclone.(wip)
- Telegram File mirrorring to cloud along with its unzipping, unrar and untar
- Drive/Teamdrive support/All other cloud services rclone.org supports
- Unzip, Unrar, Untar while Leeching to Telegram .
- Custom file name (Used in Prefix on Every Item Leeched)
- Custom commands for Using in Telegram .
- Get total size of your working cloud directory
- You can also upload files downloaded from `/ytdl` command to gdrive using `/ytdl gdrive` command.
- You can also deploy this on your VPS .
- Option to select either video will be uploaded as document or streamable
- Added `/renewme` command to clear the downloads which are not deleted automatically.
- Added support for YouTube Playlist .
- Renaming of Telegram files support added. 😐
- Changing rclone destination config on fly (By using `/rlcone` in private mode)
- Aria2 configs In Root
- Small FIX for Gclone
- Added Dynamic Config
- Added Custom ToggleDoc and ToggleVid Commands
- Added Custom Rename Command via vars
- Added direct rclone.conf url in vars
- Dual Commands Usage (Both With / Without Bot Username)
- Auto Commands Set To BotFather in Telegram
- New Torrent Search Support

    ```text
    nyaa.si, sukebei, 1337x, piratebay, tgx, yts, eztv, torlock, rarbg
    ```

- Extract Error Fixed
- UI Added for Improved User Experience with Easy to Use.
- Added New Status Bar using `/status` command.
- Added Speedtest Support.
- Direct links Supported:

    ```text
    letsupload.io, hxfile.co, anonfiles.com, bayfiles.com, antfiles,
    fembed.com, fembed.net, femax20.com, layarkacaxxi.icu, fcdn.stream,
    sbplay.org, naniplay.com, naniplay.nanime.in, naniplay.nanime.biz, sbembed.com,
    streamtape.com, streamsb.net, feurl.com, pixeldrain.com, racaty.net,
    1fichier.com, 1drv.ms (Only works for file not folder or business account), solidfiles.com 
    ```

- Extract these filetypes and uploads Telegram

    ```text
    ZIP, RAR, TAR, 7z, ISO, WIM, CAB, GZIP, BZIP2, APM, ARJ, CHM, CPIO, CramFS, DEB, DMG, FAT,HFS, LZH, LZMA, LZMA2, MBR, MSI, MSLZ, NSIS, NTFS, RPM, SquashFS, UDF, VHD, XAR, Z.
    ```

## Bot Commands (Set in [@BotFather](https://t.me/BotFather))

```text
leech - leech any torrent/magnet/direct-download link to Telegram 
leechunzip - This will unarchive file and upload to telegram.
leechzip - leech any torrent/magnet/direct-download link to Telegram and Upload It as .tar.gz acrhive...
ytdl - This command should be used as reply to a supported link
pytdl - This command will download videos from youtube playlist link and will upload to telegram. 
toggledoc - choose whether the file shall be uploaded as doc or not
togglevid - choose whether the file shall be uploaded as streamable or not
savethumbnail - save thumbnail
clearthumbnail - clear thumbnail
tleech - This will mirror the telegram files to ur respective cloud .
tleechunzip - This will unarchive telegram file and upload to cloud.
gclone - This command is used to clone gdrive files or folder using gclone
gytdl - This will download and upload to your cloud.
gpytdl - This download youtube playlist and upload to your cloud.
gleech - leech any torrent/magnet/direct-download link to cloud
gleechzip - leech any torrent/magnet/direct-download link to Cloud and Upload It as .tar.gz acrhive...
gleechunzip - This will unarchive file and upload to cloud.
getsize - This will give you total size of your destination folder in cloud.
rename - rename the file 
speedtest - Check Server Speedtest 
help - send help 
status - show bot stats and concurrent downloads
renewme - clear all downloads ❗ admin only
log - This will send you a txt file of the logs. ❗ admin only
rclone - This will change your drive config on fly. (First one will be default) ❗ admin only
```

## Environment Variables

### Required Variables

- `TG_BOT_TOKEN`: Create a Bot using [@BotFather](https://telegram.dog/BotFather), and get the Telegram API Token.
- `APP_ID`: Get this Value from [my.telegram.org/apps](https://my.telegram.org/apps).
- `API_HASH`: Get this Value from [my.telegram.org/apps](https://my.telegram.org/apps).
  - NOTE: If Telegram is blocked by your ISP, try Telegram to get the IDs.
- `AUTH_CHANNEL`: Create a Super(Means Changing it to `Visible` for `Chat History for New Members`) in Telegram, forward a Message from the Group to `@ShowJsonBot` to get this value.
- `OWNER_ID`: ID of the Bot Owner, He/She can be abled to access bot in bot only mode too(`Private mode`).

### Optional Variables

- `STRING_SESSION`: For 4 GB file upload. TG account must be premium.
- `CUSTOM_CAPTION`: Custom caption for uploaded files.
- `BOT_NO`: Bot number if you want more than one bot. Example: when you enter `5`, bot commands will set like: `/leech5`
- `SUDO_USERS`: Sudo users seperate with blank. `5234234 23423421 124214124`
- `TG_MAX_FILESIZE`: Dont touch if you want auto-detecting maximum available filesize.
- `CAP_STYLE`: Caption style html tag. Default code. Meanings: "\<code>\</code>" For bold: `bold`
- `BOT_PM`: For sending files to user in private chat. this will protect your group from copyright things. True or False
- `LEECH_LOG`: Log leeched files in channel. Example: `-1002342342`
- `PRM_LOG`: Log premium leeched files in channel. Example: `-1002342342`
- `EX_LEECH_LOG`: Log leeched files in extra channel. Example: `-1002342342`
- `UPLOAD_AS_DOC`: Takes two option True or False. If True file will be uploaded as document. This is for people who wants video files as document instead of streamable.
- `INDEX_LINK`: (Without `/` at last of the link, otherwise u will get error) During creating index, plz fill `Default Root ID` with the id of your `DESTINATION_FOLDER` after creating. Otherwise index will not work properly.
- `DESTINATION_FOLDER`: Name of your folder in ur respective drive where you want to upload the files using the bot.
- `CUSTOM_FILE_NAME`: Custom filename for uploaded documents.
- `EDIT_SLEEP_TIME_OUT`: Message editing delay in seconds.
- `UPDATES_CHANNEL`: Give your updates channel username or your personal username without @
- `DOWNLOAD_LOCATION`
- `ARIA_TWO_STARTED_PORT`
- `CANCEL_COMMAND_G`
- `CHUNK_SIZE`
- `CLEAR_THUMBNAIL`
- `CLONE_COMMAND_G`
- `FINISHED_PROGRESS_STR`
- `GET_SIZE_G`
- `GLEECH_COMMAND`
- `GPYTDL_COMMAND`
- `GYTDL_COMMAND`
- `LEECH_COMMAND`
- `LOG_COMMAND`
- `MAX_MESSAGE_LENGTH`
- `MAX_TIME_TO_WAIT_FOR_TORRENTS_TO_START`
- `PROCESS_MAX_TIMEOUT`
- `PYTDL_COMMAND`
- `RCLONE_COMMAND`
- `RENAME_COMMAND`
- `RENEWME_COMMAND`
- `SAVE_THUMBNAIL`
- `STATUS_COMMAND`
- `TELEGRAM_LEECH_COMMAND`
- `TELEGRAM_LEECH_UNZIP_COMMAND`
- `TG_OFFENSIVE_API`
- `TOGGLE_DOC`
- `TOGGLE_VID`
- `UN_FINISHED_PROGRESS_STR`
- `UPLOAD_AS_DOC`
- `UPLOAD_COMMAND`
- `YTDL_COMMAND`

## Available Bot Commands & Usage

Command | Usage
------------ | -------------
|`/rclone`| This will change your drive config on fly.(First one will be def `/gclone`..This command is used to clone gdrive files or folder using gclone.-Syntax- `[ID of the file or folder][one space][name of your folder only(If the id is of file, don't put anything)]` and then reply /gclone to it.\
|`/log`| This will send you a txt file of the logs.
|`/ytdl`| This command should be used as reply to a [supported link](https://ytdl-org.github.io/youtube-dl/supportedsites.html)
|`/pytdl`| This command will download videos from youtube playlist link and will upload to telegram.
|`/gytdl`| This will download and upload to your cloud.
|`/gpytdl`| This download youtube playlist and upload to your cloud.
|`/leech`| This command should be used as reply to a magnetic link, a torrent link, or a direct link. this command will SPAM the chat and send the downloads a seperate files, if there is more than one file, in the specified torrent
|`/leechzip`| This command should be used as reply to a magnetic link, a torrent link, or a direct link. [This command will create a .tar.gz file of the output directory, and send the files in the chat, splited into PARTS of 1024MiB each, due to Telegram limitations]
|`/gleech`| This command should be used as reply to a magnetic link, a torrent link, or a direct link. And this will download the files from the given link or torrent and will upload to the cloud using rclone.
|`/gleechzip` | This command will compress the folder/file and will upload to your cloud.
|`/leechunzip`| This will unarchive file and dupload to telegram.
|`/gleechunzip`| This will unarchive file and upload to cloud.
|`/tleech`| This will mirror the telegram files to ur respective cloud cloud.
|`/tleechunzip`| This will unarchive telegram file and upload to cloud.
|`/getsize`| This will give you total size of your destination folder in cloud.
|`/renewme`| This will clear the remains of downloads which are not getting deleted after upload of the file or after /cancel command.
|`/rename`| u can add custom name as prefix of the original file name...Like if your file name is `gk.txt` uploaded will be what u add in `CUSTOM_FILE_NAME` + `gk.txt`..And also added custom name like...You have to pass link as ..`www.download.me/gk.txt new.txt`..the file will be uploaded as `new.txt`.
|`/toggledoc` | it used for toggling to be files if shall it be uploaded as doc via direct inchat cmd... **any users can now choose if their files will be upload as doc or streamabe...**
|`/togglevid` | it used for toggling to be files if shall it be uploaded as vid via direct inchat cmd... **any users can now choose if their files will be upload as doc or streamabe...**
|`/status`| show bot stats and concurrent downloads
|`/savethumbnail`| save the thumbnail
|`/clearthumbnail`| clear the thumbnail
|`/help`| send help

## RClone Guide

- Set Rclone locally by following the official repo : <https://rclone.org/docs/>
- Get your `rclone.conf` file. will look like this:

    ```text
    [NAME]
    type = 
    scope =
    token =
    client_id = 
    client_secret = 
    ```

- Copy `rclone.conf` file in the root directory (Where `Dockerfile` exists).
- Your config can contains multiple drive entries.(Default: First one and change using `/rclone` command)

## Lisence

![](https://www.gnu.org/graphics/gplv3-127x51.png)

You can use, study share and improve it at your will. Specifically you can redistribute and/or modify it under the terms of the [GNU General Public License](https://www.gnu.org/licenses/gpl-3.0.html) as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

## Credits

- [`MysterySD`](https://github.com/5MysterySD) for Speedtest, Direct Link Support, More in Future.
- [`KGK06`](https://github.com/KGK06) For Merging Different Repos
- [`XcodersHub`](https://github.com/XcodersHub) For The Aria2 Config & Little More
- [`GautamKumar`](https://github.com/gautamajay52/TorrentLeech-Gdrive) 😬
- [`SpEcHiDe`](https://github.com/SpEcHiDe/PublicLeech) for his wonderful code😚
- [`Rclone Team`](https://rclone.org) for theirs awesome tool☁️
- [`Dan Tès`](https://telegram.dog/haskell) for his [Pyrogram Library](https://github.com/pyrogram/pyrogram)
- [`Robots`](https://telegram.dog/Robots) for their [@UploadBot](https://telegram.dog/UploadBot)
- [`@AjeeshNair`](https://telegram.dog/AjeeshNait) for his [torrent.ajee.sh](https://torrent.ajee.sh)
- [`@gotstc`](https://telegram.dog/gotstc), `@aryanvikash`, [`@HasibulKabir`](https://telegram.dog/HasibulKabir) for their TORRENT groups
