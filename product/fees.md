---
description: Information on fees charged by using the xBacked protocol
---

# Fees

## Opening & Closing a vault

No fees.

## Interest rate

Varies per collateral type. Initially, the Algo/xUSD vault will be set to 2%. This rate can only change by **launching a new vault**. This means old vaults will have a static rate applied, which cannot change.

## Liquidations

A liquidator will receive a discount when liquidating a vault. For example, it might be 3.5%.

The protocol will charge a 1% fee on this collateral, so the liquidator effectively gets a 2.5% discount.

If the liquidator uses staked xUSD, the staker will receive a 2% discount, the liquidator will receive 0.5% of the liquidated collateral, and the protocol takes 1% fee.

## Redemption

When redeeming, a fee is applied to the collateral. For example, if you redeem 100 xUSD for $101 ALGO, at a 1% you will receive $100.5 worth of ALGO.

## Fee Distribution

These are the beginning metrics - and can be modified later via governance.

**Algo Fees (Liquidation & Redemptions)**

These fees accrue in the contract over time. Anyone can trigger fee distribution, and when they do they receive 0.5% of the accrued fees. These Algo fees go to the following

* 0% to xUSD stakers in the liquidation contract (initially this will be 0%, the parameter can be modified)&#x20;
* 100% to the DAO treasury address

**xUSD Fees (generated via interest)**

Over time, interest accrues in the contract in the form of xUSD. Anyone can trigger the settlment of these fees. Upon settlement, the caller receives no reward. However, the fees are distributed in the following way

* 100% to the DAO treasury address
* 0% to the governance token stakers (the parameter can be modified)

The incentive here is for those staking governance tokens to trigger fee distribution for xUSD fees.
