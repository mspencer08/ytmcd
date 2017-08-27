# ytmcd
YouTube Music Channel Downloader.

A sensible selection of youtube-dl flags to download music from music channels in bulk!

If you are using this for yourself, feel free to ignore file `downloaded` as that is for my own personal record, and be sure to edit `channels` to your own preferences.


### Remarks

Refer to the man page for my `youtube-dl` flag choices, but here are some points worth mentioning:

* `--download-archive downloaded`: sucessful downloads will have their video ids listed here, which `youtube-dl` will ignore in subsequent runs
* `--geo-bypass`: useful for a lot of the Asian songs (thanks SONY Japan...)
* `--max-filesize 128m`: Usually amounts to 2-3 hour files in ytmcd's case, fits most reasonable-length music mixes and avoids annoying 10-hour novelty videos
* `--add-metadata`: Writes the video's metadata (e.g. title becomes title, channel name becomes artist) to the downloaded audio file

And for some general Q/A (please correct me if I am wrong via issue or PR):

##### Why `-f bestaudio -f m4a` instead of `-x --audio-format mp3 --audio-quality 0`?

See [this](https://www.reddit.com/r/DataHoarder/comments/6w37ec/ytmcd_a_sensible_selection_of_youtubedl_flags_to/dm5anr1/) reddit thread. [Here](https://superuser.com/a/846856) is another great explanation.

##### Why no `--restrict-filenames`?

* I download lots of East Asian music and prefer to keep the original titles as filenames
* My terminal can handle unicode


### Channels

These are the channels I currently back up for myself.

In no particular order:

```
UCKioNqOX_kOCLcSIWPL_lxQ - Aviencloud
UCtkSwwONNeMC3C2aHxGeFmA - Inspira
UCJWQkiBMWCmr3BbZolEmgXw - Shinico
UC6hBefyLMtG7FXhZ55da3Vw - Artzie Music
UCUHhoftNnYfmFp1jvSavB-Q - Funky Panda™
UCIKF1msqN7lW9gplsifOPkQ - GalaxyMusic
UCYTNxR2Z4ryz88WRWiaPCdg - K - Music Sweet
UCZ7368uifluuE3Xh-XrqlWQ - Leafy Radio
UCJ6td3C9QlPO9O_J5dF4ZzA - Monstercat
UC_aEa8K-EOJ3D6gOs7HcyNg - NoCopyrightSounds
UCl4UOc8h1ZnO-inFPgAu7gw - NXS
UC3ifTl5zKiCAhHIBQYcaTeg - Proximity
UCcoYD5HDg8P-gvJU-oDYq5Q - StrobeNetwork Records
UCsPOjxg79gnqBmpUY38t_3g - VoicedOut
UC-wNjNTqCfXSKd4S1tNgWUg - Waifu Wednesdays
UCRs41MXZpAhXgiD4KjTjabg - Xefox Music
UCMOgdURr7d8pOVlc-alkfRg - xKito Music
UC7tD6Ifrwbiy-BoaAHEinmQ - Diversity
UC5nc_ZtjKW1htCVZVRxlQAQ - MrSuicideSheep
UCbKJXEbKdmiJO0tQzb1SmRg - Wejustman Music
UCvOGElQWhX8tyTxwzv1rKzg - ENM
UCKP5rY3Kr5FBZY13LzF-gpw - Universe Music
UCbfMTDftQhRySQKFCV8PfHg - GalaxyMusicNet
UCSa8IUd1uEjlREMa21I3ZPQ - CloudKid
UCM9KEEuzacwVlkt9JfJad7g - Chill Nation
UCa10nxShhzNrCE1o2ZOPztg - Trap Nation
UC8QfB1wbfrNwNFHQxfyNJsw - Rap Nation
UCFZ75Bg73NJnJgmeUX9l62g - Selected
UCgMyPaCx5-LkEx_54Ul9f-A - Futurism
UCK9Rngx643faIs9b4jxHQHw - Grizzly Music
UCSXm6c-n6lsjtyjvdD0bFVw - Liquicity
```
