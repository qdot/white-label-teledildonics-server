# White Label Teledildonics

## About

An absolutely generic teledildonics based chat server that is absolutely not based off a quick hack of a [furry yiff server](https://github.com/kisuka/YiffSpot) with [Buttplug](https://github.com/buttplugio/buttplug-js) bolted onto it. 

WHAT. 

STOP LOOKING AT ME LIKE THAT.

## Installation

```bash
npm install
```
## Usage

### Glitch.com

To us our prebuilt instance on glitch:

- Go to https://metafetish-white-label-teledildonics-server.glitch.me
- You will be matched with random people. Please do not teledildonics them without knowing who they are. That could be bad otherwise.

To spin up your own server instance on glitch (so you could use it with someone else with whom you have shared the URL):

- Go to https://glitch.com/~metafetish-white-label-teledildonics-server
- Hit View Source
- Click on project name in upper right
- Hit "Remix Project"
- Change the name of config.example.js to config.js
- Change server name in config.js to the url of your glitch project, like so:

```javascript
module.exports = {
  "host": 'https://metafetish-white-label-teledildonics-server.glitch.me',
  "page_title": 'GENERIC TELEDILDONICS FOR GENERIC USERS',
  "debug": false,
  "http_port": process.env.PORT || 3000,
  "https_port": process.env.PORT || 3443,
  "ssl_enabled": false,
  "ssl_key": "",
  "ssl_crt": "",
  "redis_user": "",
  "redis_password": "",
  "redis_host": "localhost",
  "redis_port": 6379
}
```

### Production on own server

```bash
npm run launch
```

### Development on own server

This starts the server in development mode, which watches the source files for changes and re-builds automatically.

```bash
npm run dev
```

## License

[MIT](LICENSE)
