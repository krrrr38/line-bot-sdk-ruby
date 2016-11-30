# sinatra echo - LINE Messaging API

Sample echo-bot using [Sinatra](http://www.sinatrarb.com/)

## Getting started local env

```
$ export LINE_CHANNEL_SECRET=YOUR_LINE_CHANNEL_SECRET
$ export LINE_CHANNEL_TOKEN=YOUR_LINE_CHANNEL_ACCESS_TOKEN

$ bundle install
$ bundle exec app.rb
```

## Getting started with Heroku

### heruku button

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/krrrr38/line-bot-sdk-ruby)

then set Webhook URL: `https://{YOUR_APP}.herokuapp.com/callback`

### deploy by yourself

```sh
heroku create
heroku info # then set Webhook URL: https://{YOUR_APP}.herokuapp.com/callback
heroku config:set LINE_CHANNEL_SECRET="..."
heroku config:set LINE_CHANNEL_TOKEN="..."
git push heroku master
heroku logs
```
