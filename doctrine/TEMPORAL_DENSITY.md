# Temporal Density

**Date:** 2026-09-14
**Status:** candidate cross-domain doctrine

## Origin specimen

Last Convoy gained throttle after its core movement system already existed. Drew reports that this apparently small addition expanded the game enormously.

The reason is that speed was not isolated. Several systems already depended on time, heading, path history, and enemy interaction.

In the source-backed Last Convoy implementation:

- movement direction controls body orientation;
- the lead cannon auto-fires on a fixed time interval;
- the convoy follows stored position history;
- trail recording is intentionally scaled by speed;
- touch magnitude can reduce or increase commanded travel speed without introducing a separate attack verb.

## Temporal-density view

Throttle can be understood as control over:

```text
world-time spent per unit distance
```

For a fixed-time event with period `T`:

```text
spatial interval ~= speed * T
```

So changing speed changes how densely time-based consequences are packed into space.

This can affect:

- how many timed attacks occur before crossing a region;
- how much heading correction is possible per unit distance;
- how long threats have to act before the player leaves the region;
- how future formation geometry is written while the lead body moves.

## Design consequence

A system does not need another discrete verb to become substantially deeper. Adding one continuous degree of freedom to an existing control can multiply decision regimes when several systems already listen to that variable.

```text
NEW BUTTON
is not the only way to add agency.

EXISTING VERB + NEW DIMENSION
can be much denser.
```

This is especially valuable in compressed games where control purity matters.

## Candidate rules

> **Throttle is not merely speed selection. It is control over temporal density.**

> **Before adding another verb, ask whether an existing verb can gain one meaningful degree of freedom.**

> **A small interface can support a large decision space when one scalar changes several coupled systems at once.**
