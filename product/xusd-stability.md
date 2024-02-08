---
description: Planned Stability mechanisms for xUSD explained
---

# xUSD Stability: Coming Soon

## OverCollateralized Portfolio of Assets on the Balance Sheet

![Balance sheet comparison of Banks vs Crypto Protocols. xBacked is closest to MakerDAO. There is no negative equity in our protocol.](<../.gitbook/assets/image (10).png>)

xBacked is an over-collateralized protocol, designed closer to MakerDAO or Liquity. xUSD can only be minted when > $1 of underlying collateral is deposited. The collateral that backs xUSD is a portfolio of different assets; Algos, wrapped BTC & ETH, and later LP tokens from DEXEs. Each collateral type is limited to how much xUSD it can mint, which is the primary way xBacked can control the about of debt exposure to a certain collateral type.

![](<../.gitbook/assets/image (8).png>)

xUSD is backed by **exogenous collateral**, meaning the relationship is external to the protocol. This is the opposite of **endogenous collateral**, which describes the relationship between LUNA and UST

Importantly; in the bill proposed by Lummis in 2022, it is a requirement that stablecoins have ≥ 100% of collateral backing the tokens.

_Note: MakerDAO was used by TESLA in Apr 2022:_ [https://www.thismorningonchain.com/articles/defi/makerdao-is-diversifying-into-the-real-world-by-issuing-loans-to-tesla/](https://www.thismorningonchain.com/articles/defi/makerdao-is-diversifying-into-the-real-world-by-issuing-loans-to-tesla/)

## Supply fees

Each vault has a supply fee. This can be adjusted via governance to effect the demand on xUSD. For example, if it is too cheap there could be an oversupply in xUSD causing the peg to break to the down side.

## Liquidations

Vaults on xBacked can be liquidated by anyone, as long as the vaults collateral ratio is below the defined threshold. Depending on the type of collateral, collateral ratios will be lower of higher. For example, volatile illiquid assets would have higher collateral types while more liquid assets could have a lower collateral ratio.

Liquidators repay xUSD to a vault, in exchange for discounted collateral. This discount rate also differs per collateral type.

The protocol will take a 1% fee from all liquidations, and the stability pool stakers will receive a share of this for staking their xUSD.

![](<../.gitbook/assets/image (5).png>)

## Redemption

The redemption mechanism allows **1 xUSD token to be redeemed for $1 of underlying collateral  at a 1% discount 7 days after a vault is put in shutdown mode**. This means if the peg is trading below the $1 target, people are able to buy on a DEX and instantly profit on the arbitrage opportunity. This happening 7 days after a vault is put in shutdown mode also gives vault owners the option to close down their vaults to avoid being redeemed against and also avoids surprises [Read more about redemptions.](redemptions.md)

## xUSD Stability Pool

Users are able to stake their xUSD for liquidators to use in liquidations. Users receive discounted collateral, while liquidators do not need to provide capital upfront to liquidate bad vaults. Liquidators receive 0.5% of the liquidation (without risking their own capital). Think of this like a permissioned flash loan. Users are also able to use the stability pool as a hedge; they can define at what prices their staked xUSD will be used to liquidate collateral.

## Isolated Risk Vaults

Each vault is isolated from the other. This means if one asset price tanks, rugs, or otherwise fails to serve as decent collateral, it will only effect a small portion of xUSD in supply. There are "tier 1" assets like Algo, goBTC, goETH that are all strong collateral types. These vaults will have the highest debt ceilings, while other more risky vaults have lower caps.

## Use cases & Other mechanisms

As more use cases & stability mechanisms are developed, a list will be found here.

## Other resources

AlgoHQ Interview - ["When xBacked launches, what strategies are you thinking of to make sure from day 1, it stays at $1?"](https://www.youtube.com/watch?v=eM7TyelPA8c\&start=1577)

JT Invests in you Interview - ["What mechanisms do you have in place to help the stability of xUSD?"](https://www.youtube.com/watch?v=Cv1ktW2lk0I\&start=670)
