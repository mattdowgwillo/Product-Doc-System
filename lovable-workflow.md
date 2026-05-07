# Lovable Workflow

## Purpose

Define the correct workflow for using Lovable with structured product documentation.

Core principle:

Docs define the product.  
Lovable builds the product.  
GitHub stores the truth.

---

# Build Philosophy

Lovable should build:

- pages
- layouts
- UI structure
- visual hierarchy
- interaction polish

Lovable should NOT redefine:

- product logic
- component behavior
- flow behavior
- ownership boundaries
- MVP scope

---

# Primary Build Rule

Lovable builds from:

```text
page-*.md
```

Page docs are the primary build docs.

---

# Component Rule

Reusable behavior belongs in:

```text
component-*.md
```

Page docs should reference component docs instead of redefining behavior.

Example:

```md
Uses:
[component-chat-input.md](component-chat-input.md)
```

---

# Flow Rule

Flows define:

- transitions
- triggers
- outcomes

Flows should not define page layout or reusable component behavior.

---

# Recommended Workflow

## Step 1 — Define or Update Docs

Before building:

- create or update the correct docs
- clarify ownership
- resolve open questions

---

## Step 2 — Build One Page at a Time

Recommended prompt structure:

```text
Build page-user-dashboard.md.

Use:
- component-chat-input.md
- flow-user-onboarding.md

Do not add features outside MVP scope.
Do not redefine component behavior.
```

---

## Step 3 — Review Build

Check:

- does the UI match the page doc?
- does behavior match component docs?
- does flow behavior align with flow docs?

---

## Step 4 — Update Docs Only if Logic Changes

If:
- UI improves → no doc update needed
- behavior changes → update owning doc

---

# Build Priorities

1. Correct structure
2. Correct behavior
3. Real usability
4. Visual polish

---

# Anti-Patterns

Do NOT:

- build from giant brainstorm docs
- duplicate logic across files
- redefine components inside page docs
- let Lovable invent product logic
- overbuild MVP features too early

---

# Final Model

Define → Build → Test → Update docs → Repeat
