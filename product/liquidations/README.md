---
description: Information about Liquidations of Vaults on xBacked
---

# Liquidations

The xBacked protocol allows users to stake xUSD into a pool used by the system for liquidating risky vaults.

## When do liquidations happen?

As soon as a vault collateral ratio drops below `110%` liquidation can begin. In this scenario, xUSD is used to repay the vault debt. The collateral is then transferred to the liquidator.

This happens until a vault collateral ratio is back to `120%`

## What fees are involved?

Liquidators receive discounted collateral. At the moment, this discount is 3.5% to the spot rate.

The protocol takes a 1% fee from the liquidated collateral. This leave the liquidator with a 2.5% discount to spot

## Do Vaults get partially liquidated, or completely liquidated?

Partially liquidated. Vaults are only liquidated back to a healthy collateral ratio of `120%`.

## What is the incentive for me to stake my xUSD?

[Read about staking xUSD here.](staking-xusd.md)
