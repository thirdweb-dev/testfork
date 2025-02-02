---
slug: /sdk.editiondrop._constructor_
title: EditionDrop.(constructor)
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## EditionDrop.(constructor)

Constructs a new instance of the `EditionDrop` class

**Signature:**

```typescript
constructor(network: NetworkOrSignerOrProvider, address: string, storage: ThirdwebStorage, options: {
        readonlySettings?: {
            chainId?: number | undefined;
            rpcUrl: string;
        } | undefined;
        gasSettings?: {
            maxPriceInGwei?: number | undefined;
            speed?: "standard" | "fast" | "fastest" | undefined;
        } | undefined;
        gasless?: {
            experimentalChainlessSupport?: boolean | undefined;
            openzeppelin: {
                relayerForwarderAddress?: string | undefined;
                useEOAForwarder?: boolean | undefined;
                relayerUrl: string;
            };
        } | {
            biconomy: {
                deadlineSeconds?: number | undefined;
                apiId: string;
                apiKey: string;
            };
        } | undefined;
    } | undefined, abi: Abi, chainId: number, contractWrapper?: ContractWrapper<PrebuiltEditionDrop>);
```

## Parameters

| Parameter       | Type                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | Description       |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------- |
| network         | [NetworkOrSignerOrProvider](./sdk.networkorsignerorprovider.md)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |                   |
| address         | string                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |                   |
| storage         | ThirdwebStorage                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |                   |
| options         | { readonlySettings?: { chainId?: number &#124; undefined; rpcUrl: string; } &#124; undefined; gasSettings?: { maxPriceInGwei?: number &#124; undefined; speed?: "standard" &#124; "fast" &#124; "fastest" &#124; undefined; } &#124; undefined; gasless?: { experimentalChainlessSupport?: boolean &#124; undefined; openzeppelin: { relayerForwarderAddress?: string &#124; undefined; useEOAForwarder?: boolean &#124; undefined; relayerUrl: string; }; } &#124; { biconomy: { deadlineSeconds?: number &#124; undefined; apiId: string; apiKey: string; }; } &#124; undefined; } &#124; undefined |                   |
| abi             | [Abi](./sdk.abi.md)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |                   |
| chainId         | number                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |                   |
| contractWrapper | ContractWrapper&lt;PrebuiltEditionDrop&gt;                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | <i>(Optional)</i> |
