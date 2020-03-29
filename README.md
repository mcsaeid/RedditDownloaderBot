# Reddit Downloader Bot
A telegram bot to download the reddit posts.
## What can this bot do?
* Send posts as text in telegram
* Download and send photos in `i.redd.it`
* Download and send GIFs
* Download videos on `v.redd.it` and merge the audio with them using [FFmpeg](https://www.ffmpeg.org/)
* Choose the quality of photos or videos
## What this bot can't do?
* Upload files that are larger than 50MB
* Download any videos or photos that are not hosted on `x.redd.it` (for example youtube)
## Setup
To start, please at first install [FFmpeg](https://www.ffmpeg.org/) in your path. On Ubuntu, `apt install ffmpeg` is enough.

Then download and build this project:
```bash
git clone https://github.com/HirbodBehnam/RedditDownloaderBot
go get github.com/go-telegram-bot-api/telegram-bot-api github.com/google/uuid github.com/patrickmn/go-cache
go build main.go
```

For running, pass the bot token as the first argument: `./bot 1234567:4TT8bAc8GHUspu3ERYn-KGcvsvGB9u_n4ddy`