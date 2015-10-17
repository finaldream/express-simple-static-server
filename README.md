# express-simple-static-server
Simple Express.js server for serving local static content.
Helps e.g. with testing static site content in the local development process.

## Installation

`npm install --save-dev express-simple-static-server`

## Usage

```
Usage: static-server [options] <content-dir>

Simple Express.js server for serving local static content.

Options:

  -h, --help              output usage information
  -V, --version           output the version number
  -a, --address <value>.  Address to listen to [127.0.0.1]
  -p, --port <value>.     Port to listen to [3000]
```

## Examples

Serving a local folder `./content` to localhost:3000
```
static-server content

> Serving content from http://127.0.0.1:3000
```

Serving to a different port
```
static-server -p 2856 content

> Serving content from http://127.0.0.1:2856
```

Serving to different address and port:
```
static-server -a 192.168.2.100 -p 2856 content/htdocs

> Serving content from http://192.168.2.100:2856
```
