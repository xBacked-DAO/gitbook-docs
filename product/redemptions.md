---
description: Details about redemptions in the xBacked protocol
---

# Redemptions

## What are redemptions?

Redemptions are a mechanism within xBacked that **guarantees 1 xUSD can always be redeemed for $1 USD of underlying collateral**. This is different from repaying your debt. It is more like paying down system debt. This feature is only available 7 days after shutdown and is incentivized by allowing the user to purchase xUSD at a 1% discount

## How do redemptions work?

A user can redeem xUSD from any vault of their choice 7 days after shutdown, the protocol allows this at a 1% discount. During redemption, the protocol keeps 0.5% of discounted collateral and sends the remaining to the user.  The xUSD is used to repay the vaults debt and discounted collateral is sent to the user who performed the redemption. &#x20;

The owner of a vault incurs a net loss because the collateral is purchased at a discount although this will lead to a healthier collateral ratio for such vaults.

