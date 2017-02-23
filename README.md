# Project Hermes
Used for creating First Screen (1Screen) LPP landing page.

### How to setup:
------
* Download, Fork, or Clone this repo
* `npm install`
* Create a new file on `root` name `./config.json` and copy the following:
```
{
    "ipAddress" : "192.168.1.11",
    "port" : "7070",
    "creatives" : "creatives",
    "creativeName" : "KeyToHappiness",
    "country" : "TR",
    "operatorId" : "_300",
    "previewHtml" : "preview.html",
    "defaultHtml" : "default.html",
    "indexHtml" : "index.html"
}
```

### Where:
------
* `ipAddress`: is your device IP ipAddres
* `port`: your prefered port
* `creative`: creative folder
* `creativeName`: creative name that your working on
* `country`: country iso alpha-2 code in capital letters
* `operatorId`: operator ID, for multiple operator you can do "_100_200_300"
* `previewHtml`: html file for preview, no need to change this
* `defaultHtml`: html file for subscription flow, no need to change this
* `indexHtml`: html file for creative, no need to change this

### Commands:
------

`gulp`

Default, this will create the server, watch for file changes and reload the page, open page your working on.

`gulp deploy`

This command will split your `preview.html`, separate subscription flow to `default.html` and creative to `index.html`.