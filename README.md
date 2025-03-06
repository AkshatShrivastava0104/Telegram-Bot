
# Telegram Bot Starter

This is a simple Telegram bot starter project built using Node.js and Express. The bot responds with "Polo!!" when a user sends a message containing the word "start".

## Features
 
- Message Handling
- Telegram API Integration  



## Prerequisites
* Node.js installed on your machine.
* A Telegram bot token.You can get this by creating a new bot via the BotFather on Telegram.
## Installation      

Clone the repository:

```bash
git clone https://github.com/your-username/telegram-bot-starter.git
cd telegram-bot-starter
```
Install the required dependencies:

```bash
npm install
```

Replace the bot token in the code with your own Telegram bot token:
```bash
axios.post(
    "https://api.telegram.org/botYOUR_BOT_TOKEN/sendMessage",
    {
        chat_id: message.chat.id,
        text: "Polo!!",
    }
)

```

Start the server:
```bash
node index.js
```



## Deployment

Install now on your system :

```bash
  npm install -g now
```
Add a start script to your package.json file:
```bash
"scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "start" : "node index.js"
  }
```

Once you’ve added the script, run the command :
```bash
now
```

Now, all we need to do is let telegram know that our bot has to talk to this url whenever it receives any message. We do this through the telegram API. Enter this in your terminal :

```bash
curl -F "url=https://my-telegram-bot-tanvxponxj.now.sh/new-message" https://api.telegram.org/bot<your_api_token>/setWebhook
```


## Usage/Examples


* Send a message containing the word "start" to your bot on Telegram.
* The bot will respond with "Polo!!".



## Project Structure

* index.js: The main server file that handles incoming requests and sends responses.
* package.json: Contains project dependencies and scripts.
## Dependencies

* express: Web framework for Node.js.
* body-parser: Middleware to parse incoming request bodies.
* axios: Promise-based HTTP client for making requests to the Telegram API.
## Contributing

Contributions are always welcome!

See `README.md` for ways to get started.

Feel free to fork the repository and submit pull requests.
For major changes, please open an issue first to discuss what you would like to change.

