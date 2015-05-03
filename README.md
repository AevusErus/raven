# Raven

Raven is a chat bot built on the [Hubot][hubot] framework. It was initially generated by [Hubot Generator][generator-hubot], and configured to be deployed on [Heroku][heroku].

[heroku]: http://www.heroku.com
[hubot]: http://hubot.github.com
[generator-hubot]: https://github.com/github/generator-hubot

## Active Deployments

Raven supports one deployment currently:

* The Omega Res Novae Slack (as Mudkip, invocation is @mudkip)

## Active Plugins

* Authentication (user specific permission to access bot functionality)
* Teamspeak track
* Danbooru
* e621
* YouTube
* Google
* Weather
* Topic protection
* Hubot aliases

## Features Wanted

* Room archiving (to get around Slack/HipChat 10k history limit)

##Setup
1. Clone the repo
2. ''''cd raven''''
3. ''''npm install''''
4. Launch on heroku (you get a tutorial when you create heroku)
5. Setup the following env variables: ''''heroku config:set ENVVAR=blah''''
	1. HEROKU_URL
	2. ADAPTER
	3. HUBOT_SLACK_TOKEN
	4. HUBOT_ADMINS (only Slack id)
	5. HUBOT_TEAMSPEAK_IP
	6. HUBOT_TEAMSPEAK_USER
	7. HUBOT_TEAMSPEAK_PASSWORD
	8. HUBOT_TEAMSPEAK_VOICE_PORT
	9. HUBOT_TEAMSPEAK_OUT_ROOM
	10. FORECAST_IO_KEY - ''''https://developer.forecast.io/''''
	11. GOOGLE_API_KEY & HUBOT_GOOGLE_API_KEY
		1. https://console.developers.google.com/project
		2. create a new project
		2. then click on APIS & Auth -> APIs
		2. and under api library
		2. search for Geocoding API
		2. and enable that
		2. then search for Time Zone API
		2. and enable that
		2. then go to credentials
		2. and hit create new key for public access
	12. REDIS_URL & REDISCLOUD_URL & REDISTOGO_URL

##Commands
Here is a list of commands that you can run:
* mudkip teamspeak
* mudkip weather me <location>
* mudkip ping
