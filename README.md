# EVT Guide


## 1. EVT Architecture

![EVT Architecture](./res/EVT.png)

## 2 EVT Components & Tools

### 2.1 Movie Commander

- Create wallet
- Slice media source
- Encrypt media source
- Create EVT Contract
- Register key & EVT contract to NewKeeper

### 2.2 NewKeeper

- Save encrypt key
- Check EVT permission by address
- Dispatch EVT `encrypt key`

### 2.3 NewPlayer

- Decode media sorce
- Play media source.

### 2.4 [EVT-libs](https://github.com/newtonproject/EVT-lib)

Library for EVT development.
- Standard implementation of EVT
- Example contracts for using EVT
- Factory for EVT industry application

### 2.5 [EVT-toolchain](https://github.com/newtonproject/EVT-toolchain)

In this toolchain, you can use some simple shell command line to deploy contract, create EVT, call EVT Encryption functions, call EVT Variable functions. etc.

## 3 How to integration

### 3.1 Summary

- Upload Media Source(mp4,...) to Movie Commander.

- Movie Commander job:
  - create new wallet; 
  - recharge `NEW` to wallet address;
  - slice media source;
  - generate random secret;
  - use `secret key` encrypt `sliced media source`;
  - upload `encrypted media source ` to CDN/IPFS/...;
  - deploy media source EVT contract;
  - register `secret key` and `EVT contract` to `NewKeeper`;
  - get `EVT contract address`.

- User call `mint` to mint EVT;

- User get `token uri` from `EVT contract address`, then fetch `secret key` from `NewKeeper`;

- Provide `player link` & `secret key` to `NewPlayer` and you can play the `media source`.

### 3.2 Android
- [demo & doc](https://gitlab.weinvent.org/wave/business/wave-websites/EVT-player-android)
### 3.3 iOS
- [demo & doc](https://gitlab.weinvent.org/wave/business/wave-websites/EVT-player-ios)

### 3.4 Server

### 3.5 F&Q


## 4. Build Your EVT
