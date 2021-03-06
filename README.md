YakYak
======

[![Build Status](https://travis-ci.org/yakyak/yakyak.svg)](https://travis-ci.org/yakyak/yakyak) [![Gitter](https://d378bf3rn661mp.cloudfront.net/gitter.svg)](https://gitter.im/yakyak/yakyak)

Desktop client for Google Hangouts

![sshot](https://cloud.githubusercontent.com/assets/123929/16032313/cdba46c2-3204-11e6-912f-a72fef60563a.png)

(This app is in no way associated with or endorsed by Google)

## Install it

We provide [prebuilt binaries](https://github.com/yakyak/yakyak/releases) for Mac OS X, Linux 32 / 64 and Windows 32 / 64.

This is the [latest release](https://github.com/yakyak/yakyak/releases/latest).
We love [bug reports](https://github.com/yakyak/yakyak/issues)!

## What does it do:

* Send/receive chat messages
* Create/change conversations (rename, add people)
* Leave/delete conversation
* Notifications (using native OS notifications)
* Toggle notifications on/off
* Drag-drop, copy-paste or attach-button for image upload.
* Hangupsbot sync room aware (no bot name, proper user pics)
* Show inline images
* Send presence/focus/typing/activeclient to behave like a proper client
* History scrollback
* Video/audio integration (open in chrome)
* Focus/typing indications (mainly a design issue. keep it clean)
* Offer alternative color schemes

![sshot1](https://cloud.githubusercontent.com/assets/123929/16032393/991d63f8-3205-11e6-98bf-31f1b57cdc96.png)

![sshot2](https://cloud.githubusercontent.com/assets/123929/16032394/9e2ac08e-3205-11e6-81cc-fd4cb37441b5.png)


## Credits

#### Main authors

* [Davide Bertola](https://github.com/davibe)
* [Martin Algesten](https://github.com/algesten)

#### Contributors

* [David Banham](https://github.com/davidbanham)
* [Max Kueng](https://github.com/maxkueng)
* [Arnaud Riu](https://github.com/arnriu)
* [Austin Guevara](https://github.com/austin-guevara)
* [André Veríssimo](https://github.com/averissimo)

## Developing

This is an open source project. Please help us!

It is written in coffeescript (nodejs) based on
[hangupsjs](https://github.com/algesten/hangupsjs) using
[trifl](http://algesten.github.io/trifl/) on top of
[electron (atom shell)](https://github.com/electron/electron).

### Setup

Requirements:

- Node.js (v4 or v6)

```bash
$ npm install
$ npm run gulp
```

### Continuous build

```bash
$ npm run gulp watch
```

### Run it

```bash
$ npm run electron app
```

### Build Binaries for Deployment

*Supported platforms:* Windows (*win32*), Mac OS X (*darwin*), Linux (*linux*)

*Suported architectures:* 64-bits (*x64*), 32-bits (*ia32*)

```bash
# Building for all platforms and architectures
$ npm run deploy

# You can also build specific builds by using
#  deploy:<platform>-<architecture>
# example:
$ npm run deploy:darwin-x64
```

*note:* if you are building *Windows* binaries in *Linux* or *Mac OS X*, Wine (1.6 or higher) must be installed. It also requires a 32-bit Wine installation when building Windows 32-bit binary.

### Structure

| Location  | Description                              |
|-----------|------------------------------------------|
| `src/`    | Is where sources live                    |
| `src/ui/` | Holds renderer code (client side)        |
| `dist/`   | Everything is compiled to this directory |

### Acknowledgement 

- All the users and developers of YakYak
- ["You wouldn't believe"](https://notificationsounds.com/notification-sounds/you-wouldnt-believe-510) as the 'new message' sound for some platforms and is licensed under CC
