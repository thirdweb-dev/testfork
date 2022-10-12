---
slug: /solana/react.balancequery
title: balanceQuery() function
hide_title: true
displayed_sidebar: react
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## balanceQuery() function

**Signature:**

```typescript
export declare function balanceQuery(wallet: RequiredParam<UserWallet>): {
  queryKey: readonly [
    "__tw__",
    "sol",
    RequiredParam<import("@thirdweb-dev/sdk/solana").Network>,
    "wallet-balance",
    {
      readonly address: string | undefined;
    },
  ];
  queryFn: () => Promise<{
    value: string;
    displayValue: string;
  }>;
  enabled: boolean;
};
```

## Parameters

| Parameter | Type                            | Description |
| --------- | ------------------------------- | ----------- |
| wallet    | RequiredParam&lt;UserWallet&gt; |             |

**Returns:**

{ queryKey: readonly \["\_\_tw\_\_", "sol", RequiredParam&lt;import("@thirdweb-dev/sdk/solana").Network&gt;, "wallet-balance", { readonly address: string \| undefined; }\]; queryFn: () =&gt; Promise&lt;{ value: string; displayValue: string; }&gt;; enabled: boolean; }