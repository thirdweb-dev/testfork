---
slug: /react.useownednfts
title: useOwnedNFTs() function
hide_title: true
displayed_sidebar: react
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## useOwnedNFTs() function

> This feature is currently in beta and may change based on feedback that we receive.

Use this to get a the owned NFTs for a specific [NFTContract](./react.nftcontract.md) and wallet address.

## Example 1

```javascript
const nftDrop = useNFTDrop(<ContractAddress>);
const { data: ownedNFTs, isLoading, error } = useOwnedNFTs(nftDrop, <OwnerWalletAddress>);
```

## Example 2

```javascript
const { contract } = useContract(<ContractAddress>);
const { data: ownedNFTs, isLoading, error } = useOwnedNFTs(contract?.nft, <OwnerWalletAddress>);
```

**Signature:**

```typescript
export declare function useOwnedNFTs<TContract extends NFTContract>(
  contract: RequiredParam<TContract>,
  ownerWalletAddress: RequiredParam<WalletAddress>,
): import("@tanstack/react-query").UseQueryResult<NFT<TContract>[], unknown>;
```

## Parameters

| Parameter          | Type                                                                                       | Description                                            |
| ------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------ |
| contract           | [RequiredParam](./react.requiredparam.md)&lt;TContract&gt;                                 | an instance of a [NFTContract](./react.nftcontract.md) |
| ownerWalletAddress | [RequiredParam](./react.requiredparam.md)&lt;[WalletAddress](./react.walletaddress.md)&gt; | the wallet adress to get owned tokens for              |

**Returns:**

import("@tanstack/react-query").UseQueryResult&lt;[NFT](./react.nft.md)&lt;TContract&gt;\[\], unknown&gt;

a response object that includes the list of owned tokens