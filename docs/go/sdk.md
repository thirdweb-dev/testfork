---
slug: /sdk
title: ThirdwebSDK
hide_title: true
displayed_sidebar: go
---

## ThirdwebSDK

```go
type SDKOptions struct {
    PrivateKey string
    GatewayUrl string
}
```

## type [ThirdwebSDK](https://github.com/thirdweb-dev/go-sdk/blob/main/pkg/thirdweb/sdk.go#L11-L14)

```go
type ThirdwebSDK struct {
    *ProviderHandler
    Storage IpfsStorage
}
```

### func [NewThirdwebSDK](https://github.com/thirdweb-dev/go-sdk/blob/main/pkg/thirdweb/sdk.go#L23)

```go
func NewThirdwebSDK(rpcUrlOrChainName string, options *SDKOptions) (*ThirdwebSDK, error)
```

#### NewThirdwebSDK

Create a new instance of the Thirdweb SDK

rpcUrlOrName: the name of the chain to connection to \(e\.g\. "rinkeby"\, "mumbai"\, "polygon"\, "mainnet"\, "fantom"\, "avalanche"\) or the RPC URL to connect to

options: an SDKOptions instance to specify a private key and/or an IPFS gateway URL

### func \(\*ThirdwebSDK\) [GetEdition](https://github.com/thirdweb-dev/go-sdk/blob/main/pkg/thirdweb/sdk.go#L85)

```go
func (sdk *ThirdwebSDK) GetEdition(address string) (*Edition, error)
```

#### GetEdition

Get an Edition contract SDK instance

address: the address of the Edition contract

### func \(\*ThirdwebSDK\) [GetEditionDrop](https://github.com/thirdweb-dev/go-sdk/blob/main/pkg/thirdweb/sdk.go#L111)

```go
func (sdk *ThirdwebSDK) GetEditionDrop(address string) (*EditionDrop, error)
```

#### GetEditionDrop

Get an Edition Drop contract SDK instance

address: the address of the Edition Drop contract

### func \(\*ThirdwebSDK\) [GetNFTCollection](https://github.com/thirdweb-dev/go-sdk/blob/main/pkg/thirdweb/sdk.go#L72)

```go
func (sdk *ThirdwebSDK) GetNFTCollection(address string) (*NFTCollection, error)
```

#### GetNFTCollection

Get an NFT Collection contract SDK instance

address: the address of the NFT Collection contract

### func \(\*ThirdwebSDK\) [GetNFTDrop](https://github.com/thirdweb-dev/go-sdk/blob/main/pkg/thirdweb/sdk.go#L98)

```go
func (sdk *ThirdwebSDK) GetNFTDrop(address string) (*NFTDrop, error)
```

#### GetNFTDrop

Get an NFT Drop contract SDK instance

address: the address of the NFT Drop contract