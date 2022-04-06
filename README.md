---
description: >-
  xBacked is a Distributed Autonomous Organization (DAO) building decentralized
  stable assets for Algorand
---

# About

xBacked is a DAO building a decentralised, permissionless stablecoin on Algorand, over collateralized by ASAs like Algo, goBTC, and goETH.

## How does it work? <a href="#docs-internal-guid-6f74a61e-7fff-7f17-cdec-6e0307f1c772" id="docs-internal-guid-6f74a61e-7fff-7f17-cdec-6e0307f1c772"></a>

xBacked ensures all xUSD in circulation is over collateralized via vaults. These vaults are collateralized debt positions (CDPs), and work similarly to MakerDAO, Liquity, and over collateralized stablecoins.

A core focus of the protocol is capital efficiency. Extremely low liquidation threshold of a 110% collateral ratio. Users can, technically, mint all the way up to this point if they really wanted to. Algorand is fast; we leverage that because we can guarantee that liquidations/debt being returned to vaults will never be held up&#x20;

xBacked also leverages isolated risk markets in the architecture. Different vault types (e.g Algo/xUSD and gotBTC/xUSD) have different health factors, they are not combined. It means if one vault is affected by massive volatility, it will not affect other positions taken on xBacked and only affect a subset of xUSD in circulation.

Check out this blog post for more information about the protocol: [https://medium.com/algopulse/xbacked-a-decentralized-stablecoin-for-algorand-69f3f296efd2](https://medium.com/algopulse/xbacked-a-decentralized-stablecoin-for-algorand-69f3f296efd2)

{% file src=".gitbook/assets/xBacked_Litepaper - Mar 2022.pdf" %}
