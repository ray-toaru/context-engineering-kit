---
name: typescript-best-practices
description: Use when reading, writing, or reviewing TypeScript code and project-local TypeScript standards are needed.
---

# TypeScript Best Practices

Apply the TypeScript rule file at `../../rules/typescript-best-practices.md` when working on TypeScript code.

Focus on:

- strict and accurate types
- interfaces for object shapes and type aliases for unions or intersections
- type guards over unsafe assertions
- async APIs and `async`/`await`
- clear names, destructuring, and reusable library functions
- consistent time handling and non-silent error logging

Follow existing project conventions when they are explicit. If the rule conflicts with local architecture or tooling, explain the tradeoff and keep the change narrowly scoped.
