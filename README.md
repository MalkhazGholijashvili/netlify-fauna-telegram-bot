
## Hooking up the Bot

Therafter, you need to specify and tell telegram where your bot should direct the messages it received to. Do so by simply visiting this url (without the ```{```, ```}```)

```
https://api.telegram.org/bot{your_bot_token}/setWebhook?url={your_netlify_domain_url}/api/bot
```

If it is setup correctly it should reponse back with

```json
{
  "ok": true,
  "result": true,
  "description": "Webhook was set"
}
```

Afterwhich, YOU ARE DONE!🎉🎉

Try typing ```/start``` to your bot and watch as the user ID of the Telegram user is stored inside your FaunaDB database

# Extending Telegram Bot Functionality

This bot uses telegraf.js for its Telegram Bot functionality. Head to its [website](https://telegraf.js.org/#/) to find out how to extend the functionality of the bot you have created :)

