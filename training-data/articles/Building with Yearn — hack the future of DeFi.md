
## Building with Yearn — hack the future of DeFi

## 📣Yearn Finance is calling on developers to build on top of our protocol!

![](https://cdn-images-1.medium.com/max/4630/1*vRsSgfHNlc4_Dxmg_FUeaA.png)

**Building on Yearn is easier than you think! I’ve met many a developer that have shied away from building on top of Yearn out of fear of it being far too complex or obtuse. Fear not fren! We have compiled a short guide to ease the way and included a list of ideas to inspire you!**

## This guide covers several topics:

* **What is Yearn? An overview of Yearn**

* **What can I build on top of Yearn?**

* **How the heck do I integrate with the Vaults?**

## What is Yearn and Why Even Build On It?

Yearn Finance is a suite of decentralized finance (DeFi) products that let users optimize their earnings on crypto assets through lending and trading services.

Yearn’s core product is the **Vault** (also known as yVault) — a set-it-and-forget-it yield aggregator running on top of DeFi’s yield-generating protocols like Compound, Aave, Curve, and Convex.

Vaults, in essence, are pools of funds with an associated yield strategy for maximizing returns on the asset in the vault. Vault strategies are more active than just lending out coins. Most strategies can do multiple things to maximize the returns, including supplying collateral and borrowing other assets such as stable coins, providing liquidity and collecting fees or farming other tokens and selling them for profit.

Because of the Vault’s open design, you can incorporate the generated yield as a design component of your project. Said differently, with Yearn, you can incorporate yield generation into your product, without having to build a a yield strategy from scratch.

## Prizes 💰

Yearn Finance is offering the following prizes:

🥇3 prizes totaling **$10,000.**

We are looking for innovative projects that either build on top of Yearn, support Yearn in some fashion, or represent an innovative idea.
> # Projects which exceed expectations will be offered bonus prizes through Yearn’s Grants Program.

**Yearn Grants. **We provide one-off grants or bounties to projects that have built interesting use-cases on top of Yearn. Reach out to people@yearn.finance.

## What to Build? Some Ideas..

DeFi is delivering tremendous value and utility to users through automation-driven, blockchain-based financial products and services that are defining a new crypto-economy. DeFi is slowly finding its way into every facet of the blockchain space. Whether you are building a P2E game, an NFT project, or DAO tooling, it is s likely that there is a DeFi functionality you can incorporate to build a better product.

Yearn Vaults are built with open standards and many projects have leveraged available vault integrations to build amazing applications on top of them.

**Common use-cases:**

* **Using Vaults as collateral for lending/borrowing**

* **Using Vaults to generate yield with user funds**

In both cases, the protocol integrating with yearn is rewarded with performance fees taken from the vault’s overall profits, the more total volume that a partner contributes to a vault, the bigger share of the profit they receive.

**Hundreds of protocols have built exciting functionalities using Yearn’s integration methods. These include:**

* **Alchemix** provides self-repaying loans using vault yields

* **Abracadabra** provided the first yVault leveraging system that allows users to take loans and keep the yield rolling

* **QiDao** provides 0% interest loans if you use yVaults as collateral

**Here are some ideas on what you can build:**

 1. Use the Vaults as collateral to borrow money and probably get some leverage. (e.g. Abracadabra)

2. Build a product that allows you to use yield to do cool stuff:

* donate yield to an NGO

* invest the yield in more risky stuff or directional bets

* paying bills and subscriptions

3. Create a metavault on top of multiple vaults. One idea that comes to my mind is having a USD metavault that deposits into multiple dollar pegged vaults based on some strategy and abstracts the complexity from the user.

4. Build a UI that accepts deposits and allows you to move assets across chains.

5. Use the vaults as a place to earn interest on funds that are not currently actively being used by the user.

**Previous Hackathon Projects**

* Bunker Finance: Bunker.finance is a decentralized protocol for NFT-backed loans. They integrated with Yearn v3’s USDC and WETH vaults and use them as a place to earn interest on funds that are currently not being supplied to borrowers.

* Skew You: Users can borrow against their options collateral, unlocking a whole new world of capital efficiency.

## Getting Started

**0. Background**

First things first, get your machine ready!

**You will need to download and install the following.**

* *git*

* [*eth-brownie](https://eth-brownie.readthedocs.io/en/stable/)*

* [*ganache](https://trufflesuite.com/ganache)*

* *Text editor (VS Code, Sublime Text, vim, others)*

To integrate with our vaults:

* [*BaseRouter](https://github.com/yearn/yearn-vaults/blob/main/contracts/BaseRouter.sol)*

* [*BaseWrapper](https://github.com/yearn/yearn-vaults/blob/main/contracts/BaseWrapper.sol)*

Read through our [docs](https://docs.yearn.finance/developers/v2/getting-started) to get your system ready to build on yearn.

## **Vaults in a Nutshell**

* *Written in Vyper 🐍*

* *They are an ERC20, so you can — Transfer, Swap, use them as collateral, and everything you do with other tokens.*

* *Keep track of your shares (amount, price per share)*

* *Immutable code managed by Yearn Governance*

* *A vault can run multiple strategies at the same time 😱*

* *Keep3rs integrated 🤖*

**Figure 1. You can interact with yVaults through depositing or withdrawing.**

![](https://cdn-images-1.medium.com/max/2996/0*VkIVKK6rkzIiR1Wy)

![](https://cdn-images-1.medium.com/max/2996/0*YHtlQGe0vigN9mmf)

## How to Integrate with the Vaults?

The most simple integration with Yearn is redirecting funds from a service into a yVaults in order to generate yield for your users on assets that otherwise wouldn’t generate yield. This opens up exciting new functionalities within your product or application.

We propose two methods of integration, wrappers and delegated deposits. Each have their distinct use-cases.

 1. Wrapper

2. Deposits

Figure 2. Wrapper Architecture

![](https://cdn-images-1.medium.com/max/2000/0*LFiqjAciF70LH6QR)

Learn more about the implications of both of these methods [here](https://docs.yearn.finance/partners/integration_guide).

## **Resource Bank:**

**DevDocs: [https://yearn.github.io/yearn-devdocs](https://yearn.github.io/yearn-devdocs)**

**yearn-vaults: [https://github.com/yearn/yearn-vaults](https://github.com/yearn/yearn-vaults)**

**BaseRouter: [https://github.com/yearn/yearn-vaults/blob/main/contracts/BaseRouter.sol](https://github.com/yearn/yearn-vaults/blob/main/contracts/BaseRouter.sol)**

**BaseWrapper: [https://github.com/yearn/yearn-vaults/blob/main/contracts/BaseWrapper.sol](https://github.com/yearn/yearn-vaults/blob/main/contracts/BaseWrapper.sol)**

**Wrapper-mix: [https://github.com/yearn/brownie-wrapper-mix](https://github.com/yearn/brownie-wrapper-mix)**

[**Article](https://medium.com/iearn/yearn-partners-building-with-yvaults-4cd042ea092): Yearn Partners– Building with yVaults**

[**Video: Into to Yearn Vaults](https://www.youtube.com/watch?v=a1TsO62402c)**

**Article: [Strategy Vetting and Endorsement](https://medium.com/iearn/how-new-yearn-vault-strategies-are-endorsed-8c0e0870790d)**

[**Video](https://www.youtube.com/watch?v=NVR3teJw0Y0): Become a mighty strategist!**

[**Tweet: Getting a Strategy to Prod](https://twitter.com/flashfish0x/status/1460246273488044036?s=20&t=kxak7a6qtrmDCfcn6UrGYA)**
