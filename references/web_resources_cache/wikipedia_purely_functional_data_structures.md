# Purely Functional Data Structures - Wikipedia

**Source:** https://en.wikipedia.org/wiki/Purely_functional_data_structure  
**Cached:** 2025-07-02

## Core Definition

"Purely functional data structures are data structure[s] that can be directly implemented in a purely functional language"

## Key Characteristics

- **Fundamentally immutable** data structures that cannot be modified after creation
- Implemented using only persistent data structures like tuples, sum types, and product types
- Avoid destructive updates, which permanently alter data
- Maintain previous versions of data structures unmodified

## Advantages

1. **Full persistency**
2. **Quick object copying**
3. **Thread safety**

## Design Techniques

### 1. Lazy Evaluation
- Computation performed only when result is required
- Allows efficient handling of potentially unused data

### 2. Memoization
- Saves computed results to prevent redundant calculations
- Particularly useful in lazy implementations

### 3. Amortized Analysis and Scheduling
- Distribute computational costs across operations
- Ensure predictable performance by spreading inefficient operations

## Example Implementations

- **Stack** (singly-linked list)
- **Queue** (real-time queue)
- **Double-ended queue**
- **Red-black trees** for sets and maps
- **Priority queues**
- **Random access lists**

## Practical Considerations

- Requires explicit state management
- May need to return multiple values from functions
- Can use modules or classes to enforce immutability in impure languages

## Relationship to Event Sourcing

- **Immutability principle**: Events are never modified once created
- **Structural sharing**: Efficient storage of event histories
- **Persistence**: Previous states remain accessible
- **Thread safety**: Concurrent access to event logs
- **Predictable performance**: Amortized costs for event processing

## Philosophy

The approach fundamentally transforms how data structures are conceived, prioritizing immutability and predictability over direct mutation.