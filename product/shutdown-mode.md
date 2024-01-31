# Shutdown Mode

Shutdown mode ensures that all xUSD can be returned for underlying collateral. When shutdown mode is triggered, vault owners cannot mint more xUSD.&#x20;

## Vault Owners

Vault owners have 48hrs after to return xUSD and close their vaults. After this, their vault may be redeemed against.

## xUSD Holders

7 days after shutdown mode, any xUSD holder can redeem xUSD  1$ of underlying colateral **at a 1% discount on the collateral price**. The protocol deducts 0.5% of the discounted collateral\
\
Liquidations would also still be available within the 7 days that leads up to the redemption feature being unlocked

When all vaults are closed, and there is no more outstanding xUSD, the vault contract will cease to function.
