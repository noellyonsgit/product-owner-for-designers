# Product Owner for Designers

**Status: beta.** Tested on real work, still rough at the edges. Feedback very welcome.

AI means designers can now build almost anything. The hard part has moved upstream: should we build it, for whom, and how will we know it worked? That is product ownership, and most designers have never been taught it.

These two Claude skills help a designer build a real product plan for their own work, with a coach that explains every challenge as it goes.

## What's inside

### designer-po-coach
Share whatever you have (prototype, brief, requirements doc, design files, research) and it builds a product plan with you in five stages:

1. **Problem and outcome:** what changes, for whom, and how we'll measure it
2. **Evidence:** what we know, what we're assuming, and what's riskiest
3. **The bet:** the case for investing, and the points where we'd stop
4. **The slices:** turning your design into releasable increments
5. **The plan:** roadmap, metrics and who needs to sign off

It starts by showing you what your material already covers and what's missing. It drafts; you decide. Every challenge comes with a reason: who would push back, and what it would cost. It also asks how decisions get made where you work, so the plan fits your organisation rather than a generic template.

It can also diagnose your product owner strengths and gaps, review documents you've written, and rehearse difficult conversations with a sponsor or engineering lead.

### design-to-backlog
Turns a design into the thinnest slices that still deliver value. Writes user stories with acceptance criteria and edge cases taken from the design itself, flags gaps back to the designer rather than inventing answers, and prioritises in a way that shows the trade-offs.

The coach hands off to this skill at Stage 4, so they work best together.

## Install

### Claude Code
```
/plugin marketplace add noellyonsgit/product-owner-for-designers
/plugin install product-owner-for-designers@product-owner-for-designers
```

### Claude app (web, desktop, mobile)
1. Download the zips from the latest [release](../../releases), or from the `dist` folder.
2. In Claude, open your skills settings and upload each zip as a skill. Skills need code execution turned on.
3. Make sure both skills are switched on.

## Getting started
Start a conversation with something like:

> I'm a designer taking on product owner work for [project]. Here's the prototype and brief. Help me build a product plan.

The coach will introduce the five stages, read what you've shared and show you where to start.

## Feedback
This is a beta. If it misses something, challenges the wrong thing, or gets the tone wrong, please [open an issue](../../issues). Real examples help most.

## Author
Noel Lyons. 11 years leading design in FTSE 100 banks, with design teams of 125 to 300.

## Licence
MIT. See [LICENSE](LICENSE).
