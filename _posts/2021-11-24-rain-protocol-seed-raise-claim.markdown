---
layout: single
title:  "Rain Protocol: Seed, Fund, Raise"
date:   2021-11-24 13:00:23 +0000
categories: rain general
---

## Intro

On a traditional raise platform, such as [Seedrs][seedrs], those wanting to raise funds for a project, must go through a ‘vetting process’ which is entirely at the discretion of the centralised platform on which the Project wants to raise.

Web3 (decentralised) platforms unlock the possibility for changing this dynamic between Project Creators and the Platforms on which they want to Raise, in that Platform Creators can create spaces which are more community owned and managed.

Rain Protocol is the underlying facilitator of Platforms (such as [Polygen][polygen]), which aim to create these kind of community owned spaces for creating Raises for any type of Project to which the Platform decides to tailor itself.

## Mechanics of Decentralised Platforms

Decentralised Platforms built on Rain protocol, have to operate slightly differently to traditional Platforms, by the very nature of the fact that they are controlled and operated by smart contracts.

Rain Protocol, lets Platforms integrate a 3 step process for enabling Project Creators to raise funds for their Projects: Seed, Raise, Claim. The ‘Claim’ phase is similar to the traditional step where Shareholders cash out, and Raise is similar to where Buyers will buy shares.

The ‘Seed’ Phase is slightly different, but is a necessary component because of the decentralised nature of these Platforms. The Seed phase is a way in which Projects are sort of ‘underwritten’ (to use legal terminology), but with significantly less risk to the Underwriter/Seeder.

## Underwriting/Seeding

Technically, there is no risk to an ‘Underwriter/Seeder’ of a project during the ‘Seed’ phase (except in the case of a hack), as they will be able to claim back the exact amount with which they helped to Seed the Project whether or not a target Raise has been successful.

In the case of a successful Raise (i.e. a Project meets the set target in terms of raised funds), the Underwriter/Seeder who helped the project via a Seed fund, will be rewarded with an amount that is taken as a percentage from the Raise that has occurred.

In this next section, will will outline, with some diagrams, what exactly is happening during these phases, and how - together with the use of - Balancer Protocol smart contracts, Platforms can use the Rain Protocol to help Projects Raise funds in a community owned way.

## 1. Seed Phase

![Seed Phase](https://assets.unegma.net/rainprotocol.xyz/blog/seed-phase.png "Seed Phase")

In this Phase, the Underwriter/Seeder (who is any User interacting with the platform via a Web3 wallet such as Metamask), will put in a Reserve currency (such as USDT or Wrapped Eth), in exchange for a ‘Seed Token’ representing their right to claim back their Seed amount later (plus reward if successful).

## 2. Raise Phase

![Raise Phase](https://assets.unegma.net/rainprotocol.xyz/blog/raise-phase.png "Raise Phase")

After the Seed phase is complete, (ie the Seed amount set by the Project Creator is gathered), the Raise phase is started. Please be aware that ANYONE can trigger the Raise phase once the full Seed is gathered.

Under the hood, Rain Protocol uses a special ‘Trust’ smart contract, which will automatically move the Reserve amount (earlier provided by the Underwriter/Seeder) into a Balancer liquidity pool, along with newly minted Project Specific ‘Share’ tokens, in order to fulfil the [AMM a+b=k][amm].

## 2. Raise: Funding The Raise

![Raise: Funding The Raise](https://assets.unegma.net/rainprotocol.xyz/blog/raise-funding-the-raise.png "Raise: Funding The Raise")

During the Raise phase, users will be able to continually add tokens of a desired type, initially set during the Seed Phase (e.g. USDT), in exchange for Project specific tokens representing a share in that Project. The Balancer contract will then govern the rising and falling price of the Token.

Please be aware that as these Project specific tokens have been automatically created by the Trust contract, their utility will be limited, and so it may be necessary to use them as a temporary placeholder for which relevant users are given an officially issued utility token later on (or NFT or in person gift etc).

## 2. Raise: Ending a Raise

![Raise: Ending a Raise](https://assets.unegma.net/rainprotocol.xyz/blog/raise-ending-a-raise.png "Raise: Ending a Raise")

If a Raise is successful, i.e. it meets the ‘minimum threshold’ or is higher, the Trust smart contract will automatically send the raised amount (in e.g. USDT), to the Project Creator, as well as returning to the Underwriter/Seeder their original fee + reward amount.

At this stage, it is important to note that the Trust will also burn any unsold Project specific tokens, and so the Project specific tokens owned by Raisers will now represent 100% of the shares in the project. These Project Specific tokens are then frozen so they can’t be traded.

Now that the Project Creator is able to see a list of the share holder addresses (due to the open nature of blockchains), they can then decide how they will reward these shareholders in whatever way they had originally promised in the project description.

This ‘reward’ to Shareholders could be anything from real-life tickets to a gig performed by the Project Owner, to ‘Tiered access’ to a DAO (more to come on this in future articles). In this way, Project tokens don’t necessarily have to mean ‘Securities’ in certain jurisdictions.

## 2. Raise: Failed Raises

![Raise: Failed Raises](https://assets.unegma.net/rainprotocol.xyz/blog/raise-failed-raises.png "Raise: Failed Raises")

The only other, slightly different scenario, is in the case of a failed raise, in which the original amount will be transferred by the Trust contract to the Underwriter/Seeder (at no cost to them), and the Raised amounts transferred back to the Users who provided the capital.

## 3. Claim (when Raise is Successful)

And that is it, the Project Creator now has their raised funds (transferred automatically by the Rain Trust smart contract), the Raisers have their project specific tokens (likely to be replaced by the Project Creator), and the Seeder has their original Seed amount plus reward.


[seedrs]: https://www.seedrs.com
[polygen]: https://polygen.io
[amm]: https://www.youtube.com/watch?v=1PbZMudPP5E



