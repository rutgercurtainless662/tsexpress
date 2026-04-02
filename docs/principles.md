# Principles

## Keep The Runtime Small

The runtime should stay compact and understandable. New abstractions need to justify themselves with real clarity or capability, not with novelty.

Contributions violate this principle when they add indirection, configuration layers, or framework machinery that do not clearly improve the developer experience.

## Stay Close To Node

`tsexpress` should live close to Node's `http` model. The framework should not hide the runtime so aggressively that developers lose their intuition about what the server is doing.

Contributions violate this principle when they replace straightforward Node semantics with a separate internal world that is harder to reason about than the platform itself.

## Feel Like Express

The project should preserve the shape and texture that make Express readable: familiar naming, obvious control flow, simple middleware chaining, and direct route registration.

Contributions violate this principle when they make common tasks feel unlike Express for the sake of clever typing or framework personality.

## Types Are Part Of The Design

TypeScript is not an optional finishing layer. It is part of the framework's design surface from the start.

Contributions violate this principle when they add runtime behavior without a coherent type story, or when they accept weak, misleading, or inconsistent typings around core APIs.

## Contracts Are First-Class

Routes should have explicit contracts, and the framework should derive as much useful information from those contracts as possible.

Contributions violate this principle when they treat contracts as optional decoration rather than as a foundation for handler typing, validation, and future introspection.

## Tests Prove Behavior

If a contribution changes framework behavior, it should usually come with tests that prove the behavior directly. Tests are part of the quality bar, not a cleanup task for later.

Contributions violate this principle when they change core behavior without evidence, or when tests only confirm implementation details instead of user-visible framework behavior.

## Introspection Should Not Distort The API

The framework should support introspection and agent-friendly tooling, but those capabilities should remain in service of the core developer experience.

Contributions violate this principle when they push the public API toward agent-specific ceremony, metadata clutter, or patterns that weaken the Express-like feel of ordinary application code.
