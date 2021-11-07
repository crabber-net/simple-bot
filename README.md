# Simple Bot

A basic Crabber bot that posts randomly from a list of quotes.

## Installation

1. Clone this repository
```console
~$ git clone https://github.com/crabber-net/simple-bot/
~$ cd simple-bot
```

2. Create an account for your bot on [Crabber](https://crabber.net)

3. Generate a developer key and access token on 
   [Crabber's developer page](https://crabber.net/developer/)

4. In your project directory, create a file called `.env` and put the following
   content in it:
```bash
export CRABBER_DEPLOY_KEY="{{your developer key}}"
export CRABBER_DEPLOY_TOKEN="{{your access token}}"
```

5. Edit `quotes.txt` and fill it with stuff you want the bot to post.

6. **[Only once]** Install the dependencies
```console
# with poetry
~/parabot$ poetry install
# or with pip
~/parabot$ pip3 install -r requirements.txt
```

7. Run your bot and see if it works!
```console
# with poetry
~/parabot$ poetry run python simple_bot.py
# or with pip
~/parabot$ python3 simple_bot.py
```
If it was successful you should see something like this in the logs:
```console
2021-11-07 12:24:39.791 | INFO     | __main__:<module>:68 - Posted molt successfully.
```
Otherwise, read the logs and look for what went wrong. It's likely something
pretty simple.

8. Deploy your bot! There are a lot of ways to do this so it's recommended you
   look up the best way to do it on your system. Here are a couple recommended
   options:
	* *Linux:* crontab
	* *Windows:* Windows Task Scheduler
	* *macOS:* Shortcuts, Automator, or crontab
