# Mentor bot

A discord bot for submitting a mentor request form at HackTheMidlands 4.0.

## Usage

Type `!mentor` anywhere in the HackTheMidlands Discord server, and it will trigger the bot to privately message you the questions required for requesting a mentor.

## Development

### Setup a virtual environment

```bash
$ python3 -m venv .venv
$ source .venv/bin/activate
```

### Install required packages

```bash
$ pip3 install -r requirements.txt
```

### Configuation

You will need a token for discord. Follow [this guide](https://github.com/reactiflux/discord-irc/wiki/Creating-a-discord-bot-&-getting-a-token) to get one.

Add the token, and URL for the form you want to use to `config.json`.

```json
{
    "token": "token",
    "url": "url",
    "start_message": "First message when the command is called",
    "end_message": "Last command to show all the questions have be answered",
    "embed_title": "The title for polls, such as radios",
    "prefix": "prefix for the discord bot"
}
```

### Run

```bash
$ python3 -m mentorbot
```

## Contributors

- [Justin Chadwell](https://github.com/jedevc): Form scraping, validation and submission
- [Will Russell](https://github.com/wrussell1999): Discord bot used for asking questions and response handling
