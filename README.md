[TOC]

# EVT Guide



## 1. Introduction

### 1.1 What's EVT

EVT protocol and EVT contract

### 1.2 Why do we need EVT



### 1.3 EVT vs NFT



### 1.4 Quick Start



## 2. Architecture

![EVT Architecture](./res/evt.png)

### 2.1 Steps



### 2.2 EVT Components

#### 2.2.1 EVT-libs

Summary

#### 2.2.2 NewKeeper

Summary

#### 2.2.3 NewPlayer

Summary

## 3. Technology

### 3.1 Token standards

### 3.2 Decentralized Storage

### 3.3 Content protection



## 4. Tutorials

### 4.1 Build Your EVT

#### 4.1.1 Create a movie EVT



#### 4.1.2 Create a music EVT



### 4.2 How to integration

### 4.2.1 Summary

- Upload Media Source to EVT Commander.

- EVT Commander job:
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

### 4.2.2 NewPlayer SDK

- [Android SDK & demo](https://gitlab.weinvent.org/weinvent/incubator/evt-integration/evt-player-android)
- [iOS SDK & demo](https://gitlab.weinvent.org/weinvent/incubator/evt-integration/evt-player-ios)(https://gitlab.weinvent.org/wave/business/wave-websites/EVT-player-android)

### 4.2.3 NewKeeper authorization

- [NewKeeper API & demo](https://github.com/newtonproject/evt-integration-newkeeper)

## 5. Development

### 5.1 [EVT-lib](https://github.com/newtonproject/EVT-lib)

Library for EVT development.

- Standard implementation of EVT
- Example contracts for using EVT
- Factory for EVT industry application

### 5.2 Industry metadata



### 5.3 [EVT-toolchain](https://github.com/newtonproject/EVT-toolchain)

In this toolchain, you can use some simple shell command line to deploy contract, create EVT, call EVT Encryption functions, call EVT Variable functions. etc.

### 5.4 Newkeeper

- Save encrypt key
- Check EVT permission by address
- Dispatch EVT `encrypt key`

### 5.5 EVT Commander

- Create wallet
- Slice media source
- Encrypt media source
- Create EVT Contract
- Register key & EVT contract to NewKeeper

### 5.6 NewPlayer

- Decode media sorce.

- Play media source.

## 6. FAQ



## 7. Future

### 7.1 NewKeeper



#### 7.1.1 Decentralized key management



#### 7.1.2 P2P Distribution
