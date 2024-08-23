# dApp lowest common multiple of two numbers
<a id="readme-top"></a>

<!-- PROJECT LOGO -->
## About
<p>
    This is decentralized application (dapp) for getting the lowest common multiple of two numbers. powered by <a href="https://docs.cartesi.io/cartesi-rollups/1.3/">cartesi</a> rollups technology.
</p>


## Getting Started

Below you'll find instructions on how to setup this DApp locally.

### Prerequisites

Here are some packages needed to successfully run this application on your PC:

* [NodeJS](https://nodejs.org/en), [npm](https://docs.npmjs.com/cli/v10/configuring-npm/install), [yarn](https://classic.yarnpkg.com/lang/en/docs/install/#debian-stable) 

* [Docker](https://docs.docker.com/get-docker/) 

* [Cartesi-CLI](https://docs.cartesi.io/cartesi-rollups/1.3/development/migration/#install-cartesi-cli)
  ```sh
  npm install -g @cartesi/cli
  ```

For Windows, its recommended to have Ubuntu WSL installed then installing docker on the Linux sub system. This article provide step by step guide on how to successfully install docker on Ubuntu WSL 2 [here](https://dev.to/bartr/install-docker-on-windows-subsystem-for-linux-v2-ubuntu-5dl7)

### Installation

1. Clone this repo
   ```sh
   git clone 
   ```
2. Install NPM packages
   ```sh
   yarn  install
   ```
3. Build and run the dapp via `cartesi-cli`
   ```sh
   cartesi build 
   ```
   and
   ```sh
   cartesi run 
   ```

## USAGE
#### Advanced handlers
```
description — fet the lowest common multiple for two given number.
parameters * — { firstNumber: int, secondNumber: int }
```

###### sample
```
{
     "data": {
        "firstNumber": 2,
        "secondNumber": 9
    }
}
```
###### Interact
Via `cartesi cli`, access your terminal in another window and input these instructions below:
```
cartesi send generic \
    --dapp=0xab7528bb862fb57e8a2bcd567a2e929a0be56a5e \
    --chain-id=31337 \
    --rpc-url=http://127.0.0.1:5000 \
    --mnemonic-passphrase='test test test test test test test test test test test junk' \
    --input=0x7b22616374696f6e223a2267656e657261746550617373776f7264222c202264617461223a7b226e756d4368617273223a2238222c20226e756d4e756d62657273223a2234227d7d
```
