---
title: Routines
date: 2022-06-12
summary: Rules for non-player Companies in Flagrant Factions
weight: 50
---

These procedures and guidelines apply to Companies not controlled by a player. Unless otherwise
specified, Routine Companies follow the same rules as other companies. Where decisions are unclear,
use judgement.

<!-- vale Contractions.Use = NO -->

{{< hint info >}}
This section assumes skirmishes fought between two sides, each with a single company. If you're
playing with more sides or more companies, use your judgment.
{{< /hint >}}

<!-- vale Contractions.Use = YES -->

## Personalities

Routine companies have a Personality. Roll 1d6 or choose for each Routine Company:

1. **Incompetent:** Follow default orders.
1. **Arcane:** Prefer to use and acquire magic over the mundane.
1. **Bold:** Chase objectives and move with no concern for enemy action.
1. **Cautious:** Steer clear of enemies unless odds are favorable.
1. **Ferocious:** Destroy the enemy whenever possible.
1. **Guarded:** Avoid attacking directly, prefer to hold and whittle the enemy down.

## Traits

When a Routine Company might choose to trigger one of their traits, roll 1d6: on 4+, they trigger
the trait.

## Setup

### Initiative

Incompetent Companies automatically forfeit their initiative roll, counting as a 1 for all purposes.
When a Routine Company wins the initiative roll-off:

If the Routine Company's Captain has the Shrewd trait, they use it according to their preference:

- Bold and Ferocious Companies prefer to be the attackers.
- Cautious and Guarded Companies prefer to be the defenders.
- Arcane Companies prefer whichever role is more eldritch (e.g. the ritualists in the Ritual
  scenario). If unclear, they choose at random.

### Deploying

Routine Companies deploy in accordance with the scenario, but with some alterations. Define four
quadrants on the table that include the valid deployment zones for the Routine Company in the
scenario. Follow this process:

1. Line up the Routine Company's Groups from lowest to highest point value along one edge of the
   table.
1. To deploy the first Group, roll 1d6:
   - If the result is _even_, deploy the group farthest right in the line to the nearest deployment
     zone.
   - If the result is _odd_, deploy the group farthest left in the line to the farthest deployment
     zone.
1. For each remaining Group, roll 1d6:
   - If the result is _odd_, select the left-most Group. If even, select the right-most Group.
   - If the result is _lower_ than the previous roll, deploy the selected Group in an adjacent
     quadrant (chosen at random).
   - If the result is _equal_ to the previous roll, deploy in the same quadrant.
   - If the result is _higher_ than the previous roll, deploy in the opposite quadrant.
1. Adjust the Company's deployment based on their personality, as needed:
   - Arcane Companies must deploy Groups with the Casting or Summoning order within 6" of a friendly
     group, if possible.
   - Bold Companies must deploy their Groups as close an enemy or objective as possible.
   - Cautious Companies must deploy their Groups with Shooting, Casting, or Summoning orders within
     6" of a friendly group and as far away from enemy Groups as possible.
   - Ferocious Companies must deploy their Groups within range to Attack or Shoot, if possible.
   - Guarded Companies must deploy their groups within 6" of a friendly Group. If any Groups have
     the Defensive trait, they must be as evenly dispersed among Group clusters as possible.
   - Whenever a decision is unclear, choose at random.

### Ambitions

Routine Companies may have [Ambitions][1], based on their Personality. For each Ambition listed next
to the Routine Company's Personality below, roll 1d6. On a 4+, they have that Ambition. Routine
Company Ambitions always count as revealed.

- **Arcane:** Give Better Than We Get, Draw First Blood,They Will Know My Name.
- **Bold:** They Will Reel Before Us, Give Better Than We Get, Draw First Blood, They Will Know My
  Name.
- **Cautious:** We Will Not Break, Give Better Than We Get, Rain Hell Upon Them.
- **Ferocious:** They Will Reel Before Us, We Will Snap Their Spine, Break Even Their Anvil, Draw
  First Blood, We Will All Shed Blood.
- **Guarded:** We Will Not Break, Win Without Moving, Do Not Waver, Give Better Than We Get, Rain
  Hell Upon Them.
- **Incompetent:** _None_.

## Turns

Routine Companies start their turn by rallying Shaken Groups then testing for Reckless Groups, as
normal.

Individual Groups follow this process when activating, unless specified otherwise:

1. Must activate the Captain's Group first, then the Group closest to the Captain's Group that has
   not yet activated.
1. Roll 1d6 to determine the Group's activation: (1--2) Move, (3--4) Attack, (5--6) Shoot. If the
   group cannot perform the specified action, default to the next lower-order action until they can.
   - If activating to Move, roll 1d6 and: (1--2) Move directly away from the nearest enemy, (3--4)
     Move toward the nearest enemy, (5--6) Move toward the nearest objective.
1. Resolve each activation as normal.

### Arcane Group Activations

Arcane Companies must activate any Groups with Cast or Summon orders before others, from highest to
lowest point value. Groups capable of the Casting or Summoning order _must_ use that order, if
possible. If capable of both, alternate between them.

### Bold Group Activations

Bold Companies must activate the Group nearest an enemy or objective that has not already activated.
Groups capable of seizing an objective or attacking an enemy must do so, preferring objectives over
attacking.

### Cautious Group Activations

Cautious Companies never Attack an enemy Group whose R is equal to or greater than their own.
Groups more than 6" away from a friendly Group must Move toward one, if possible.

### Ferocious Group Activations

Ferocious Companies must activate the Group nearest an enemy that has not already activated. Groups
capable of Attacking or Shooting must do so, preferring whichever order has a better chance to hit
Groups not within range of an objective or enemy must Move toward the nearest enemy Group.

### Guarded Group Activations

Guarded Companies may not activate to Attack an enemy Group unless there is a friendly
Group within 12". Groups not within 12" of a friendly Group must move toward the nearest
friendly Group if possible, or toward the nearest defensible position otherwise.

## Eccentrics

- Groups in Bold and Ferocious Companies with the Defiant trait must always test to activate that
  trait when possible.
- Groups in Cautious and Guarded Companies with the Elusive trait must always test to activate when
  possible.
- Choose spells randomly unless specified otherwise.
- Groups with the Casting order may not activate to Cast the same spell twice in a row.
- If a Company has the Arcane Personality, they may not recast the same spell until they have
  attempted all their known spells at least once. When choosing a spell to Cast, they must choose
  the remaining spell with the highest activation difficulty from among those with a valid target.
  Otherwise, they must Cast a random spell against the nearest valid target.
- Groups with Foe or Bane traits must Move towards and attempt to Attack the nearest specified type
  of Group if within 18" of one.
- Groups with Self-Destruct trait must attempt Self-Destruct once they are Bloodied.

<!-- Reference Links -->

[1]: {{% ref "/games/factions/rules#ambitions" %}}
