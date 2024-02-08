---
description: Information about Liquidations of Vaults on xBacked
---

# Liquidations

Liquidations are allowed within the xbacked protocol when there is a vault that has its collateral ratio below the liquidation collateral ratio. Any actor simply pays a portion of the debt of such vault and collateral is received by that actor at a discount, there is a small fee attached to this, you can check out the various fees of the protocol [here](https://docs.xbacked.io/product/fees). The xBacked protocol will also allow users to stake xUSD into a pool used by the system for liquidating risky vaults.

## When do liquidations happen?

As soon as a vault collateral ratio drops below the liquidation collateral ratio, liquidation can begin. In this scenario, xUSD is used to repay the vault debt. The collateral is then transferred to the liquidator.

This happens until a vault collateral ratio is back to the minimum collateral ratio, you can find the minimum and liquidation collateral ratio of several vaults [here](https://docs.xbacked.io/contracts-and-tokens/mainnet)

## What fees are involved?

Liquidators receive discounted collateral. At the moment, this discount can be up to 3.5% of the spot rate, you can check out the discount rate for several vaults here.

The protocol takes a certain [fee](https://docs.xbacked.io/product/fees) from the liquidated collateral. This leaves the liquidator with <mark style="color:purple;">`discountRate`</mark>` ``-` [<mark style="color:purple;">`fee`</mark>](#user-content-fn-1)[^1]  percentage to profit

## Do Vaults get partially liquidated, or completely liquidated?

Partially liquidated. Vaults are only liquidated back to a healthy collateral ratio, the maximum collateral ratio a vault can be liquidated on is the minimum collateral ratio for that vault's collateral type.

## What is the incentive for me to stake my xUSD?

[Read about staking xUSD here.](staking-xusd.md)

[^1]: 
