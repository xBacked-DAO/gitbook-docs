---
description: Information about minting xUSD on xBacked
---

# Minting xUSD

To mint xUSD, you must open a vault on the xBacked protocol. Below are details on how Vaults work on xBacked.

## What is a Vault?

Vaults are created by a user of the xBacked protocol when they deposit collateral (e.g ALGO) and mint xUSD. A user can only have 1 vault per wallet address they hvae.

## What can I do with a Vault?

After a vault is created, you are able to deposit more collateral and mint more xUSD as long as your vault has a healthy collateral ratio.

If you repay the vault debt, the vault is closed and any collateral still in the vault is transferred back to you.

## What is a Collateral Ratio?

xBacked is an over collaterized stablecoin. This means that there must **always be more collateral in the system than debt**. This is a common DeFi primitive call a Collaterized Debt Position (CDP). Collateral Ratios are calculated using the following formula:

$$
Collateralization\space Ratio\space (CR)={\sum Value\space of\space Collateral\over\sum Value\space of\space Debt}
$$

## **What are the minimum collateral ratios for Vaults?**

Vaults have a **minimum collateral ratio which varies per vault.** Below this level, vaults become available for liquidation.

To withdraw collateral, or to mint new debt, the collateral ratio **must be above a certain collateral ratio**.

{% hint style="info" %}
Note: the frontend by default enforces a margin of saftey when updating a vault. If you would like to push the limits of a vault, it is possible via the SDK or by using DEGEN Mode
{% endhint %}

## What is the minimum collateral deposit required to open a Vault?

There will be a minimum mint amount to open a vault on xBacked, which is `100 xUSD`. This is subject to change via governance proposals. The reasoning is that a bad actor could spam vaults and fill xBacked with junk vaults quite cheaply. This would slow down liquidators monitoring legitimate vaults, and decrease overall health of the protocol.

## Is there a maximum vault collateral size?

Yes, vaults will have a maximum dollar value for the collateral allowed. This is to help mitigate the risk of a vault being too large to liquidate with on chain liquidity.

## What collateral types does xBacked support?

xBacked is multi-collateral and supports a diverse range of collateral types. View the current range of collateral options and their vault parameters [here](https://docs.xbacked.io/contracts-and-tokens/mainnet)

## Do Vaults have an interest rate?

Yes, xBacked vaults have a fixed interest rate, which can differ per collateral type. There is no minting fee, or closing fee charged. Originally there was only a minting fee charged; however the team decided an ongoing fee would be helpful to maintain the xUSD peg, incombination with redemptions. [Read more about that here](redemptions.md).

## Is there a time limit on repaying minted xUSD?

No, there is no repayment schedule for xUSD. When a user mints xUSD there is **no expectation they repay it** to the protocol. The only expectation is that eventually the vault will close, either via liquidation or by the owner returning vault debt.

## What happens if my Vault is liquidated?

If your vault collateral ratio drops below the minium (e.g`110%`) then it is liquidated. In this case, your vault will be liquidated back to `120%` and you will be left with the remaining vault collateral & xUSD.

In this process, liquidators repay your vaults debt.

## What happens if my Vault is redeemed against?

In the event of a redemption against your vault, it would have been the riskiest vault in the system at the time. Even if your collateral ratio is healthy (e.g `125%`) a redemption will still happen.

In this case, a part or all of your collateral can be redeemed. You will keep the xUSD minted, but your collateral will be reduced partially, or completely (and your debt will be reduced partially or completely too).
