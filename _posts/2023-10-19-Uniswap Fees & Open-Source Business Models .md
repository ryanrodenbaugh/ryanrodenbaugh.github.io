---
layout: post
title: "Uniswap Fees & Open-Source Business Models"
date: 2023-10-19
categories: crypto
---

*This post originally appeared on the [Wallfacer Labs Substack](https://wallfacerlabs.substack.com/p/uniswap-fees-and-open-source-business-models)*

## Introduction

This week, Uniswap Labs announced that they would begin charging 15bps (0.15%) for a limited set of swaps that go through the popular uniswap.org interface and mobile wallet. 

This fee accrues value to Uniswap Labs (the company and its equity holders), but not the Uniswap Protocol (the protocol and its $UNI token holders). 

To state the obvious, it is well within Uniswap Lab's right to do this. They have made it clear for some time now that they ("Labs") are the owner of the front-end domain and Uniswap Wallet. The DAO is not.   

Additionally, Uniswap Labs raised hundreds of millions of dollars from investors in 2022 and it is perhaps a necessity to start generating revenues. 

Uniswap Labs's clear ownership of the frontend and mobile wallet has not stopped detractors from declaring their frustration about the fact that Labs is charging a fee (and accruing value) while the DAO is not.

In the crypto industry, there is a lack of precedent for a Labs company charging for services on top of an open-source protocol they also built. This makes it challenging to determine the correct approach. To make an informed judgment, let's explore the historical open-source business models and their relevance to crypto.

## The Reality of Open Source Contributions

One framework for thinking about any "DeFi Project" is open-source financial software with governance (and sometimes financial) rights attached in the form of a token. 

Still, many crypto projects are still plagued by the same issues that plague non-crypto open-source software ("OSS"). 

Types of Open Source Contributions: 

Open-source projects can be categorized into four buckets:

*(Many of the ideas in this section come from Working in Public: The Making and Maintenance of Open Source Software by Nadia Eghbal, which I would recommend!)*

Most crypto projects aspire to be federations (which are characterized as being many-to-many interactions) but get stuck relying on one core team and wind up as stadiums (or worse, toys). 

Given the historical problems that OSS projects have had creating the right incentives for people to participate, it should be no surprise that:

> "One study found that in more than 85% of the open-source projects the researchers examined on GitHub, less than 5% of developers were responsible for over 95% of code and social interactions."

The difficulty in attracting contributors in part comes from a lack of funding for OSS. As a result of some of these funding issues, many OSS projects have had to turn to sponsorships, donations, and the contributions of power users to stay alive. 

## Corporates/Sponsorship and OSS

In the realm of open-source software, major projects – often related to programming languages or development frameworks – attract the interest of large corporations. These companies may choose to sponsor OSS maintainers or undertake in-house contributions and maintenance.

Notable Examples:

- Jane Street + OCaml: As the largest corporate user of OCaml powering its trading systems, Jane Street has heavily invested in the language and contributed lots of open-source code. 

- NuBank + Clojure: NuBank bet early on a less popular programming language, Clojure, and has since gone on to acquire Cognitect, founded by Clojure's creator to promote the language's adoption.

- Facebook + React: Facebook remains the core maintainer of React, and continues to employ Jordan Walke who authored the widely used React program. 

## Bitcoin and Donations

The software that perhaps best embodies the term "open source" is Bitcoin. With a disappeared founder and no corporate entity attached to it, no single person or entity is "in charge of" Bitcoin. In place of a BDFL or official corporate sponsor, many independent sponsors have stood up to fund developers. A short list of examples: 

Square, Paradigm, Chaincode Labs, Brink, Bitmex, Coinbase, and many more.

This feels unique to Bitcoin given how many businesses drive revenue from Bitcoin (Square, Bitmex, Coinbase) or where individuals have had massive wealth generated as a result of Bitcoin (Chaincode, Brink). There are decent financial incentives to fund continued development. But it is still far from perfect.

## The State of Protocols and their Labs

Both the sponsorship and donation model are analogous to the relationship that "Labs" companies have with their respective protocols once they're launched. Today, Labs companies are closer to "donors", but should aspire to be "sponsors". Let me explain...

Compound Labs (as an example) has no legal (de jure) responsibility to improve the Compound Protocol. However, their community expects them to continue to improve the protocol (de facto responsibility). Employees and founders likely feel this responsibility and have the financial upside to do so (as they may still be individual holders of the token). 

Comparing Labs companies to corporate sponsors, there is one key difference:

- Jane Street's business relies on OCaml
- NuBank's business relies on Clojure
- Facebook's business relies on React
- Compound Labs does not have a profitable business built on top of the Compound Protocol

There isn't some revenue source that dries up at Compound Labs if Compound Protocol stops. 

As such, current Labs companies look more like "donors". Compound Labs and Uniswap Labs (for example) each raised venture dollars that went to their corporate entities (not their DAOs) and have been able to use that to fund the development of their protocols without being immediately concerned about revenue. Spending their time and resources on open-source protocols that they can't monetize can be viewed as a "donation". 

Once those dollars run out, some of these "Labs" companies need to actually ask their DAOs for tokens to compensate them for their work (as Aave Companies did following the release of V3). 

This "charitable" path is not sustainable and it should not be the path we aspire to as an industry.

## A Renaissance in Open Source Software (OSS)

As outlined, for most of the history of open-source software, funding models have been bleak. 

OSS has relied on generous people who spend time as maintainers or on the kindness of corporations and wealthy benefactors. 

Over the past 20 years though this has begun to change with a flourishing in OSS business models. 

Diving into commercialization efforts, a16z lays out the three stages:

### Open Source 0.0 - The Free Software Era (the 1970s-1990s)

Software was created by academics and hobbyists with a focus on offering it for free. The idea of a business model was absent, and any funding for "free software" typically came from university or corporate research grants.

### Open Source 1.0 - The Support and Services Era (the 1990s-2000s)

The initial business model introduced paid support and services for free software by companies like RedHat and MySQL. Notably, open-source companies had significantly lower value compared to their closed-source counterparts, such as RedHat versus Microsoft or MySQL versus Oracle. 

### Open Source 2.0 - The SaaS & Open Core Era (2000s - Today)

Once users could host open-source services in the cloud, users no longer distinguished between open-source and proprietary software. Companies could leave the core of the code open-source ("open-core") and add value-added proprietary services on top. 

As a result of the Open Source 2.0 model of hosted open-source software being positioned as SaaS, open-source companies have been able to attain valuations similar to their proprietary counterparts. 

## Open Source 2.0 (but make it crypto)?

The "Labs" entities associated with crypto companies (Uniswap Labs, Compound Labs), could certainly try to recreate the models of many OSS 2.0 companies.

For example, Compound Labs built valuable open-source code (the Compound Protocol) that is used by many individuals and corporations. Compound acts as a new open-source infrastructure for lending. 

With the deep knowledge Compound Labs has about Compound Protocol (or as Matt Mullenweg calls it, "Founding Privilege") who is better suited than Compound Labs to build a scalable business on top of the Compound Protocol? 

This relationship should be similar to that of WordPress:

- Wordpress.org is a free open-source software and resource center 
- Wordpress.com is a managed WordPress hosting service that costs money to use

Now, the question crypto companies (note: companies, not protocols) have yet to answer is -- what should these businesses built atop protocols look like? 

## Open Source 3.0 Challenges

One core difference between prior models of OSS and crypto is that in crypto there are two capital structures, tokens and equity. 

For example, WordPress doesn't have a token that needs to accrue value. From a "returns" perspective, they only need to be concerned with accruing value to "Automattic" (the Labs co. behind WordPress and many other online properties). 

This is a legitimate challenge if the same team is responsible for the maximization of the company equity value and the token value. Inevitably, there will be a conflict. 

That said, if Labs entities wish to be protocol maintainers into perpetuity (something most token holders should want), they need to have sustainable business models. 

So what can they do?

## Open Source 3.0 Potential Models

OSS 0.0 was defined by free software, 
OSS 1.0 by support and service, 
OSS 2.0 by Cloud hosting and SAAS, 
OSS 3.0 will be defined by… 

My bet is that the companies that build impressive standalone businesses on top of crypto protocols will be focused on security, abstraction, and enablement. 

### Security
DeFi is risky. Adding a layer of security on top of protocols. 

The prevalence of hacks that happen throughout crypto is staggering and even though I have not seen this quantified, I have to presume it's a major deterrent for wider adoption. 

The Wormhole hack had the potential to be one of the single biggest losses for users in crypto until Jump backstopped the shortfall. While having Jump as a backstop is not scalable, charging users for protocol-specific insurance that core teams obtain from traditional insurers is a potential service. 

To an extent, the business that custodians or MPC providers are in has a lot of overlap here. For instance, Fireblocks users are required to whitelist individual smart contracts to engage with them.

### Abstraction

Even though they don't seem to be charging for it, Infinex, Kain from Synthetix's new project, is a good illustration of this principle. 

As Kain said:

> "One approach to solving [liquidity fragmentation] is to abstract away the network and act more like a centralized exchange; this is the experiment Infinex intends to run." 

Trading on Binance is easy. Trading on Synthetix is hard. A UI on top of the core protocol that makes it easier to trade on Synthetix is a net good for the protocol and SNX holders. 

It's something $SNX holders should be ecstatic about, even if the owners of this new front-end decide to charge a fee. 

Another example is Oku.trade built on top of Uniswap V3. Oku is a pro-interface that addresses the needs of pro-retail traders by offering advanced features typically found in traditional exchanges such as Binance or Coinbase, including order books, price charts, depth charts, trading history, user order history, and more.

The Oku UI has far more capabilities than the Uniswap.org UI and will potentially attract centralized exchange users with its richer feature set. Oku, Infinex, and other pro interfaces are logical for Labs or independent teams to build and charge users for usage.

### Enablement

In 2021, Compound Labs launched Compound Treasury, which was intended to be a bridge for non-crypto financial institutions to use protocols like Compound. While this product did not take off, the spirit of it was great and conceptually was the best attempt I've seen to build a business on top of a protocol that "grows the pie". 

For example, Current (a NeoBank app in the US) was going to give users access to Compound yields by integrating with Compound Treasury. This, on net, leads to more users, more deposits, and would be a huge win for the protocol. 

I can't imagine how any token holder could be mad if Compound Labs charged a fee for providing this service. 

## Uniswap's Position

One of my favorite podcast episodes of the last few months was this a16z podcast with Uniswap's COO, Mary-Catherine Lader. She was honest about how difficult it is to build a business at Uniswap Labs (or in crypto more broadly). 

To summarize some of her key quotes:

- Monetization without extensive user data collection is a challenge. No clear answer on what users will pay for.
- Uniswap prioritizes products that remove barriers to using the core protocol and acquire new users.
- They launched a wallet since wallets are a barrier to using Uniswap.
- They got into NFT trading as a user acquisition strategy, but missed the mark on solving an actual user need.
- Uniswap transitioned from an idea to a business in order to make the protocol easier to use and achieve wider adoption. Building the business is a critical component to fulfilling the initial idea.
- Uniswap struggles with finding product-market fit for products versus protocols. They are still learning how to deeply understand users and identify the right problems to solve.

I believe in Uniswap Labs' pitch that their mission is to lower barriers for users to access the core protocol. If they are successful at lowering those barriers, they should be able to charge for that. 

To the extent I have any pushback on Uniswap Labs turning on a front-end fee, it's that the UI they're implementing it on is already the default and is not net new or net additive to using the protocol. 

They are taking what is already the default way for many users to interact with the protocol and adding a fee. This can be viewed more as "rent-seeking" on existing user behavior and less as "growing the pie" by lowering new barriers. I think if they had implemented the fee only on wallet swaps (not the desktop front-end), they would have received far less pushback. 

That said, the beauty of crypto is that the core infrastructure is open and no one needs to use the Uniswap front-end. In the coming weeks and months, we will see how the market "votes" (with its transaction flow). You can follow along on Dune. 

The other place I see a lot of frustration is from users who are angry that Labs is turning on fees both (a) before the protocol and (b) higher than the proposed protocol fees. There is also a perception that Labs (who omit themselves from governance) and large investors are against turning on fees at the protocol level. Labs is likely NOT colluding with investors and the Foundation to hold off on protocol fees so that they could move first with their fees. To the extent critique should be levied for not yet turning on protocol fees, I think this falls more into the domain and mandate of the Uniswap Foundation than Uniswap Labs. 

## Closing

When Compound Labs launched Compound Treasury, I thought they described Compound Labs' role in the most elegant way possible:

> "The mission of Compound Labs, the company that built the protocol and handed it over to the community, is to build products and services that expand the Compound protocol's functionality and enable more users to access that functionality."

To me, that is the essence of what a good Labs company should be doing. Grow the overall protocol by increasing the addressable user base and taking a fee for that. Doing work that is aligned with the overall growth of the protocol. 

In contrast to what Compound had proposed with Compound Treasury, Uniswap throwing a fee on top of the already most-used UI is not "growing the pie". It's more extractive than additive. If, on the other hand, Uniswap had launched a "pro interface" (more like Oku.trade) that had features around providing V3 liquidity or setting complex trade types and tried to charge fees on that, I think the community would not view this as "extractive".

Existing web 2.0 open-source companies like GitLab or Automattic have done a great job of clarifying the role of their open-source contributions and drawing clear lines between what is and is not a free function. Uniswap Labs is beginning to define these boundaries within the Uniswap ecosystem, although it’s unclear whether these efforts will pay off.

One of the core challenges for entities that look to commercialize on top of protocols will be finding “minimally extractive” or “maximally additive” models that can justify fees on top of what might already exist within the protocol. If a protocol charges a native fee (something that does not exist in traditional OSS) and then a company charges a fee on top of that for their services, fees could quickly add up.

Companies looking to commercialize need to walk a fine balance of not losing the trust of their existing users who will (rightly) become upset if we revert back to the norms we thought we were breaking free of in the first place. 