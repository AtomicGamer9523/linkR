# **linkr-api** module

## Import

```js
const LinkR = require('linkr-api');
```

```ts
import * as LinkR from 'linkr-api';
```

<br>

## Example Using discord.js

```js
// Common JS
const LinkR = require('linkr-api');//importing
LinkR.setToken("12345678901234567890");//logging in
// is in debug mode right now
// change to .setToken("TOKEN", false); to disable
const Discord = require('discord.js');
const client = new Discord.Client();
client.login("TOKEN");

client.on("message", message => {
    if(message.content === "!data"){
        const user = LinkR.parse("DISCORD", message.author.id);//get LINKR_ID using discord
        message.reply(LinkR.userEmbed(user));//sends a Discord MessageEmbed
    }
});
```

<br>

```ts
// ECMAScript or TypeScript
import * as LinkR from 'linkr-api';//importing
LinkR.setToken("12345678901234567890");//logging in
// is in debug mode right now
// change to .setToken("TOKEN", false); to disable
import * as Discord from 'discord.js';
const client = new Discord.Client();
client.login("TOKEN");

client.on("message", message => {
    if(message.content === "!data"){
        const user = LinkR.parse("DISCORD", message.author.id);//get LINKR_ID using discord
        message.reply(LinkR.userEmbed(user));//sends a Discord MessageEmbed
    }
});
```
