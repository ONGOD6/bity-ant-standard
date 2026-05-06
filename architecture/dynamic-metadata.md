# Dynamic Metadata Layer — BITY ANT Standard

## Overview

The Dynamic Metadata Layer defines how Autonomous Node Tokens (ANTs) evolve over time without replacing, migrating, or reissuing the underlying NFT.

ANTs are persistent autonomous protocol entities whose metadata, state, augmentation profile, continuity score, lineage, and operational attributes may evolve continuously across Ethereum and Solana while preserving a stable token identity.

The NFT remains permanent.

The state evolves.

---

# Core Principles

## Persistent Identity

The ANT token identifier never changes.

Ethereum:
- ERC-721 tokenId remains constant

Solana:
- Mint address remains constant

Dynamic protocol state is layered onto the token instead of replacing the token itself.

---

## Autonomous Evolution

ANT metadata may evolve through:

- Augmentation
- CRS accumulation
- Node participation
- Protocol events
- Governance actions
- AI interactions
- Cross-chain synchronization
- Environmental triggers
- Real-world verified events
- Lineage inheritance
- RAP activation
  - Regeneration
  - Augmentation
  - Proliferation

---

## Metadata Separation

The architecture separates:

| Layer | Purpose |
|---|---|
| Static Metadata | Permanent NFT identity |
| Dynamic Metadata | Mutable protocol state |
| Visual Metadata | Render state and appearance |
| Intelligence Metadata | CRS, autonomy, memory |
| Lineage Metadata | Parent-child inheritance |
| Cross-Chain State | Ethereum/Solana synchronization |

---

# Ethereum Metadata Architecture

## Base Standards

Ethereum ANT implementations SHOULD combine:

- ERC-721
- ERC-4906
- ERC-8004
- Optional ERC-6551

---

# ERC-4906 Dynamic Metadata

ERC-4906 enables metadata update notifications.

ANT contracts SHOULD emit:

```solidity
event MetadataUpdate(uint256 _tokenId);
