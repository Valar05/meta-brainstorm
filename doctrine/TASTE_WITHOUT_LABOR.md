# Taste Without Labor

**Date:** 2026-09-14
**Status:** active doctrine / user preference clarification

## Observation

After sustained game-development work, Drew no longer treats manual production labor as inherently valuable. In this domain, labor has often cost more joy than it produced.

The ideal outcome is therefore not "keep some craft work for authenticity." It is:

```text
minimal or zero required production labor
+ output that reliably matches Drew's taste
+ retained ability to inspect, reject, redirect, and own the result
```

The human contribution may collapse toward taste, judgment, selection, and veto rather than implementation.

## Consequence

A Good House should not preserve friction merely because a previous generation associated labor with authorship.

The relevant question is not:

> How much work did the human personally perform?

It is:

> Did the system produce something the human actually wants, while preserving the human's authority over what counts as acceptable?

This permits a very small creative loop:

```text
WANT -> RECEIVE -> JUDGE -> KEEP / REJECT / REDIRECT -> ENJOY
```

If the result already satisfies taste, further labor is optional.

## Taste is not a fixed profile

The brainstorm corpus itself is evidence that Drew's taste is highly time-varying. It moves across vehicle combat, survivorlike pressure loops, text-choice systems, embodied FPS movement, procedural animation, historical tactics, creative tooling, and other very different forms without requiring one stable genre identity.

Therefore a system should not model taste as one permanent vector such as:

```text
TASTE = fixed_user_profile
```

A better representation is:

```text
T_t = current taste state at time t
B   = slower-changing boundaries, values, and judgment habits
```

The objective is to estimate `T_t` without mistaking it for identity.

This suggests a **taste-weather** model rather than a taste-profile model:

- infer strongly from immediate context and recent choices;
- retain broad, slower-changing constraints without forcing them into genre preferences;
- keep multiple distinct possibilities alive rather than converging on one recommendation basin;
- allow a tiny choice, rejection, or redirect to update the current state quickly;
- preserve surprise and exploration so successful prediction does not become narrowing;
- never treat yesterday's delight as an obligation today.

The stable signal may live less in *what* Drew wants and more in *how he judges*: whether something has causal coherence, useful consequence, sufficient distinctness, real play value, and freedom from unnecessary extraction or friction. Those are hypotheses to test, not a license to freeze Drew into a permanent profile.

## Important boundary

Taste matching is not passive personalization if the person cannot inspect or contest it. A system that predicts taste but quietly captures attention, narrows options, or optimizes for another party has recreated the Bad House.

The target is **taste sovereignty**, not merely recommendation accuracy.

A taste-sovereign system must therefore preserve the right to become different tomorrow.

## Compact doctrine

> **Labor is not the proof of authorship, and friction is not the proof of craft.**

> **For Drew's ideal game, the remaining human job may be nothing more burdensome than: does this delight me?**

> **Taste is weather, not identity. Match the present without imprisoning the future.**
