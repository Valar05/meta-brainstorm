# Shared-Verb Conflict

**Date:** 2026-09-14
**Status:** active doctrine / cross-domain hypothesis
**Primary specimen:** Last Convoy

## Observation

A small control vocabulary does not require a small decision space.

Last Convoy demonstrates a stronger mechanism than mere input compression: one player verb can serve multiple systems that want different things at the same moment.

The lead vehicle moves continuously. Its main cannon auto-fires on a recurring timer and inherits the vehicle's current body rotation as shot direction. The same movement also writes the position trail later used by convoy followers.

Thus steering near a firing event simultaneously affects:

```text
immediate offensive geometry
+
delayed convoy geometry
```

The goals can conflict. Pointing the lead vehicle to make the next shot useful may produce a path shape that is worse for the convoy, and positioning the convoy cleanly may sacrifice the cannon's next firing angle.

## Shared-verb conflict

Define a **shared verb** as one control action whose state feeds more than one consequential subsystem.

The verb becomes interesting when those subsystems are not perfectly aligned.

```text
one verb
-> consequence A
-> consequence B

where optimizing A can worsen B
```

This creates decision depth without adding another button.

The critical distinction is:

```text
shared function with aligned goals = convenience
shared function with competing goals = decision
```

## Temporal version

Last Convoy also separates the consequences in time.

```text
NOW:
orient the vehicle for the sampled cannon shot

LATER:
the convoy follows the route just authored
```

This means one action is evaluated against more than one clock.

> **One verb becomes deep when its consequences arrive on different clocks.**

## Relation to fruit density

Shared-verb conflict is a high-density way to create depth.

Instead of adding a separate aim stick, attack button, formation screen, or tactical mode, the system reuses steering and allows the conflicts among consequences to generate the decision space.

This can preserve purity because the player's vocabulary remains small while the world becomes more articulate.

## Guardrail

Do not force unrelated systems onto the same verb merely to reduce button count. Shared-verb conflict is useful when the coupling is legible and causal.

A player should be able to learn:

```text
I turned for the shot,
therefore I bent the convoy route.
```

If the second consequence feels arbitrary or invisible, the compression becomes control ambiguity rather than depth.

## Compact doctrine

> **Do not measure control depth by button count. Measure how many meaningful, legible obligations each verb carries.**

> **Steering can be both reticle and choreography.**
