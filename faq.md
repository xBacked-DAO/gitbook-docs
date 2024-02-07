---
description: Quick answers to FAQs on the xBacked protocol
---

# FAQ

## What are the fees?

Supply fees can vary per vault. Presently, all vaults have an annual fee of 3%

These supply fees **are fixed, and will not change.** To change supply fees, vaults must be deprecated & redeployed with a new fee rate. Read more about deprecation.

## What collateral can I use?

xBacked is multi-collateral. Currently, a range of assets are available including ALGO, goBTC, goETH, GOLD$ and more. See a full list including vault parameters for each [here](https://docs.xbacked.io/contracts-and-tokens/mainnet). In the further future, the team and community will assess other options.

## How are new collateral types integrated?

The following factors are considered when selecting new collateral types for xBacked

* On Chain liquidity; will liquidations cause a cascading crash if there's too much debt for this new collateral type? Will liquidators be able to sell liquidated collateral at a favorable price? [2022, Solend highlighted this risk](https://decrypt.co/103489/solend-whale-108m-loan-nearly-crashed-solana).
* Bridge risk; if the asset is bridged, what is the risk of accepting it? How much of this asset should be backing xUSD? [This risk is highlighted in the 2022 hack of Wormhole](https://twitter.com/dmihal/status/1488982240830930960?s=20\&t=Chjj\_7FEshVFaum6xXO7rw).
* Community demand; will our users actually find this introduction valuable?
* Price feeds; can we get or create reliable price feeds for this asset?



## Can I participate in Algorand Governance via xBacked?

xBacked does not natively allow users to stake Algos for governance. Instead, we have integrated Liquid Staking assets like gAlgo from [Folks Finance](https://folks.finance/) and mAlgo from [Messina](https://messina.one/). We are focused on being the **best stablecoin, not liquid staking.** Leveraging composability, we can still allow users to participate in governance & xBacked.

## What are the fees for xBacked?

[Documentation on our fee structure is here.](product/fees.md)

| Action       | Fee                   |
| ------------ | --------------------- |
| Minting xUSD | 0%, annual supply fee |
| Liquidations | 1%                    |
| Redemptions  | 0.5%                  |

## What is the minimum collateral ratio?

This varies per vault but could be as low as 110% depending on the collateral type.[ Check out individual Min Cr values for each vault here](https://docs.xbacked.io/contracts-and-tokens/mainnet)

## What is the minimum amount of xUsd required to open a vault?

$100 xUsd, but could vary per vault and change over time.

## Is xBacked a DAO?

Yes, we are working towards a fully decentralized governance model.

* [Join the community](community-links.md)
* [Read about participating in governance](governance/participating-in-governance.md)

