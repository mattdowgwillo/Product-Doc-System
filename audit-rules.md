# Audit Rules

## Purpose

Define how product documentation should be audited for consistency, clarity, and Lovable readiness.

---

# Audit Priorities

## 1. Ownership Clarity

Every doc must clearly define:

```md
## This doc owns:
## This doc does NOT own:
```

Flag:
- unclear ownership
- duplicated ownership
- missing ownership blocks

---

## 2. Duplicate Logic

Logic should only exist in one place.

Flag:
- repeated component behavior
- repeated flow definitions
- duplicated page logic

Recommend linking instead.

---

## 3. Correct Doc Types

Check whether content belongs in:

- system
- page
- component
- flow

Flag:
- component behavior inside page docs
- page layout inside flow docs
- flow logic inside component docs

---

## 4. Lovable Readiness

Page docs should be build-ready.

Check:
- clear layout
- clear states
- linked components
- MVP clarity

Flag:
- abstract product thinking
- unclear page behavior
- ambiguous ownership

---

## 5. MVP Discipline

Flag:
- overbuilt systems
- future complexity in MVP
- unnecessary abstraction
- premature personalization

---

## 6. Missing Relationships

All related docs should link to each other where appropriate.

Flag:
- missing links
- isolated docs
- unclear dependencies

---

# Audit Output Format

Use:

```text
KEEP
FIX
MERGE / DELETE
MISSING
NEXT ACTION
```

---

# Final Principle

Documentation should reduce ambiguity, not create it.
