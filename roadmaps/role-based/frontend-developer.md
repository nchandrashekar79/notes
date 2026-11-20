---
title: Frontend Developer Roadmap
---

# Frontend Developer

Build accessible, responsive user interfaces and the browser-side logic behind them.

[← Role based roadmaps](README.md) | [All roadmaps](../README.md)

## What a frontend developer does

A frontend developer turns a product idea and a design into an interface people can use. That includes page structure, visual layout, interaction, accessibility, performance, testing, and collaboration with designers and backend engineers.

## Start here

- [ ] Build a page with semantic HTML and no framework
- [ ] Style it with CSS and make it usable on a phone
- [ ] Add interaction with JavaScript
- [ ] Publish the page and share its URL

## Learning stages

### 1. The web platform

Learn how browsers request, parse, and display a page.

- Semantic HTML: headings, landmarks, forms, images, and native controls
- CSS: the box model, selectors, cascade, specificity, layout, and responsive design
- JavaScript in the browser: the DOM, events, modules, and the Fetch API
- Browser developer tools: inspect elements, check the accessibility tree, debug JavaScript, and measure network requests
- HTTP basics: requests, responses, status codes, headers, and caching

**Build:** a multi-section responsive profile page that works without JavaScript and can be navigated with a keyboard.

### 2. Language and interface fundamentals

- Modern JavaScript: scope, closures, objects, arrays, promises, and async/await
- TypeScript: types, narrowing, generics, and working with third-party types
- Accessibility: labels, focus order, keyboard behavior, contrast, and reduced-motion preferences
- Forms: validation, helpful errors, and safe submission
- Responsive images, fonts, and layout for a range of viewport sizes

**Build:** an accessible form that validates input and displays errors next to the relevant field.

### 3. Application development

Choose one component-based framework after you can build interactively without one.

- Component composition and state management
- Routing and URL state
- Data fetching, loading states, empty states, and errors
- Rendering strategy: client-side, server-side, or static
- Build tools and environment configuration
- API contracts and authentication flows

**Build:** a small application that reads from a public API and supports search, filtering, and a useful loading state.

### 4. Quality and production

- Unit tests for pure logic and component tests for user behavior
- End-to-end tests for the most important user journeys
- Web performance: bundle size, image optimization, and Core Web Vitals
- Security basics: untrusted content, cross-site scripting, and secret handling
- Continuous integration and deployment
- Observability: client errors, performance signals, and release verification

**Build:** add tests and automated deployment to the previous project, then measure it on a slow mobile connection.

### 5. Working as a professional

- Break work into small, reviewable changes
- Write clear pull requests and review feedback
- Estimate effort and communicate risks early
- Use feature flags and progressive rollout where appropriate
- Explain trade-offs between performance, complexity, and maintainability

**Build:** keep a short record of one technical decision, the alternatives considered, and the result.

## Definition of done

You can build a responsive, accessible application from an empty folder, connect it to an API, test its critical flows, deploy it, and explain your choices to another developer.

## Related roadmaps

- [Frontend beginner](../beginners/frontend-beginner.md)
- [JavaScript](../skill-based/javascript.md)
- [Git and GitHub](../skill-based/git-and-github.md)
- [Portfolio project](../projects/portfolio-project.md)

## FAQ

### Do I need a framework?

Not at first. One framework is more valuable once you understand the browser platform and can debug the problems the framework abstracts.

### How much design skill is needed?

Enough to produce a clear, usable layout. You should understand spacing, hierarchy, typography, color contrast, and responsive layout, even when a designer provides the visual direction.

[↑ Catalog](README.md) | [← Category index](README.md)
