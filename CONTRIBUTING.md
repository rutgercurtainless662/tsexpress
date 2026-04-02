# Contributing to tsexpress

## Why Contribute

`tsexpress` is a greenfield framework project. That means early contributions can materially shape the API, the repository standards, and the engineering culture around the project.

If you want to make an impact on a framework while it is still defining itself, this is a good place to do it. Strong early work will be visible because the project is starting from zero.

## Human and AI Contributions

Human contributions are welcome.

AI-assisted contributions are also welcome.

This repository is intentionally being set up so agents can understand the project context and execute well-scoped work. Issues labeled `agent-task` are expected to be workable by coding agents. Issues labeled `good first issue` should be especially approachable for both humans and agents.

## What Good Contributions Look Like

Good contributions usually have these properties:

- they keep the framework feeling like Express
- they improve or protect the TypeScript experience
- they stay close to Node's `http` model
- they are small enough to review clearly
- they include tests when framework behavior changes
- they avoid unnecessary magic or abstraction

## Before You Start

- Read [README.md](./README.md), [docs/vision.md](./docs/vision.md), and [docs/principles.md](./docs/principles.md).
- Prefer starting from an existing issue.
- If you want to work on something substantial that does not have an issue yet, open one first so the direction can be discussed.

## Working on an Issue

- Stay within the issue's scope unless discussion changes that scope.
- If you find a better approach, explain the tradeoff before widening the change.
- Keep changes understandable. A smaller sharp contribution is better than a broad unclear one.
- If a change alters framework behavior, add or update tests with it.

## Quality Bar

The project is aiming for a high bar from the start.

- The runtime should stay small.
- The API should feel like Express on first contact.
- TypeScript should be part of the design, not an afterthought.
- Route contracts should be treated as first-class.
- Types should match runtime behavior as closely as possible.
- Tests are expected for meaningful behavior changes.

Changes that make the framework feel heavier, stranger, or less like Express should be challenged, even if they look technically clever.

## Communication

Be direct. Explain tradeoffs. Raise uncertainty early.

This project should welcome serious disagreement about design when that disagreement improves clarity. The goal is not to merge anything that compiles. The goal is to build a framework with a coherent identity.
