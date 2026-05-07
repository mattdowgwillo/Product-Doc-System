Home Hero – Product System
Home Hero helps buyers decide which home to buy.

Search tells you what a home has.
Touring tells you how a home lives.

Core Principle
Docs define the product.
Lovable builds the product.
GitHub stores the truth.

If it is not in /docs, it does not exist.

How to Use This Repo
This file is your entry point.

When updating the product:

Identify what you are changing
Use the sections below to find the correct doc
Click → edit → build
Do NOT:

edit multiple docs for the same logic
define behavior outside docs
Product Overview
system-summary.md
→ Core product definition, problem, MVP, strategy
System (Foundation)
These define how the product works at a system level.

system-architecture.md
→ Structure of product (pages, components, flows)

system-context-states.md
→ How context (open house, agent, independent) affects behavior

system-email.md
→ Email triggers, role, and return-to-product behavior

Pages (UI Surfaces)
Use these when changing what users see or interact with on a screen

page-property-details.md
→ Core experience during and after a tour

page-buyer-dashboard.md
→ Buyer workspace for managing homes and decisions

page-agent-dashboard.md
→ Agent surface for leads, follow-up, and insights

Components (Reusable Systems)
Use these when changing interaction logic or input behavior

component-tour-composer.md
→ Prompt bar + input system (notes, guided input, ratings)
Flows (User Movement)
Use these when changing when and how things happen

flow-check-in.md
→ Entry into the product (QR, open house, etc.)

flow-tour-capture.md
→ Behavior during active tour

flow-post-tour.md
→ Reflection after leaving

flow-decision-comparison.md
→ Comparing homes + decision making

AI Build Support
lovable-workspace-rules.md
→ Global AI behavior rules (copied into Lovable workspace)

lovable-manifest-prompt.md
→ Task-specific doc loading

testing-guide.md
→ Validation framework

How to Make Changes (Workflow)
Step 1 — Identify the change
Start with a real issue:

“Users aren’t taking notes”
“Comparison feels generic”
“Drop-off after check-in”
Step 2 — Map to system
Determine:

Page → UI or layout
Component → behavior or interaction
Flow → timing or transitions
Step 3 — Update ONE doc
Only update the doc that owns the logic
Link to other docs if needed
Do NOT duplicate behavior
Step 4 — Validate coverage
Before building:

Does this affect multiple pages?
Does this change a component?
Does this introduce new states?
Does this impact a flow?
If yes: → update those docs first

Step 5 — Build in Lovable
Example:

Build using page-property-details.md
Use component-tour-composer.md

Step 6 — Evaluate
Does it match the doc?
Does it work in real use?
Step 7 — Update docs if needed
Behavior changed → update doc
UI polish → ignore
Product Evolution (Post-MVP)
Always start with behavior:

User Behavior → Product Intent → System Impact → Doc Update → Build → Learn
