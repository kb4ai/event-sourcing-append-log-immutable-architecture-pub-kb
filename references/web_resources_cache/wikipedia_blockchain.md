# Blockchain - Wikipedia

**Source:** https://en.wikipedia.org/wiki/Blockchain  
**Cached:** 2025-07-02

## Core Definition

Blockchain is a "distributed ledger with growing lists of records (blocks) that are securely linked together via cryptographic hashes"

## Block Structure

Each block contains:
1. **Cryptographic hash of previous block**
2. **Timestamp**
3. **Transaction data** (typically in a Merkle tree structure)

## Immutability and Append-Only Characteristics

- Transactions are "resistant to alteration because, once recorded, the data in any given block cannot be changed retroactively without altering all subsequent blocks"
- Blocks are "linked" in a chain, creating an append-only log where new blocks reference previous blocks

## Consensus Mechanisms

- Managed by peer-to-peer networks using consensus algorithms
- Validates and adds new transaction blocks
- Uses mechanisms like proof-of-work or proof-of-stake to ensure network agreement

## Key Architectural Layers

1. **Infrastructure** (hardware)
2. **Networking**
3. **Consensus**
4. **Data** (blocks/transactions)
5. **Application layer**

## Design Goals

The design ensures a "robust workflow where participants' uncertainty regarding data security is marginal" by creating a decentralized, transparent, and tamper-resistant record-keeping system.

## Relationship to Event Sourcing

- **Append-only log structure**: Similar to event streams
- **Immutability**: Events cannot be changed once recorded
- **Cryptographic integrity**: Events have verifiable hashes
- **Consensus**: Agreement on event ordering and validity
- **Audit trail**: Complete history of all changes