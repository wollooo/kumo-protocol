<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@kumodao/lib-ethers](./lib-ethers.md) &gt; [SendableEthersKumo](./lib-ethers.sendableetherskumo.md) &gt; [repayKUSD](./lib-ethers.sendableetherskumo.repaykusd.md)

## SendableEthersKumo.repayKUSD() method

Adjust existing Trove by repaying some of its debt.

<b>Signature:</b>

```typescript
repayKUSD(amount: Decimalish, overrides?: EthersTransactionOverrides): Promise<SentEthersKumoTransaction<TroveAdjustmentDetails>>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  amount | [Decimalish](./lib-base.decimalish.md) | The amount of KUSD to repay. |
|  overrides | [EthersTransactionOverrides](./lib-ethers.etherstransactionoverrides.md) |  |

<b>Returns:</b>

Promise&lt;[SentEthersKumoTransaction](./lib-ethers.sentetherskumotransaction.md)<!-- -->&lt;[TroveAdjustmentDetails](./lib-base.troveadjustmentdetails.md)<!-- -->&gt;&gt;

## Remarks

Equivalent to:

```typescript
adjustTrove({ repayKUSD: amount })

```
