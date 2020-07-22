# WD Economy Bot

This is a fork of [taubot](https://github.com/jonathanvdc/taubot)

## Dependencies

Taubot's dependencies are defined in the `requirements.txt` file. Install them with

```bash
pip3 install -r requirements.txt
```

## Usage

The bot will need credentials to log into Reddit. Summarize them in a JSON file named `bot-config.json` placed in the directory from which you run the bot. A `bot-config.json` looks like this:

```json
{
  "reddit_client_id": "CLIENT_ID",
  "reddit_client_secret": "CLIENT_SECRET",
  "reddit_username": "USERNAME",
  "reddit_password": "PASSWORD",
  "discord_token": "BOT TOKEN",
  "server_key": "PEM PRIVATE RSA KEY",
  "prefix": ["Prefix 1", "Prefix 2", "etc"],
  "colour": "Hex code for embed colour",
  "ledger-path": "/path/to/ledger"
}
```
Please note that if any of the arguments are missing the bot will print a warning and gracefully degrade into not using the
associated feature

To make the bot respond to all unread messages, simply run `python3 src/bot.py`.

## Rules For Contribution

All people who wish to contribute to the source must first consider wether there changes would be valued by the base repository [taubot](https://github.com/jonathanvdc/taubot)
if you believe that the changes would be of value there make a pull request there and we'll merge the changes, if you do not believe they will be accepted
by taubots development team but would work with Weekly Dictator make a pr here

all changes made here that are not made on taubots base repo legally must be named in the [CHANGES.md](https://github.com/gamingdiamond982/WD-Economy-Bot/blob/master/CHANGES.md) file per the license agreement
