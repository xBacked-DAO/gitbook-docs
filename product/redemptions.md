---
description: Details about redemptions in the xBacked protocol
---

# Redemptions

## What are redemptions?

Redemptions are a mechanism witin xBacked that **guarantee 1 xUSD can always be redeemed for $1 USD of underlying collateral**. This is different to repaying your own debt. It is more like paying down system debt in the event the value of XUSD drops below $1 USD

## How do redemptions work?

When a user redeems xUSD on xBacked, the redemption is made against **the riskiest vault in the system** even if that vault's collateral ratio is over the minimum of `110%`. The xUSD is then used to repay some of that vaults debt, and the collateral transferred from the vault to the redeemer.

The owner of a vault will not incur a net loss, but exposure to their collateral will be reduced.

There is a 2% fee taken from **the redeemed** collateral. For example, if you redeem 100 xUSD for $100 worth of Algo, 2% will be taken by the protocol as a fee.

## Proposing Vaults for Redemption

Vaults are not sorted on chain. Instead, the protocol relies on a network of Keepers monitoring for riskier vaults than those in the current list. When one of these keepers finds a riskier vault, and successfully propose it, they receive 0.075% of that vaults collateral as a reward.
