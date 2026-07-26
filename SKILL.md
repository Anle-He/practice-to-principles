---
name: practice-to-principles
description: Distills scoped, evidence-backed principles from meaningful real-world use, manages candidate/active/retired lifecycle, and routes confirmed principles into the workflows where they must load before action. Use after a framework materially affects a decision, action, or review and outcome evidence exists, or when Anle asks to retain, generalize, promote, activate, route, revise, audit, or retire a learned rule.
---

# Practice to Principles

Turn applied knowledge into reusable principles without confusing source claims with validated experience.

## Protocol

1. Before distilling or changing principle state, read `references/active.md` and `references/candidates.md`; update an overlapping entry instead of creating a duplicate.
2. Treat one completed decision, action, or review as one application episode. Run at most one distillation pass per episode.
3. Stop without writing when the episode only retrieved information, produced no new learning, or lacks meaningful evidence.
4. Record novel learning in `references/candidates.md` using its schema. Preserve source, scope, evidence, exceptions, counterevidence, and proposed activation targets.
5. Never increase confidence merely because a source is persuasive. Merge practical support and contradiction explicitly.
6. Promote a candidate only after repeated practical support, Anle's explicit confirmation, and a verified activation route as described below.
7. Move disproved or superseded principles to `references/retired.md`; never erase their history, and account for every installed activation route.
8. Briefly report any recorded, promoted, routed, revised, or retired principle.

## Promotion and activation

`references/active.md` is the canonical registry, not an automatic global context source. A principle is active only when it is both registered and routed into at least one workflow that naturally loads it before the relevant behavior occurs.

1. Draft the active entry and an activation plan. Choose the narrowest natural target, such as the nearest applicable `AGENTS.md` or an operational skill that already triggers for the scoped work.
2. Ask Anle to confirm the principle and authorize each external activation target. Promotion confirmation alone is not blanket permission to edit proposed targets.
3. Install a concise execution hook at every authorized target. Include the principle ID and enough operational wording to act without reconstructing the evidence history; keep full evidence only in `active.md`.
4. Verify that each target is naturally loaded before the trigger described by the principle. A file that is merely stored or only loaded by this distillation skill is not an activation route.
5. Only after registration, route installation, and verification, move the entry to `active.md` with `Activation status: routed`.
6. If Anle confirms the principle but no route is authorized or available, keep it in `candidates.md` as `confirmed-unrouted`. Do not call it active.
7. When revising or retiring an active principle, identify its installed routes and obtain authorization before updating or removing external hooks. Record route cleanup in `retired.md`.

## Boundaries

- Modify only this skill's files unless Anle explicitly authorizes each external activation target.
- Never rewrite system instructions, project rules, `AGENTS.md`, `ANLE.md`, or external memory automatically.
- Keep every principle narrow enough to state when it applies and when it does not.
