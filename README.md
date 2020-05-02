# DoW: DApp Over WebRTC

## Overview

The idea is to use WebRTC to share sites and data to build a highly-decentralized and free internet by automatically and transparently using *all* connected devices as nodes.

### DApps

DApps (Decentralized Applications) are the future of internet. Central servers can suffer several kinds of attacks, natural and governmental interventions, data transfer issues etc. If sites can be spread along several servers around the globe, they can be highly available and faster.

### Blockchains and other DLTs

The coming of programmable blockchains, like Ethereum and others, opened a huge market for dapps. Several blockchain alternatives has been developed, like holochain, hashgraph, dag, tangle etc. They are referred to as [Distributed Ledger Technology (DLT)](https://101blockchains.com/blockchain-vs-hashgraph-vs-dag-vs-holochain/).

However, DLTs have some drawbacks:
* Programming DLTs is not straightforward; developers must learn new languages and paradigmas (blockchains etc.).
* It's necessary to create and maintain digital wallets to serve and to use dapps. Managing wallets is not easy for most users (it's not as simple as typing username and password).
* It's necessary to pay some value in cryptocurrency tokens to use dapps. This requirement turns difficult to build free services for users. Most users won't buy cryptocurrencies.
* Some DLTs require users to download and install software in order to use them, which is a barrier for non-technical users.

### Zeronet

[Zeronet](https://zeronet.io) is an interesting alternative to DLTs, since it has some advantages:
* It's free: users share their storage and bandwidth to serve pages.
* No need of wallets.
* No need of buying cryptoassets (except for namecoin if the developer wants to register a prettier domain name).
* It uses well-known languages like Javascript and MySQL.
* Auto-login for zeronet sites.
* It's very easy to be a node.
* No expensive hardware/bandwidth requirements.

The downsides of Zeronet are:
* User still must download and install Zeronet software in order to use it, and it's not available for all common platforms/OS (e.g. iOS).
* For proxies and multiuser sites, user must insert the private key as login, but it's not well documented how to get the own private key.
* http, not https.

### WebRTC

[WebRTC](https://webrtc.org/) is a technology which permits to exchange data between browsers in a p2p fashion. It was designed to share media streams, but it works with any kind of data. So it can be used to share apps/sites and their data.

WebRTC still uses some auxiliary servers for signaling and NAT-traversaling, but also ZeroNet uses trackers to find peers.

### Requeriments for DoW

* Must work offline.
* Free: users already pay for their devices and internet.
* Zero installation.
* Automatic use in all devices.

One important note here. DoW is not intended for anonimity. No effort will be made to hide the authors of contents, as of most sites works so. The main goal here is to serve apps and data in a decentralized way, for free, transparently for users.

### Security concerns

Apps cannot be made directly in JS because it could easily get access to private data somewhere below `window` or `document`; so it's necessary to build an auxiliary safer language for DApps.

### Next steps

Next step is to develop a simple app to testify the viability of building dapps over WebRTC.

See [Offline Wiki](https://github.com/sonysantos/offline-wiki/).
