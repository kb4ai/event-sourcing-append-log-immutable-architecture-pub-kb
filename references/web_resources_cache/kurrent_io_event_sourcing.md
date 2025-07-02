# Event Sourcing - Kurrent.io

**Source:** https://www.kurrent.io/event-sourcing  
**Cached:** 2025-07-02

## Event Sourcing Overview

Event Sourcing is an architectural design pattern where changes in a domain are immutably stored as events in an append-only log.

### Core Definition

- Stores each change as a sequence of events
- Provides rich context about system state changes
- Allows reconstruction of system state by replaying events

### Key Benefits

1. **Comprehensive Audit Trail**
2. **"Time Travel" State Reconstruction**
3. **Root Cause Analysis**
4. **Fault Tolerance**
5. **Event-Driven Architecture Support**
6. **Asynchronous First Design**
7. **Service Autonomy**
8. **Replay and Reshape Capabilities**
9. **Enhanced Observability**
10. **Support for Occasionally Connected Systems**
11. **One-Way Data Flow**
12. **Legacy System Migration Assistance**

## Core Architectural Principles

### 1. Events
- Represent immutable business facts
- Described in past tense
- Contain unique metadata
- Capture business context

### 2. Event-Native Databases
- Append-only log as central storage
- Events stored chronologically
- Immutable event records

### 3. Streams
- Unique identifiers for domain objects
- Contain full history of changes
- Efficiently store large numbers of events

### 4. Projections
- Translate event data into read/write models
- Temporary and disposable
- Can generate new events or state representations

### 5. Subscriptions
- Enable publish/subscribe functionality
- Trigger notifications for events
- Support complex business workflows

## Related Architectural Patterns

- Domain-Driven Design
- CQRS (Command Query Responsibility Segregation)
- Event-Driven Architecture

## Implementation Considerations

- Focus on preserving business context
- Use smaller, concise aggregates
- Maintain a ubiquitous language between business and development

## Practical Example

An invoice processing system where each state change (issuing, payment, discount) is captured as a distinct event with full contextual information.

## Recommended For

Domains requiring:
- Complex state tracking
- Comprehensive audit capabilities
- Detailed historical analysis
- Flexible system evolution