---
name: angular-frontend
description: "Implement and review Angular frontend features, components, templates, forms, routing, accessibility, performance, and tests. Use when editing an Angular application or diagnosing Angular UI behavior."
---

# Angular Frontend Skill

Use this workflow for Angular application implementation, debugging, and
frontend review.

## Workflow

1. Inspect `package.json`, the Angular configuration, nearby source files, and
   relevant tests before choosing APIs. Follow the installed Angular version
   and existing project conventions; do not assume the latest Angular release.
2. Trace the affected UI flow and identify its data, state, routing, and
   loading/error behavior before editing.
3. Make the smallest complete change. Reuse existing components and services,
   preserve established boundaries, and avoid adding dependencies or
   restructuring unrelated code.
4. Keep templates readable and state explicit. Use the project's existing
   patterns for standalone or NgModule-based code, signals or RxJS, and
   template control flow. Do not mix patterns or migrate architecture without
   a requirement.
5. For forms, preserve validation and submission behavior, use the project's
   existing forms approach, and provide clear accessible labels and error
   feedback.
6. Check semantic HTML, keyboard operation, focus behavior, accessible names,
   and responsive layouts for UI changes. Avoid unnecessary ARIA where native
   elements already provide the semantics.
7. Add or update focused tests for changed behavior. Prefer the test framework
   and test style already present in the project.
8. Run the narrowest relevant test, lint, or build command available. Report
   what changed and the checks run, including any checks that could not be run.

## Review priorities

When reviewing, focus on demonstrable issues such as incorrect rendering or
state transitions, subscription/resource leaks, broken form or navigation
behavior, inaccessible interactions, and missing coverage for changed logic.
Explain the user impact and point to the relevant code. Do not report
speculative or purely stylistic preferences as defects.
