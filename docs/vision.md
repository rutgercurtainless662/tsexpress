# Vision

## What tsexpress Is

`tsexpress` is a TypeScript-first web framework inspired by Express.

It should feel familiar to developers who know Express, while taking TypeScript, route contracts, and long-term maintainability more seriously from the beginning.

The target experience is simple and readable:

- app and router primitives
- middleware chains
- familiar request and response semantics
- direct relationship to Node's `http` server model

## What tsexpress Is Not

`tsexpress` is not trying to be:

- a generic AI framework
- a batteries-first meta-framework
- a reinvention of the Node HTTP mental model
- a heavy TypeScript abstraction that stops feeling like Express

## TypeScript-First Development

TypeScript should shape the framework, not merely annotate it.

In `tsexpress`, route contracts are expected to be first-class. Once a route contract is declared, the framework should infer useful types for handlers, middleware, and response behavior with as little friction as possible.

The goal is not to force ceremony. The goal is to make the framework structurally aware of the application in a way that improves correctness and clarity.

## Feels Like Express

This is a hard design constraint.

A Node developer should be able to read `tsexpress` code and immediately recognize the control flow:

- `app`, `router`, `req`, `res`, `next`
- middleware in sequence
- mounted routers
- route handlers that still look like route handlers

If the framework drifts so far into TypeScript cleverness that it no longer feels like Express, the design has failed.

## Agent-Friendly, Not Agent-Warped

Agent-friendly introspection matters, but it is secondary to the framework itself.

`tsexpress` should maintain enough internal metadata to support inspection, tooling, and deployment-friendly visibility. That should happen without forcing application authors into an unnatural API or a special agent-only programming model.

The right order is:

1. build a small, coherent web framework
2. make its structure intelligible to tools and agents

Not the other way around.
