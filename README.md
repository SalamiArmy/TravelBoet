# TravelBoet
## A python bot for fast paced group chats about planning trips.

### What is TravelBoet?
TravelBoet is a chat bot for telegram that can get information about flights.

### How does it work?
TravelBoet will listen for all messages in a given chat (either directly with him or in a chat room which you invite him to) starting with "/getflight".
tl;dr: Look at one of the existing commands, you must have a run(bot, chat_id, user, request_text, keyConfig, number_of_results) function.

### How do I make my own bot using this?
Go to https://console.developers.google.com and create a Google App Engine project. Then take that project id (it will be two random words and a number eg. gorilla-something-374635) and your Telegram Bot ID which the Bot Father gave you and do the following:

1. Copy app.yaml.template and rename the copy to to app.yaml.
2. Update {GOOGLE APP ENGINE PROJECT ID} in app.yaml.
3. Copy bot_keys.ini.template and rename the copy to bot_keys.ini.
4. Update {Your Telegram Bot ID here} in bot_keys.ini 


Finally go to https://{GOOGLE APP ENGINE PROJECT ID}.appspot.com/telegram_webhook?url=https://{GOOGLE APP ENGINE PROJECT ID}.appspot.com/telegram_webhook (replace both {GOOGLE APP ENGINE PROJECT ID}s with the Google App Engine Project ID) to tell Telegram where to send web hooks. This is all that is required to setup web hooks, you do not need to tell the Bot Father anything about web hooks.

### Why the name TravelBoet?
Boet is Afrikaans for brother.
