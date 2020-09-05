
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/Jishnu133/chic_.git)

# YtbDownBot
Telegram bot that utilize youtube-dl functionality for downloading video directly to telegram.
Simple clone of https://t.me/VideoTubeBot.

# Dependencies
Install `ffmpeg` and `python3`.

Python3 dependencies install via `pip3 install -r requirements.txt`
# Running
For running required phone number for bypassing telegram bot api upload files limitation to 50 MB.

Set the following enviroment variables:
  1. Bot token(from Bot Father):
`BOT_API_TOKEN`

  2. Chat id between bot and agent (regular client with phone number 
for bypass limit in 50MB):
`BOT_AGENT_CHAT_ID`

  3. Chat id between agent(regular client with phone number 
for bypass limit in 50MB) and bot:
`CHAT_WITH_BOT_ID`

  4. Api id (https://core.telegram.org/api/obtaining_api_id):
`API_ID`
  5. Api hash (https://core.telegram.org/api/obtaining_api_id):
`API_HASH`
  6. Telegram client session string for telethon StringSession:
  `CLIENT_SESSION`
  7. IBM Cloudant credentials: 
  `CLOUDANT_USERNAME`, `CLOUDANT_PASSWORD`, `CLOUDANT_URL`
  (can be easily replaced with CouchDB: read https://python-cloudant.readthedocs.io/en/latest/getting_started.html)

Note: for deploying you must set also webhook url via calling `https://api.telegram.org/bot<bot-token>/setWebhook?url=<webhook-url>` (`webhook-url` path is `bot_domanin+/bot` like `mybot.com/bot`) Use master branch if you want to use polling instead.
