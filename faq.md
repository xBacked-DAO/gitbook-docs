---
description: Quick answers to FAQs on the xBacked protocol
---

# FAQ

## What are the fees?

Supply fees vary per vault. Algo/xUSD might have an annual fee of 3.5% while BTC/xUSD might have 5%.

These supply fees **are fixed, and will not change.** To change supply fees, vaults must be deprecated & redeployed with a new fee rate. Read more about deprecation.

## What collateral can I use?

xBacked is multi-collateral. Currently, we are planning to have Algo, goBTC, goETH and gAlgo, which all have strong liquidity. In the further future the team and community will assess other options.

## How are new collateral types integrated?

The following factors are considered when selecting new collateral types for xBacked

* On Chain liquidity; will liquidations cause a cascading crash if there's too much debt for this new collateral type? Will liquidators be able to sell liquidated collateral at a favorable price? [2022, Solend highlighted this risk](https://decrypt.co/103489/solend-whale-108m-loan-nearly-crashed-solana).
* Bridge risk; if the asset is bridged, what is the risk of accepting it? How much of this asset should be backing xUSD? [This risk is highlighted in the 2022 hack of Wormhole](https://twitter.com/dmihal/status/1488982240830930960?s=20\&t=Chjj\_7FEshVFaum6xXO7rw).
* Community demand; will our users actually find this introduction valuable?
* Price feeds; can we get or create reliable price feeds for this asset?

## Will I still receive ALGO Rewards?

No, you will not receive Algo rewards. These will accrue in the vault, and when the vault eventually closes the DAO will receive any accrued rewards. In this event, the DAO will create a community proposal for how the funds should be used.

## Can I participate in Algorand Governance via xBacked?

xBacked does not natively allow users to stake Algos for governance. Instead, we plan to integrate with Liquid Staking assets like gAlgo from Folks Finance. We are focused on being the **best stablecoin, not liquid staking.** Leveraging composability, we can still allow users to participate in governance & xBacked.

## What are the fees for xBacked?

[Documentation on our fee structure is here.](product/fees.md)

| Action       | Fee                   |
| ------------ | --------------------- |
| Minting xUSD | 0%, annual supply fee |
| Liquidations | 1%                    |
| Redemptions  | 0.5-2%                |

## What is the minimum collateral ratio?

This varies per vault, but could be as low as 110% depending on the collateral type. [Read more about vaults here.](product/vaults.md)

## What is the minimum amount of collateral required to open a vault?

$100 USD, but could vary per vault and change over time.

## Is xBacked a DAO?

Yes, we are working towards a fully decentralized governance model.

* [Join the community](community-links.md)
* [Read about participating in governance](governance/participating-in-governance.md)

## Does xBacked have a bug bounty program?

Absolutely, [please follow the documentation](documentation/bug-bounty-program.md) to participate in our bug bounty program.
