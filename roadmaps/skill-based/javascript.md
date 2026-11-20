---
title: JavaScript Roadmap
---

# JavaScript

Learn the language of the web by building browser applications you can run yourself.

[← Skill based roadmaps](README.md) | [All roadmaps](../README.md)

## Start here

- [ ] Write and run a small script with variables, functions, and conditionals
- [ ] Manipulate the page with the DOM
- [ ] Fetch data from an API and show the result
- [ ] Keep the project in Git

## Learning stages

### 1. Language fundamentals

- Variables, functions, scope, and control flow
- Strings, numbers, booleans, arrays, and objects
- Equality, coercion, and common edge cases
- Modules and imports
- Errors: throwing, catching, and reading stack traces

**Build:** a command-line quiz that reads questions, tracks a score, and reports invalid answers.

### 2. Collections and functional patterns

- Array methods such as `map`, `filter`, and `reduce`
- Object and array destructuring
- Reference behavior and immutable updates
- Closures and higher-order functions
- Iteration with `for...of`

**Build:** a small data report that groups and summarizes a JSON dataset.

### 3. The browser and the DOM

- Selecting and updating nodes
- Events, delegation, and form handling
- Semantic markup and keyboard interaction
- The web storage APIs
- Developer tools for inspecting and debugging state

**Build:** a notes page that stores entries in the browser and supports editing and deleting.

### 4. Asynchronous JavaScript

- Callbacks and promises
- `async` and `await`
- Fetch, HTTP errors, and timeouts
- Concurrent requests and cancellation with `AbortController`
- Loading, empty, success, and error states

**Build:** a search interface that requests data while typing, cancels stale requests, and shows clear status.

### 5. Testing and maintainability

- Pure functions and separating logic from DOM code
- Unit tests with a test runner such as Vitest or Jest
- Browser tests for user-visible behavior
- Formatting and linting
- Observability for client errors

**Build:** add tests for the previous project’s filtering and error handling, including one browser-level test of a critical flow.

## Definition of done

You can build a browser application from scratch, handle asynchronous data safely, test critical behavior, and explain the language features you used.

## Related roadmaps

- [Frontend developer](../role-based/frontend-developer.md)
- [Frontend beginner](../beginners/frontend-beginner.md)
- [Git and GitHub](git-and-github.md)

## FAQ

### Should I learn TypeScript now?

Learn enough JavaScript to understand the runtime first, then add TypeScript for larger projects. Types catch mistakes, but they do not replace knowledge of browser behavior.

[↑ Catalog](README.md) | [← Category index](README.md)
