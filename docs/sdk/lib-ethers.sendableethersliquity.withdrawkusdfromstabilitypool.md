<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@liquity/lib-ethers](./lib-ethers.md) &gt; [SendableEthersLiquity](./lib-ethers.sendableethersliquity.md) &gt; [withdrawKUSDFromStabilityPool](./lib-ethers.sendableethersliquity.withdrawkusdfromstabilitypool.md)

## SendableEthersLiquity.withdrawKUSDFromStabilityPool() method

Withdraw KUSD from Stability Deposit.

<b>Signature:</b>

```typescript
withdrawKUSDFromStabilityPool(amount: Decimalish, overrides?: EthersTransactionOverrides): Promise<SentEthersLiquityTransaction<StabilityDepositChangeDetails>>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  amount | [Decimalish](./lib-base.decimalish.md) | Amount of KUSD to withdraw. |
|  overrides | [EthersTransactionOverrides](./lib-ethers.etherstransactionoverrides.md) |  |

<b>Returns:</b>

Promise&lt;[SentEthersLiquityTransaction](./lib-ethers.sentethersliquitytransaction.md)<!-- -->&lt;[StabilityDepositChangeDetails](./lib-base.stabilitydepositchangedetails.md)<!-- -->&gt;&gt;

## Remarks

As a side-effect, the transaction will also pay out the Stability Deposit's [collateral gain](./lib-base.stabilitydeposit.collateralgain.md) and [KUMO reward](./lib-base.stabilitydeposit.kumoreward.md)<!-- -->.
