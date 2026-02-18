<h1 align="center">Hi 👋, I'm DrayyExposed</h1>
<h3 align="center">A WhatsApp Web explorer. Diving deep into protocols, automation, and safe hacks. Powered by Baileys.</h3>

<p align="left"> <img src="https://komarev.com/ghpvc/?username=dryzxmods&label=Profile%20views&color=0e75b6&style=flat" alt="dryzxmods" /> </p>

<p align="left"> <a href="https://github.com/ryo-ma/github-profile-trophy"><img src="https://github-profile-trophy.vercel.app/?username=dryzxmods" alt="dryzxmods" /></a> </p>

<p align="left"> <a href="https://twitter.com/" target="blank"><img src="https://img.shields.io/twitter/follow/?logo=twitter&style=for-the-badge" alt="" /></a> </p>

- 🔭 I’m currently working on [Baileys](https://github.com/DrayyExposed/Baileys/tree/master)

- 🌱 I’m currently learning **- Node.js and Baileys - Web automation techniques - Ethical security research**

- 💬 Ask me about **- Baileys & WhatsApp Web automation - Node.js development - Ethical hacking & security research - Bots & scripting**

- 📫 How to reach me **dryzxmods@gmail.com**

<h3 align="left">Connect with me:</h3>
<p align="left">
</p>

# Modified Whatsapp-API
<p align='center'>
  <img src="https://files.catbox.moe/rhm9rt.webp" width="172">
</p>

--- 

## Usage
```json
"depencies": {
  "@whiskeysockets/baileys": "github:qwerty-xcv/Baileys"
}
```
## Import
```javascript
const {
  default:makeWASocket,
  // Other Options 
} = require('@whiskeysockets/baileys');
```

---
# How To Connect To Whatsapp
## With QR Code
```javascript
const {
  default: makeWASocket
} = require('@whiskeysockets/baileys');

const client = makeWASocket({
  browser: ['Ubuntu', 'Chrome', '20.00.1'],
  printQRInTerminal: true
})
```

## Connect With Number
```javascript
const {
  default: makeWASocket,
  fetchLatestWAWebVersion
} = require('@whiskeysockets/baileys');

const client = makeWASocket({
  browser: ['Ubuntu', 'Chrome', '20.00.1'],
  printQRInTerminal: false,
  version: fetchLatestWAWebVersion()
  // Other options
});

const number = "628XXXXX";
const code = await client.requestPairingCode(number.trim) /* Use : (number, "YYYYYYYY") for custom-pairing */

console.log("Ur pairing code : " + code)
```

# Sending messages

## send orderMessage
```javascript
const fs = require('fs');
const ZeppImg = fs.readFileSync('./ZeppImage');

await client.sendMessage(m.chat, {
  thumbnail: ZeppImg,
  message: "Gotta get a grip",
  orderTitle: "7eppeli-Corporation",
  totalAmount1000: 72502,
  totalCurrencyCode: "IDR"
}, { quoted:m })
```

## send pollResultSnapshotMessage
```javascript
await client.sendMessage(m.chat, {
  pollResultMessage: {
    name: "7eppeli-Corporation",
    options: [
      {
        optionName: "poll 1"
      },
      {
        optionName: "poll 2"
      }
    ],
    newsletter: {
      newsletterName: "7eppeli | Killer Queen Information",
      newsletterJid: "1@newsletter"
    }
  }
})
```

## send productMessage
```javascript
await client.relayMessage(m.chat, {
  productMessage {
    title: "7eppeli.pdf",
    description: "zZZ...",
    thumbnail: { url: "./ZeppImage" },
    productId: "EXAMPLE_TOKEN",
    retailerId: "EXAMPLE_RETAILER_ID",
    url: "https://t.me/YuukeyD7eppeli",
    body: "Nak Tido",
    footer: "Footer",
    buttons: [
      {
        name: "cta_url",
        buttonParamsJson: "{\"display_text\":\"7eppeli-Pdf\",\"url\":\"https://t.me/YuukeyD7eppeli\"}"
      }
    ],
    priceAmount1000: 72502,
    currencyCode: "IDR"
  }
})
```

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a> <a href="https://nodejs.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original-wordmark.svg" alt="nodejs" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> </p>

<p><img align="left" src="https://github-readme-stats.vercel.app/api/top-langs?username=dryzxmods&show_icons=true&locale=en&layout=compact" alt="dryzxmods" /></p>

<p>&nbsp;<img align="center" src="https://github-readme-stats.vercel.app/api?username=dryzxmods&show_icons=true&locale=en" alt="dryzxmods" /></p>

<p><img align="center" src="https://github-readme-streak-stats.herokuapp.com/?user=dryzxmods&" alt="dryzxmods" /></p>
Follow https://t.me/TenkaWaBails kalau mau liat type message yg lain :v
