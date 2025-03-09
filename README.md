<p align="center"><img width="100px"
   style="margin-bottom:-6px" src="https://cdn.discordapp.com/avatars/809496186905165834/7dbf02cb782c7111b817f329cac0257a.png" /></p>
<h1 align="center">Weky</h1>


## What is weky?
- A fun npm package to play games within Discord with buttons!
- looking for examples? click here: [Examples](https://github.com/SevenriotProjects/weky-npm/tree/main/Examples)

## Whats new?
- Removed quick.db because i got error while installing it :moyai:
- Removed djs v12 :moyai:

## Features
- 🧑 Beginner friendly
- 🎉 Easy to use
- ✨ Simple
- 🔘 Discord Buttons
- 🤖 Supports Discord.js V13
- and much more!

## Install the package 📥
```sh
npm install weky
```

## Usage 📚
```js
const { Calculator } = require("weky");
await Calculator({
    message: message,
    embed: {
        title: 'Calculator | Weky Development',
        color: '#5865F2',
        footer: '©️ Weky Development',
        timestamp: true
    },
    disabledQuery: 'Calculator is disabled!',
    invalidQuery: 'The provided equation is invalid!',
    othersMessage: 'Only <@{{author}}> can use the buttons!'
});
```

#### Discord.js v13.1.0
```js
const Discord = require('discord.js');
const client = new Discord.Client();
const { Calculator } = require('weky');

client.on('ready', async () => {
	console.log(`Logged in as ${client.user.tag}`);
});

client.on('messageCreate', async (message) => {
	if (message.content === '!calculator') {
		await Calculator({
			message: message,
			embed: {
				title: 'Calculator | Weky Development',
				color: '#5865F2',
				footer: '©️ Weky Development',
				timestamp: true,
			},
			disabledQuery: 'Calculator is disabled!',
			invalidQuery: 'The provided equation is invalid!',
			othersMessage: 'Only <@{{author}}> can use the buttons!',
		});
	}
});

client.login('DISCORD_BOT_TOKEN');
```
## Result 📤
<img src="https://i.imgur.com/DEdhHHd.png">

## Contributing 🤝
- Contributions, issues and feature requests are welcome!
- Feel free to check **[issues page](https://github.com/SevenriotProjects/weky-npm/issues)**.
- 
## Developers (New) 👨‍💻
- **Sadman**: Discord: **.sadnan_**

## Old Developers 👨‍💻
- **[Face#5454](https://github.com/face-hh)**
- **[Sujal Goel#7602](https://github.com/sujalgoel)**
- **[rayz#4986](https://github.com/rayzdev)**

## Support ❔
<a href="https://discord.gg/ANzBrkcXZy"><img src="https://invidget.switchblade.xyz/ANzBrkcXZy" /></a>
