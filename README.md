<p align="center"><a href="https://t.me/fridayot"><img src="https://telegra.ph/file/47ea0bd1ab8f0a42620a6.jpg" width="5000"></a></p> 
<h1 align="center"><b>FRIDAY-USERBOT 🇱🇰 </b></h1>
<h4 align="center">A Powerful, Smart And Simple Userbot In Pyrogram.</h4>

## Support 
<a href="https://t.me/FridaySupportOfficial"><img src="https://img.shields.io/badge/Join-Telegram%20Channel-red.svg?logo=Telegram"></a>
<a href="https://t.me/fridayOT"><img src="https://img.shields.io/badge/Join-Telegram%20Group-blue.svg?logo=telegram"></a>


# String Session - Pyrogram 
### Repl 
[![Run on Repl.it](https://repl.it/badge/github/STARKGANG/friday)](https://replit.com/@MIDHUNKMKM/StringGen)


# Hosting 🌙

### Deploying To Heroku 

[![Deploy To Heroku](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/Captainamarica/Friday-user-bot-Navanjana)

#

### Mandatory Configs 🐾
```
[+] Make Sure You Add All These Mandatory Vars. 
    [-] API_ID:   You can get this value from https://my.telegram.org
    [-] API_HASH :   You can get this value from https://my.telegram.org
    [-] STRINGSESSION : Your String Session, You can get this From Repl or BY running String_Gen File Locally
    [-] MONGO_DB : Your Mongo DB DataBase Url. 
    [-] LOG_GRP: Your Log Group/Channel Chat ID. This is Very Important and Some Modules Will Not Work Well Without This!
[+] The fridayUserbot will not work without setting the mandatory vars.
```

# Examples - Plugins 👊

### Plugins 🔧

```python3
from main_startup.core.decorators import friday_on_cmd
from main_startup.helper_func.basic_helpers import edit_or_reply

@friday_on_cmd(['helloworld'],
    cmd_help={
    "help": "This is A TEST",
    "example": ".helloworld"
    })
async def hello_world(client, message):
    mg = await edit_or_reply(message, "`Hello World! This Works!`")
```
### Custom Filters 📣

```python3
from main_startup.core.decorators import listen

@listen(filters.mentioned & ~filters.me)
async def mentioned_(client, message):
    await message.reply_text("`Hello World! Btw Why Did You Mention Me?`")
```

# X-Tra Plugins 🎸
* Please Visit [Xtra-Plugins](https://github.com/DevsExpo/Xtra-Plugins) To Checkout Xtra-Plugins.


