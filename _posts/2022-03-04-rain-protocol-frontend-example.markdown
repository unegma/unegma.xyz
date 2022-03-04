---
layout: single
title:  "Rain Protocol: Frontend Example"
date:   2022-02-21 14:00:23 +0000
categories: development
---

## Intro

For this tutorial, we will go through setting up a frontend example app which interacts with Rain GatedNFT contracts.

After this tutorial, you will be able to see how a frontend app can interact with Rain tooling.

## Setting up the Environment

We won't go into too much detail on setting up (and differences between) `npm` and `npx` or on how to code in React, you can look this up yourself, but we will begin with automatically generating a basic template React app using `create-react-app`. Run `npx create-react-app --template typescript rain-frontend-example`. 

You will now have an example app which you can edit in the way you prefer. If you now run `npm start`, you should now be able to see the template app in your browser at http://localhost:3000/

Next we will install the [Ethers][ethers] library for interacting with an EVM compatible blockchain: `npm install ethers` and also Hardhat for setting up a test local blockchain: `npm install --save-dev @nomiclabs/hardhat-ethers @nomiclabs/hardhat-waffle hardhat`. To learn more about how to set up a Hardhat project, check out our [previous tutorial here][previous-tutorial].

[//]: # (todo does hardhat work with regular ethers?)
[//]: # (todo what is the best way to get the abi in or are we using typechain)
[//]: # (todo does josh use own connect button or a library?)

[discord]: https://discord.gg/dzYS3JSwDP
[ethers]: https://docs.ethers.io/
[hardhat]: https://hardhat.org/getting-started/

[//]: # (todo link here)
[previous-tutorial]: https://blog.rainprotocol.xyz
