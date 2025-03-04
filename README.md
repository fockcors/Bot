# r/fuckcars Bot for r/place

The bot for r/fuckcars and their allies! This bot connects with the [command server](https://github.com/fockcors/Commando) and gets it's orders from there.

Command Server: https://placefc.herokuapp.com/

*This project is a copy of https://github.com/PlaceNL/Bot* - 🇳🇱 Thanks a lot! 🇳🇱

IF you want to help with maintaining this project, look into DEVELOPMENT.md.

## User script bot

### Installation instructions

before you start, make sure your cooldown has run out!

1. Install the [Tampermonkey](https://www.tampermonkey.net/) browserextention.
2. Click on this link: [https://github.com/fockcors/Bot/raw/master/fuckcarsbot.user.js](https://github.com/fockcors/Bot/raw/master/fuckcarsbot.user.js). If everything went well you'll see Tampermonkey ask you to add it. Click **Install**.
3. Reload your **r/place** tab. If everything went well, you'll see "Accesstoken ophalen..." in the top right of your screen. The bot is now active, You'll be able to see what the bot is doing through these messages.

### Cons of this bot

- When the bot places a pixel, it will look as if it wasn't placed, while the bot has already done that (and thus you're in cooldown). You can see the cooldown in the topright of your screen.

## Headless bot

### How to get reddit_session cookie
**NOTE: People have reported that this is annoying to do on chrome because teksts get unselected. Therefore we recommend that you use firefox.**

1. Go to [r/place](https://reddit.com/r/place)
2. Open dev tools and go to the network tab
3. Refresh the page
4. Click on the first request to reddit.com/r/place (See image)
![Screenshot_20220403_165251](https://user-images.githubusercontent.com/9784257/161433856-27ef7e7c-7f00-4b37-b274-4199ea919aa9.png)
5. Go to the tab called `Cookies`
6. Copy the value of the `reddit_session` cookie

### Installation instructions

1. Install [NodeJS](https://nodejs.org/).
2. Download the bot via [this link](https://github.com/fockcors/Bot/archive/refs/heads/master.zip).
3. Extract the bot anywhere on your desktop
4. Open a command prompt/terminal in this folder
    Windows: Shift+right mousebutton in the folder -> Click on "open Powershell here"
    
    Mac: No clue, sorry!
    
    Linux: Is this necessary?
5. install the dependencies: `npm i`
6. execute the bot `node bot.js SESSION_COOKIE_HERE`
7. BONUS: You can repeat these steps for any amount of accounts you'd want. Keep in mind to use different accounts.
