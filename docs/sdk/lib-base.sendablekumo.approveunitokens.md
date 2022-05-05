<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@kumodao/lib-base](./lib-base.md) &gt; [SendableKumo](./lib-base.sendablekumo.md) &gt; [approveUniTokens](./lib-base.sendablekumo.approveunitokens.md)

## SendableKumo.approveUniTokens() method

Allow the liquidity mining contract to use Uniswap ETH/KUSD LP tokens for [staking](./lib-base.transactablekumo.stakeunitokens.md)<!-- -->.

<b>Signature:</b>

```typescript
approveUniTokens(allowance?: Decimalish): Promise<SentKumoTransaction<S, KumoReceipt<R, void>>>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  allowance | [Decimalish](./lib-base.decimalish.md) | Maximum amount of LP tokens that will be transferrable to liquidity mining (<code>2^256 - 1</code> by default). |

<b>Returns:</b>

Promise&lt;[SentKumoTransaction](./lib-base.sentkumotransaction.md)<!-- -->&lt;S, [KumoReceipt](./lib-base.kumoreceipt.md)<!-- -->&lt;R, void&gt;&gt;&gt;

## Remarks

Must be performed before calling [stakeUniTokens()](./lib-base.transactablekumo.stakeunitokens.md)<!-- -->.
