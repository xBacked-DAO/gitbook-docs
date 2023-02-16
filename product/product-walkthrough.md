---
description: Images & instructions for how to use xBacked
---

# Product Walkthrough

{% embed url="https://www.youtube.com/watch?v=ZV3EMIZ8GFc" %}
Video Walkthrough - dated the 7th of February 2022
{% endembed %}

## Connecting a Wallet

Please [refer to this guide](connecting-wallets.md) on connecting a wallet for xBacked.

Make sure you have Algos in testnet: [https://bank.testnet.algorand.network/](https://bank.testnet.algorand.network)

## Creating a Vault

When you initially open xBacked, you will be presented with this screen

![](../.gitbook/assets/image.png)

Click on the "Create Vault" button, and you will be presented with a screen that allows you to enter how much collateral you will deposit & how much xUSD to mint.

![](<../.gitbook/assets/image (3).png>)

In the next step you will be asked to confirm the vault details before initiating vault creation.

![](<../.gitbook/assets/image (9).png>)

Note: on your first time using xBacked you will be prompted with three transactions; one to opt-into the xUSD token, one to opt-into the Vault application, and the third will be to deposit collateral and mint xUSD.

## Using a Vault

When you have created a vault, the main screen will update.

![](<../.gitbook/assets/image (12).png>)

Clicking on "View Vault" will show you all the actions you can do with your vault.

![](<../.gitbook/assets/image (11).png>)

Each these actions will either improve the health of your vault, or make it worse.

![](<../.gitbook/assets/CleanShot 2022-07-07 at 11.05.02.gif>)

![](<../.gitbook/assets/CleanShot 2022-07-07 at 11.05.40.gif>)

## Closing a Vault

To close a vault, simply return all xUSD + accrued supply fees. After this, the remaining collateral in the vault will be transferred back to you.

![](<../.gitbook/assets/image (4).png>)



## Liquidating a Vault

In reality, it is highly likely that a bot will liquidate a vault before you will. However, below is a guide to using the UI

![](<../.gitbook/assets/image (1).png>)

Once you fetch vaults, you will be presented with a list of vaults that can be liquidated. Clicking on "Liquidate" will take you to a page where you can repay xUSD & receive discounted collateral for improving the health of the vault

![](<../.gitbook/assets/CleanShot 2022-07-07 at 12.34.48.gif>)

## Redemptions

When xUSD is trading below the $1 target, it becomes profitable to buy it on a DEX and redeem it for $1 of underlying collateral. Choose which collateral to redeem. There is a small fee involved in redemption, taken from the redeemed collateral

![](<../.gitbook/assets/CleanShot 2022-07-07 at 12.41.52.gif>)
