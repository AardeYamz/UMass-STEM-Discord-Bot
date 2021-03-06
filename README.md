# UMass STEM Discord Bot

Bot designed for the UMass STEM Discord server for memes and other server functionality.

**Bot Prefix**: Start a command with $ to use the bot

## Add to your server

[Invite bot to server](https://discordapp.com/api/oauth2/authorize?client_id=552254598279069708&permissions=1342179392&scope=bot)

## Commands
### Roles
- get [role]
  - The bot gives the specified role to the user
- remove [role]
  - The bot removes the specified role from the user (if they have it)
- getlist
  - Prints out an organized list of roles available with the get command
- myroles [optional: @user]
  - Prints out the calling user's (or mentioned user's) roles organized by category

### General
- members
    - Outputs the current number of members in the server
- leaderboard [optional: #channel]
    - Displays the top 10 most active users on the server (or mentioned channel) measured by quantity of messages
- covid [optional: state]
    - Displays the number of cases and deaths related to COVID19 in the specified state, if no state given displays the top 15 states by cases in the U.S
- covidp
    - Displays the number of cases, and deaths related to COVID19 in the top 15 U.S states. Sorted by percentage of the state infected.
- help
    - Displays the available *Role* and *General* commands
- memehelp
    - Displays the available *Meme* and *Image Filter* commands

## Stocks
- stock [ticker]
    - Display stock price, price change, percent change
- stockcandle [ticker timeframe]
    - Displays the stock's candle data over specified timeframe.  
      - Possible timeframes (multiples can be specified ex. 5D): D, W, M, Y, MAX
- stockline [ticker timeframe]
    - Displays the stock\'s data in a line graph over specified timeframe.
      - Possible timeframes (multiples can be specified ex. 5D): D, W, M, Y, MAX
  
### Memes
- mdraw [image/image link/text]
    - The bot responds with an image of marius drawing whatever image or text is passed as the argument
- tdraw [image/image link/text]
    - The bot responds with an image of tim drawing whatever image or text is passed as the argument
- ldraw [image/image link/text]
    - The bot responds with an image of lan drawing whatever image or text is passed as the argument
- landraw [image/image link/text]
    - The bot responds with a different image of lan drawing whatever image or text is passed as the argument
- shelpoint [image/image link/text]
    - The bot responds with an image of Dan Sheldon pointing at whatever image or text is passed as the argument
- bdraw [image/image link/text]
    - The bot responds with an image of barrington drawing whatever image or text is passed as the argument

**Example of the $bdraw [text] generator**

[![bdraw example](https://i.gyazo.com/c598fe1f391e75f0207dc392332cd622.gif)](https://gyazo.com/c598fe1f391e75f0207dc392332cd622)

- barrify [image/image link]
    - The bot uses computer vision to put the barr emote on peoples faces in the inputed image

**Example of the $barrify [image/image link] meme generator**

[![barrify example](https://i.gyazo.com/8da3a10f6f2ff0b3e59f3535fad204c6.gif)](https://gyazo.com/8da3a10f6f2ff0b3e59f3535fad204c6)

- surprisedpikachu [image/image link]
    - Similar to barrify the bot responds with the inputed image with surprised pikachu over identified faces
- marify [image/image link]
    - Similar to barrify the bot responds with the inputed image with marius's face over the identified faces
- timify [image/image link]
    - Similar to barrify the bot responds with the inputed image with tim's face over the indentified faces
- liamify [image/image link]
    - Similar to barrify the bot responds with the inputed image with liam's face over the indentified faces
- zoombarr [image/image link]
    - Pastes an image of barr from Zoom onto the given image in the top right corner
- *okay* [image/image link]
    - The bot turns the given image into a video with marius saying okay as the background noise
- meme ["top" "bottom" image]
    - The bot responds with the inputed image with the specifed text on it in typical meme format
- erase
    - Deletes the most recent m/bdraw or barrify generated by the bot

### Image Filters
- intensify [factor image]
    - The bot responds with the inputed image exposed to the specified factor
- noise [image]
    - The bot outputs the inputed image with a noise filter applied
- pixelate [factor image]
    - The bot outputs the inputed image after pixelating it by a given factor, make sure to use a larger factor to see results on high-res images
- mirror [axis image]
    - The bot mirrors the image on the given axis (X or Y), and outputs the result
- saturate [factor image]
    - The bot saturates the given image by the given factor
- highlightEdges [image]
    - The bot responds with the inputed image with the highlighted edges filter
- customEdgeHighlight [red green blue image]
    - The bot responds with the inputed image with the custom highlighted edges filter

### Other functionality
- remove missing housing and major role
    - bot removes the missing housing and major role if someone has set both a housing and major role

## How to contribute
1. Fork repo
2. Install required dependencies
2. Write additional implementations
3. Create a bot on the [Discord Developer Portal](https://discordapp.com/developers/applications/)
4. Add your bot's token to your computer's environmental variables
    - key: 'BOT_TOKEN'
    - value: 'YOUR BOT TOKEN'
5. Invite your bot to a private test server
6. Test added bot commands
7. Once working, create a pull request

## Dependencies
To install the dependencies, in the root folder, run:
`pip install -r requirements.txt`
