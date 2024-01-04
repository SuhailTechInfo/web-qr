<h1 align="center"> WEB BASED MULTIDEVICE QR </h1>

  <html>
   <body>
  <p align="center">  
  <a aria-label="FORK" href="https://github.com/SuhailTechInfo/Secktor-bot/fork" target="_blank">
    <img alt="License: GPL-3" src="https://img.shields.io/github/stars/SuhailTechInfo/web-qr?style=social" target="_blank" />
  </a>
  <a aria-label="Suhail_Md is free to use" href="https://youtube.com/@suhailtechinfo" target="_blank">
    <img alt="SuhailTechInfo" src="https://img.shields.io/youtube/channel/subscribers/UCU071AMRqcd5mfTdCgJFwPg" target="_blank" />
  </a>
    <p align="center"><img src="https://profile-counter.glitch.me/{smd-web-qr}/count.svg" alt="SuhailTechInfo :: Visitor's Count" /></p>

     
  </body>
</html>


## Deployment Methods
---
1.  ***Click [`FORK`](https://github.com/SuhailTechInfo/web-qr/fork) and `Star ⭐ Repository` if you get help from repo.***
2.  ***Deploy on [`HEROKU`](https://dashboard.heroku.com/new?template=https://github.com/SuhailTechInfo/web-qr).***
3.  ***Deploy on [`REPLIT`](https://replit.com/github/SuhailTechInfo/web-qr).***
4. ***Deploy on [`RENDER`](https://dashboard.render.com/login).***
```
RENDER PROCESS:
    1: Click "NEW".
    2: Select "Web Service".
    3: Click "Build and deploy from a Git repository".
    4: Now Choose this forked git repo from list.
    5: And JUST CLICK "Connect". 
```




- Dependencies
```sh
    "@hapi/boom": "^10.0.1",
    "@whiskeysockets/baileys": "6.5.0",      
    "pino": "^8.1.0",
    "express": "^4.18.2",
    "qrcode": "latest"
```


- WASocket Options
```js
    let Smd =SuhailWASocket({ 
        printQRInTerminal: false,   // make it false if you're using web
        logger: pino({ level: "silent" }),     // make it silent to prevent baileys buffering
        browser: Browsers.baileys("Desktop"),  // awailable browsers : ubuntu, macOS, baileys.
        auth: state 
    });
```



- Getting Session in BASE64
```js
    let CREDS = fs.readFileSync(__dirname + '/auth_info_baileys/creds.json')
    var Scan_Id = Buffer.from(CREDS).toString('base64')    // converting into Base64 ---- IMPLEMENT ACCOEDING TO YOUR NEED
    // res.json({status:true,Scan_Id })
```




- Environment variable
```js
    const PORT = process.env.PORT ||  5000
    const MESSAGE = process.env.MESSAGE || "Don't Provide your session id to someone!" 
    //   Set Confirmation Message According to your need! 
```









## MADE WITH ❤️
[![SuhailTechIinfo](https://github.com/SuhailTechInfo.png?size=300)](https://github.com/SuhailTechInfo)
