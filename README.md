# Notica
Send browser notifications from your terminal. No installation. No registration.

https://notica.us/

## Usage

Notica is a Bash function / alias that sends a notification to a tab in your browser when it's ran:

```
$ long-running-command; notica Finished!
```

This will wait until the first command completes before running Notica.
That way you can go do other things while your long task runs.
Then you will recieve a notification on any devices that have the Notica website open.

![Notification Example gif](https://i.imgur.com/476ezFy.gif)

## Setup

Please follow the instructions on the Notica home page since they are generated specific to you:

https://notica.us/

## Source Code

### License

Notica is free and open-source software released under the MIT License.

### Self-hosting

Hosting Notica on your own server is extremely easy.
Clone this repository, change all notica.us URLs to your own domain, and then run `npm install && npm start`.
You can connect to it directly or through a reverse proxy.

### Usage

```text
Usage: npm start -- [options]
(After npm run build) Usage: node server.js [options]

  Options:

    -V, --version         output the version number
    -p, --port <port>     Host port (3000)
    -H, --host <IP>       Host IP (127.0.0.1)
    -U, --url <URL>       Website URL (https://notica.us)
    -t, --title <string>  Custom title ('Notification from Notica')
    -i, --icon <path>     Custom icon (img/icon.png)
    -h, --help            output usage information

  Example:

    $ npm start -- -p 80 -t 'My cool Title'
```
