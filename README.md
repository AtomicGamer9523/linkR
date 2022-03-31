# **linkR**'s Docs

## Import

```js
// Common JS
const LinkR = require('linkr-api');
```

```ts
// ECMAScript or TypeScript
import * as LinkR from 'linkr-api';
```

```dart
// Dart
import 'package:linkr/api.dart' as LinkR
```

<br>

## [Full JS Docs](https://www.docs.linkrbot.com/js/ "https://www.docs.linkrbot.com/js/")

## [Full Dart Docs](https://www.docs.linkrbot.com/dart/ "https://www.docs.linkrbot.com/dart/")

## [Endpoints](https://www.docs.linkrbot.com/https/ "https://www.docs.linkrbot.com/https/")

<br>
<br>
<br>
<br>

## Example Using discord.js@12

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
