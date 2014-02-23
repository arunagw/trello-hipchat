# trello-hipchat

Parse Trello activity feed into HipChat.

## Setup
Get your [Trello API key](https://trello.com/1/appKey/generate) and [Trello API token](https://trello.com/docs/gettingstarted/index.html#getting-a-token-from-a-user), then clone the repo or:

## Heroku
1. Clone the repo
2. Create a new Heroku app: `heroku create`
3. Push: `git push heroku master`
4. Set your config vars:

```
heroku config:set TRELLO_API_KEY=fill_me_in TRELLO_API_TOKEN=fill_me_in TRELLO_BOARD_ID=fill_me_in HIPCHAT_ROOM=fill_me_in HIPCHAT_TOKEN=fill_me_in HIPCHAT_USERNAME_TO_DISPLAY=fill_me_in UPDATE_INTERVAL=30
```

Also, you may need to start your worker: `heroku ps:scale worker=1`

## Credits
This code is heavily based on [trello-campfire](https://github.com/simondec/trello-campfire) is brought to your by [Simon de Carufel](http://rufel.ca/).
