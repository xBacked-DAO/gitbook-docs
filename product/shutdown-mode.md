# Shutdown Mode

Shutdown mode ensures that all xUSD can be returned for underlying collateral. When shutdown mode is triggered, the oracle price is frozen, and vault owners cannot mint more xUSD.&#x20;

## Vault Owners

Vault owners have 48hrs after to return xUSD and close their vaults. After this, their vault may be redeemed against.

## xUSD Holders

48hrs after shutdown mode any xUSD holder can redeem xUSD for $1 of underlying colateral **at the frozen collateral price** from 48hrs ago. There are no fees in this process.

When all vaults are closed, and there is no more otustanding xUSD, the vault contract will cease to function.
