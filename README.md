<h1 align="center">
    Hardhat Defi
</h1>

<br/>

This repository explains how to build a programmatic lending and borrowing project

<hr/>
 
## 🗎&nbsp; Requirements
- [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
    You'll know you did it right if you can run `git --version` and you see a response like `git version x.x.x`
    
- [Nodejs](https://nodejs.org/en/)

    You'll know you've installed nodejs right if you can run: `node --version` and get an ouput like: `vx.x.x`
- [Yarn](https://yarnpkg.com/getting-started/install) instead of `npm`
   
   You'll know you've installed yarn right if you can run: `yarn --version` and get an output like: `x.x.x`
   
   You might need to [install it with `npm`](https://classic.yarnpkg.com/lang/en/docs/install/) or `corepack`

## 🛠️&nbsp; How to run
- Clone the repo:
    ```
    git clone https://github.com/Meno96/hardhat-defi.git
    ```
- Enter the directory:
    ```
    cd hardhat-defi
    ```
- Install packages:
    ```
    yarn
    ```
    
## 🚀&nbsp; How it's suppose to work?

This repo requires a mainnet rpc provider, but don't worry! You won't need to spend any real money. We are going to be `forking` mainnet, and pretend as if we are interacting with mainnet contracts. 

All you'll need, is to set a `MAINNET_RPC_URL` environment variable in a `.env` file that you create. You can get setup with one for free from [Alchemy](https://alchemy.com/?a=673c802981)

Run:

```
yarn hardhat run scripts/aaveBorrow.js
```

### Running on a testnet or mainnet

- Setup environment variabltes

You'll want to set your `GOERLI_RPC_URL` and `PRIVATE_KEY` as environment variables. You can add them to a `.env` file, similar to what you see in `.env.example`.

  - `PRIVATE_KEY`: The private key of your account (like from [Metamask](https://metamask.io/)). **NOTE:** FOR DEVELOPMENT, PLEASE USE A KEY THAT DOESN'T HAVE ANY REAL FUNDS ASSOCIATED WITH IT.
    - You can [learn how to export it here](https://metamask.zendesk.com/hc/en-us/articles/360015289632-How-to-Export-an-Account-Private-Key).
  - `GOERLI_RPC_URL`: This is url of the goerli testnet node you're working with. You can get setup with one for free from [Alchemy](https://alchemy.com/?a=673c802981)

- Get testnet ETH

Head over to [faucets.chain.link](https://faucets.chain.link/) and get some tesnet ETH. You should see the ETH show up in your metamask.

- Run

```
yarn hardhat run scripts/aaveBorrow.js --network goerli
```

## Linting

To check linting / code formatting:
```
yarn lint
```
or, to fix: 
```
yarn lint:fix
```

## Formatting

```
yarn format
```

## 📫&nbsp; Have a question? Want to chat? 

[LinkedIn](https://www.linkedin.com/in/daniele-menin/)

[Instagram](https://www.instagram.com/danielemeno96/)
