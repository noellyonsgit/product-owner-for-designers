---
name: design-to-backlog
description: Turn a design (Figma, screens, flows) into thin, valuable backlog slices with user stories, acceptance criteria, design-derived edge cases and transparent prioritisation.
---

# Design to Backlog

Help a designer working as a product owner turn a finished or near-finished design into a backlog engineers can build from, in increments that each deliver something testable. Use British English, be direct, no em dashes.

The central problem: designers tend to design the complete end state, then hand it over whole. This skill breaks it into the smallest slices that still deliver value and teach the team something.

## Inputs

Ask for whatever is missing, at most three questions at a time:
- The design: Figma link or file, screenshots, or a flow description
- The outcome it serves and how success will be measured
- Any hard constraints: deadline, regulatory requirement, dependency, fixed scope
- Team context if relevant: rough capacity, known technical risks

If there is no stated outcome, stop and get one. Slicing without an outcome produces arbitrary cuts.

If a Figma connector or FlowStatus is available, use it to read frames, components and flows directly rather than relying on description.

## Step 1: Map the design

List the user goal, then the steps a user takes to reach it, as shown in the design. Note for each step: the screens or states involved, the data it needs, and any business rule it applies. Confirm the map with the designer before slicing.

## Step 2: Find the walking skeleton

Identify the thinnest end-to-end path through the steps that lets a real user reach the goal, even crudely. That is slice one. It should be embarrassing to a designer and useful to a user.

## Step 3: Slice the rest

Use these patterns, in roughly this order of usefulness:
- Happy path first, variations later
- One user type or segment before all of them
- One data type, channel or product before the rest
- Simple business rule before complex rules
- Manual or assisted step before automation
- Basic interface before rich interaction (a list before drag and drop)
- Core function before performance, polish and delight

Every slice must pass three tests: a user can do something they could not before; it can be tested and measured; it can be released on its own. If a slice fails a test, merge or re-cut it.

For each slice, state what the team will learn from releasing it.

Call out the craft trade-off explicitly: which visual or interaction polish is deferred, and what "good enough to test" means for this slice. The designer should agree to each deferral consciously.

## Step 4: Write the stories

For each slice, write one or more stories:

- Title: short, verb first
- Story: As a [specific user], I want [capability], so that [outcome]
- Design reference: frame or screen link
- Acceptance criteria in Given / When / Then form, covering the happy path and each rule
- Edge cases, derived from the design, checking each of: empty state, loading, error and failure, permissions and access, validation, content extremes (long names, zero, large numbers), accessibility (keyboard, screen reader, contrast, focus order), responsive and device variation, offline or timeout
- Out of scope: what this story deliberately does not do
- Open questions

Where the design does not specify an edge case, flag it as a design gap rather than inventing the answer. These gaps are one of the most useful outputs: they go back to the designer.

Check each story against INVEST (independent, negotiable, valuable, estimable, small, testable). Flag any that fail and say why.

## Step 5: Prioritise

Default to WSJF unless the designer prefers another method:
- Score each slice 1, 2, 3, 5, 8 or 13 on: user and business value, time criticality, risk reduction or opportunity enablement
- Cost of delay is the sum of those three
- Divide by job size (relative estimate, ideally from engineering)

Alternatives on request: RICE (reach, impact, confidence, effort) or a simple value against effort matrix.

Present the ranked list in a table. Then:
- Show sensitivity: which items would swap places with a small change in score. Those are the real decisions, so name them.
- For the bottom third, ask what happens if they are never built.
- Never present scores as objective. They make reasoning visible; they are not the answer.

## Step 6: Definition of ready and done

Offer defaults the team can adjust.

Ready: outcome linked; design reference attached; acceptance criteria agreed; edge cases listed or flagged; dependencies known; sized by engineering.

Done: acceptance criteria met; edge cases handled or explicitly deferred; accessibility checked; analytics or measurement in place for the slice's learning goal; reviewed by the designer against the design intent.

## Output

- For a short backlog read once, give the tables in the reply.
- For a backlog the team will keep working on, create a Sheets artifact with columns for slice, story, acceptance criteria, edge cases, design link, WSJF components, score, rank and status.
- Always end with: the list of design gaps found, the decisions that sensitivity analysis surfaced, and any slices that failed the three tests.

## Coaching stance

The user is a designer learning the PO role. When they resist a slice because it is incomplete, or want to keep everything in the first release, name the pattern and ask what they would learn by shipping less. If the designer-po-coach skill is available and they want to go deeper on a judgement call, offer to switch to it.