# Ethereum Token
___
[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)
___
Ethereum tokens is a representation of any good that is tradable from a physical object to a native currency used . In the future, tokens may even be used to represent financial instruments like stocks and bonds. In this sprint you will be able to build your own currency token and transfer it

 - [Key Words](#key-words)
 - [High Level Goals of this Sprint](#high-level-goals-of-this-sprint)
 - [Getting Started and Project Set Up](#getting-started-and-project-set-up)
 - [The Curriculum](#the-curriculum)
    - [Project Lecture](#project-lecture)
    - [Useful Links](#useful-links)
 - [The Project](#the-project)
 - [Extra Credit](#extra-credit)

# Key Words
___
- Web3
- Solidity
- Smart Contracts
- Ganache
- Infura

# High Level Goals of this Sprint
---
- Learn Solidity and how to write ethereal smart contracts.
- Learn how to compile a contract with solidity compiler
- Learn how to test your smart contracts using Ganache
- Learn how to deploy your code on Rinkeby Test Network

# Getting Started and Project Set Up
___
## npm
This sprint uses [npm](https://www.npmjs.com/) to manage its dependencies. npm comes bundled with Node, and is another JavaScript package manager that makes it easy for developers to share and reuse code. Even though npm started in the Node ecosystem, it is quickly becoming the default choice for sharing all types of JavaScript code. 
what you need to do here is:
1. Install Node.js if you haven't yet.
2. Run `npm install`

## Solc
JavaScript bindings for the Solidity compiler, the compiler can produce a range of choices, from simple binaries To use the latest stable version of the Solidity compiler via Node.js you can install it via npm:

Run `npm install solc -save`

## npm scripts
npm comes with a handy scripting feature that lets you define shell commands inside of package.json, here in this project we set two scripts that you are going to use a lot. you can also define your own scripts if you feel the need to do so.

# The Curriculum
___
## Useful Links
___
- [ERC20 Token Standard](https://theethereum.wiki/w/index.php/ERC20_Token_Standard)
- [Web3 Documentation](https://web3js.readthedocs.io/en/1.0/)
- [Using Infura with web3.js](https://web3j.readthedocs.io/en/latest/infura.html)

## The Project
___
### Part One: EthToken
contracts/BCCoin.sol is the smart contract the when compiled and deployed; will represent your currency, to build this contract you need to achieve the following:
- First, get familiar with the contracts/Interface.sol file and try to understand its functions with their parameters and answer the following question, what does this interface represent? and why do we use it?
*Don’t add/delete comments in this file or you will get errors because they are considered part of the code

- Run `npm run test`
  To Pass the Tests:
    - Start by implementing the functions declared in contracts/Interface.sol, inside contracts/BCCoin.sol file
    *Hint: The commented line in compile.js file will help you to fix your contract errors.
    - Implement getTokens(), getEthers() functions which will let the sender buy and sell his tokens. 
    By completing the above, you've written the smart contract of your token, now it's the time to compile the code and deploy it.
    - inside of compile.js, you'll find the the compilation code written for you, read it carefully and understand it.
    - in the file Deploy.js you need to write the code that would deploy your compiled contract, in this project we are going to use the Rinkeby test network to depoly the contracts to it, and the hosted Ethereum node cluster, infura to achieve that.

## Part Two: Front-End
In order to interact with your contract, we built a simple front-end for you, your job is:

- Inside web3.js, to create an instance of Web3 with the right provider.
- to complete src/token.js
- Inside src/app.js,to fill the functions to make them work properly

## Extra Credit
- Think about a function you can add to let the owner generates new tokens if his balance is out of tokens
- Inside of Metamask on your browser, go to add token and try to add your token, does it work properly? what do you think is the reason of that? make the necessary changes in your contracts folder to make work on metamask.
