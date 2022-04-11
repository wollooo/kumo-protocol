<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@liquity/lib-ethers](./lib-ethers.md) &gt; [SendableEthersLiquity](./lib-ethers.sendableethersliquity.md) &gt; [depositKUSDInStabilityPool](./lib-ethers.sendableethersliquity.depositkusdinstabilitypool.md)

## SendableEthersLiquity.depositKUSDInStabilityPool() method

Make a new Stability Deposit, or top up existing one.

<b>Signature:</b>

```typescript
depositKUSDInStabilityPool(amount: Decimalish, frontendTag?: string, overrides?: EthersTransactionOverrides): Promise<SentEthersLiquityTransaction<StabilityDepositChangeDetails>>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  amount | [Decimalish](./lib-base.decimalish.md) | Amount of KUSD to add to new or existing deposit. |
|  frontendTag | string | Address that should receive a share of this deposit's KUMO rewards. |
|  overrides | [EthersTransactionOverrides](./lib-ethers.etherstransactionoverrides.md) |  |

<b>Returns:</b>

Promise&lt;[SentEthersLiquityTransaction](./lib-ethers.sentethersliquitytransaction.md)<!-- -->&lt;[StabilityDepositChangeDetails](./lib-base.stabilitydepositchangedetails.md)<!-- -->&gt;&gt;

## Remarks

The `frontendTag` parameter is only effective when making a new deposit.

As a side-effect, the transaction will also pay out an existing Stability Deposit's [collateral gain](./lib-base.stabilitydeposit.collateralgain.md) and [KUMO reward](./lib-base.stabilitydeposit.kumoreward.md)<!-- -->.
