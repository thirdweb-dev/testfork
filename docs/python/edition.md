---
slug: /edition
title: Edition Objects
hide_title: true
---
<a id="contracts.edition"></a>

# contracts.edition

Interface for interacting with an edition contract

<a id="contracts.edition.Edition"></a>

## Edition Objects

```python
class Edition(ERC1155)
```

<a id="contracts.edition.Edition.mint"></a>

#### mint

```python
def mint(
    metadata_with_supply: EditionMetadataInput
) -> TxResultWithId[EditionMetadata]
```

Mint a new NFT to the connected wallet

**Arguments**:

- `metadata_with_supply`: EditionMetadataInput for the NFT to mint

**Returns**:

receipt, id, and metadata of the mint

<a id="contracts.edition.Edition.mint_to"></a>

#### mint\_to

```python
def mint_to(
    to: str, metadata_with_supply: EditionMetadataInput
) -> TxResultWithId[EditionMetadata]
```

Mint a new NFT to the specified wallet

**Arguments**:

- `to`: wallet address to mint the NFT to
- `metadata_with_supply`: EditionMetadataInput for the NFT to mint

**Returns**:

receipt, id, and metadata of the mint

<a id="contracts.edition.Edition.mint_additional_supply"></a>

#### mint\_additional\_supply

```python
def mint_additional_supply(
        token_id: int,
        additional_supply: int) -> TxResultWithId[EditionMetadata]
```

Mint additional supply of a token to the connected wallet

**Arguments**:

- `token_id`: token ID to mint additional supply of
- `additional_supply`: additional supply to mint

**Returns**:

receipt, id, and metadata of the mint

<a id="contracts.edition.Edition.mint_additional_supply_to"></a>

#### mint\_additional\_supply\_to

```python
def mint_additional_supply_to(
        to: str, token_id: int,
        additional_supply: int) -> TxResultWithId[EditionMetadata]
```

Mint additional supply of a token to the specified wallet

**Arguments**:

- `to`: wallet address to mint additional supply to
- `token_id`: token ID to mint additional supply of
- `additional_supply`: additional supply to mint

**Returns**:

receipt, id, and metadata of the mint

<a id="contracts.edition.Edition.mint_batch"></a>

#### mint\_batch

```python
def mint_batch(
    metadatas_with_supply: List[EditionMetadataInput]
) -> List[TxResultWithId[EditionMetadata]]
```

Mint a batch of NFTs to the connected wallet

**Arguments**:

- `metadatas_with_supply`: list of EditionMetadataInput for the NFTs to mint

**Returns**:

receipts, ids, and metadatas of the mint

<a id="contracts.edition.Edition.mint_batch_to"></a>

#### mint\_batch\_to

```python
def mint_batch_to(
    to: str, metadatas_with_supply: List[EditionMetadataInput]
) -> List[TxResultWithId[EditionMetadata]]
```

Mint a batch of NFTs to the specified wallet

**Arguments**:

- `to`: wallet address to mint the NFTs to
- `metadatas_with_supply`: list of EditionMetadataInput for the NFTs to mint

**Returns**:

receipts, ids, and metadatas of the mint