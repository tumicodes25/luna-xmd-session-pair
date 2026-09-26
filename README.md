# Session Id Generator For WhatsApp Bots (Encoded Session)

**This service no longer uses Mega.nz.**
Credentials are encoded in base64 and sent directly over WhatsApp.


**How the session encoding works**

The pairing endpoint now reads the generated `creds.json` file, encodes its contents in base64, and sends that string directly to the WhatsApp account that completed the pairing.

On the receiving side you can decode the message back into JSON and save it as `creds.json`. For example:

```js
import { writeFileSync } from 'fs';

// `encoded` is the text WhatsApp message you received
const json = Buffer.from(encoded, 'base64').toString('utf8');
writeFileSync('creds.json', json);
```

This eliminates the dependence on any external storage service.

CRAFTED USING TEMPLATES OF SUHAILTECHINFO ( QR )  AND PRABATH ( PAIR )

BOTH PAIR CODE AND QR CODE WORKING

YOU CAN DEPLOY IT ON ANY CLOUD PLATFORM e.g `HEROKU` `RENDER` `KOYEB` etc.

**⭐ THE REPO IF YOU ARE GOING TO COPY OR FORK**


## OTHER PROJECTS:

- [PASTE SESSION](https://github.com/GlobalTechInfo/PAIRING-WEB)
- [WHATSAPP BOT](https://github.com/GlobalTechInfo/MEGA-AI)
- [TELEGRAM BOT](https://github.com/GlobalTechInfo/TELEGRAM-AI#readme)



| [![Qasim Ali](https://github.com/GlobalTechInfo.png?size=100)](https://github.com/GlobalTechInfo) |
| --- |
| [Qasim Ali](https://github.com/GlobalTechInfo) |
