# tsexpress

TypeScript-first web framework design inspired by Express.

## Why This Exists

Express got something important right: web servers should be easy to read, easy to compose, and close to Node's native HTTP model. `tsexpress` exists to keep that feel while taking TypeScript seriously from the beginning.

This project is not trying to build a giant meta-framework. The goal is a small, understandable framework that feels like Express, but treats types and contracts as first-class parts of the design.

## Project Vision

`tsexpress` should feel familiar to anyone who has used Express:

- app and router based composition
- `req`, `res`, and `next`
- middleware chains and error middleware
- simple route registration on top of Node `http`

The difference is that `tsexpress` should champion TypeScript-first development:

- route contracts are part of route declarations
- TypeScript should infer as much as possible from those contracts
- runtime behavior and type behavior should stay aligned

Agent-friendly introspection matters, but it is downstream of the framework itself. First it must be a strong web framework. Then it can expose metadata that makes applications and deployments easier for agents to inspect.

## Design Principles

- Feel like Express from the first read.
- Stay close to Node's `http` runtime model.
- Keep abstractions small and obvious.
- Treat contracts and types as part of the framework, not optional garnish.
- Require tests for meaningful behavior changes.
- Build agent-friendly introspection without warping the API around it.

## Why Contribute Early

This project is starting from zero. Early contributors have a real chance to shape the framework, influence its conventions, and leave visible fingerprints on its foundation.

That applies to both human contributors and AI-assisted contributors. Strong early work will be easy to attribute because the project is still defining its defaults, style, and architecture.

## Initial Focus

The first wave of work is about building a serious foundation:

- clear project docs and contribution guidance
- repository scaffolding for a small TypeScript library
- framework primitives like app creation, routers, middleware, and response helpers
- contract-driven typing
- internal introspection for future agent-friendly tooling

## Contributing

See [CONTRIBUTING.md](./CONTRIBUTING.md) for contribution standards and workflow expectations.
