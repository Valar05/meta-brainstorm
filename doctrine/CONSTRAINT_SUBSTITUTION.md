# Constraint Substitution

**Date:** 2026-09-14
**Status:** active doctrine / derived from Last Convoy lineage

## Source observation

Drew describes Last Convoy as a Snake descendant that deliberately kept **constant movement without attack buttons** while removing one of Snake's defining constraints: collision with your own tail.

The reason is not simplification for its own sake.

In the source game being transformed, self-tail collision supplies movement pressure because there are no enemies competing for the same decision-space role. In Last Convoy, enemies already create dynamic pressure on movement. Retaining self-tail collision would therefore stack a familiar constraint on top of a richer one and reduce the freedom needed to maneuver around hostile threats.

The design move was:

```text
KEEP: constant forward obligation / movement as the primary verb
REMOVE: self-tail collision as an inherited constraint
ADD / PRESERVE: enemy pressure as the more interesting movement constraint
```

## Functional reading

The important thing to preserve from a source mechanic is not every rule. It is the **function** those rules perform.

In Snake, the tail is partly an adversary made from your own history. It forces path planning, spatial memory, and route compression.

In Last Convoy, hostile units and battlefield pressure can perform the route-pressure function more dynamically. Once another system owns that function better, the inherited rule becomes redundant or actively harmful.

This yields a general transformation rule:

```text
SOURCE RULE
-> identify the function it serves
-> ask whether the new system already serves that function
-> if yes, compare which implementation creates richer decisions
-> keep the better pressure, delete the redundant one
```

## Constraint substitution

Call this **constraint substitution**:

> Replace an inherited constraint when a new system produces a richer version of the same decision pressure.

This is not the same as making a game easier.

The total difficulty may stay equal or rise. What changes is the *quality of opposition*.

```text
less self-obstruction
+ more external interaction
= more expressive movement
```

A useful question is:

> Does this constraint create interesting adaptation, or merely consume maneuvering freedom that another system could use better?

## Contact / consequence / adapt connection

The Last Convoy choice increases room for the preferred loop:

```text
CONTACT with enemy / terrain / convoy geometry
-> CONSEQUENCE in formation, damage, route, or threat state
-> ADAPT through movement
```

Self-tail collision would frequently terminate or punish movement before the richer external contact could happen.

The deletion therefore increases fruit density by giving more of the player's movement budget to consequential interaction.

## Important boundary

Do not generalize this into "self-collision is bad" or "external enemies are always better." In another design, self-generated obstruction may be the entire point.

The rule is narrower:

> **When two constraints compete for the same decision role, prefer the one that produces the more interesting adaptation.**

## Compact doctrine

> **Preserve the function, not the inherited rule.**

> **Do not spend movement budget fighting your own mechanic when the world can provide a richer opponent.**
