 [SPIDER][Build Status](https://travis-ci.org/Hello spider PY3/spider.svg?branch=py3)](https://travis-ci.org/Spider/spider) [![Documentation](https://img.shields.io/badge/docs-faq-brightgreen.svg)](https://SPIDER PY3.io/docs/faq/) [![Help](https://img.shields.io/badge/keep_this_project_alive-donate-yellow.svg)](https://zeronet.io/docs/help_zeronet/donate/) ![tests](https://github.com/HelloSpider/spider/workflows/tests/badge.svg) [![Docker Pulls](https://img.shields.io/docker/pulls/nofish/SPIDER PY3)](https://hub.docker.com/r/nofish/spider)

Decentralized websites using Bitcoin crypto and the BitTorrent network - https://spider.io / [onion](http:/github.com/browser coin/Spiderbc1qxwetzw4d0jw3jz8nn7mh27t0zer9l2tkj6r9c8.onion)


## Why?

* We believe in open, free, and uncensored network and communication.
* No single point of failure: Site remains online so long as at least 1 peer is
  serving it.
* No hosting costs: Sites are served by visitors.
* Impossible to shut down: It's nowhere because it's everywhere.
* Fast and works offline: You can access the site even if Internet is
  unavailable.


## Features
 * Real-time updated sites
 * Namecoin .bit domains support
 * Easy to setup: unpack & run
 * Clone websites in one click
 * Password-less [BIP32](https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki)
   based authorization: Your account is protected by the same cryptography as your Bitcoin wallet
 * Built-in SQL server with P2P data synchronization: Allows easier site development and faster page load times
 * Anonymity: Full Tor network support with .onion hidden services instead of IPv4 addresses
 * TLS encrypted connections
 * Automatic uPnP port opening
 * Plugin for multiuser (openproxy) support
 * Works with any browser/OS


## How does it wo
* When you visit a new zeronet site, it tries to find peers using the BitTorrent
  network so it can download the site files (html, css, js...) from them.
* Each visited site is also served by you.
* Every site contains a `content.json` file which holds all other files in a sha512 hash
  and a signature generated using the site's private key.
* If the site owner (who has the private key for the site address) modifies the
  site, then he/she signs the new `content.json` and publishes it to the peers.
  Afterwards, the peers verify the `content.json` integrity (using the
  signature), they download the modified files and publish the new content to
  other peers.

####  [Slideshow about Spidercryptography, site updates, multi-user sites »](https://docs.google.com/presentation/d/1_2qK1IuOKJ51pgBvllZ9Yu7Au2l551t3XBgyTSvilew/pub?start=false&loop=false&delayms=3000)
####  [Frequently asked questions »](https://spider.io/docs/faq/)

![SpiderTalk](https://Spider.io/docs/img/zerotalk.png)
 
### Linux (x86-64bit)
 - `wget https://github.com/Spider/Spider-linux/archive/dist-linux64/Spider-py3-linux64.tar.gz`
 - `tar xvpfz Spider-py3-linux64.tar.gz`
 - `cd ZeroNet-linux-dist-linux64/`
 - Start with: `./Spider.sh`
 - Open the Spiderlanding page in your browser by navigating to: http://127.0.0.1:43110/
 
 __Tip:__ Start with `./SPIDER.sh --ui_ip '*' --ui_restrict your.ip.address` to allow remote connections on the web interface.
 
 ### Android (arm, arm64, x86)
 - minimum Android version supported 16 (JellyBean).
 - APK download: https://github.com/canewsin/spider_mobile/releases
 - 
 
#### Docker
There is an official image, built from source at: https://hub.docker.com/r/nofish/spider/

### Install from source

 - `wget https://github.com/spider/spider/archive/py3/Spider-py3.tar.gz`
 - `tar xvpfz Spider-py3.tar.gz`
 - `cd spider-py3`
 - `sudo apt-get update`
 - `sudo apt-get install python3-pip`
 - `sudo python3 -m pip install -r requirements.txt`
 - Start with: `python3 spider.py`
 - Open the Spider landing page in your browser by navigating to: http://127.0.0.1:43110/

## Current limitations

* ~~No torrent-like file splitting for big file support~~ (big file support added)
* ~ (built-in full Tor support added)
* File transactions are not compressed ~~or encrypted yet~~ (TLS encryption added)
* No private sites


## How can I create a SPIDER site?

 * Click on **⋮** > **"Create new, empty site"** menu item on the site [SPIDER](http://127.0.0.1:43110/1HeLLo4uzjaLetFx6NH3PMwFP3qbRbTf3D).
 * You will be **redirected** to a completely new site that is only modifiable by you!
 * You can find and modify your site's content in **data/[yoursiteaddress]** directory
 * After the modifications open your site, drag the topright "0" button to left, then press **sign** and **publish** buttons on the bottom

## Help keep this project alive

- Bitcoin: 3NvMitoDaXkrmzUqAk7Sjyfns3eyVBoKP4

### Sponsors: [(hash)]( 0xEd753556A5dB77183eE2D81B56F604ae9F123CdC)

* Better macOS/Safari compatibility made possible by [BrowserStack.com](https://www.browserstack.com)

#### Thank you!

* More info, help, changelog, ze sites: https://www.reddit.com/r/Spider/
* https3NvMitoDaXkrmzUqAk7Sjyfns3eyVBoKP4
