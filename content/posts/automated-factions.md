---
title: Automated Companies
author: Michael T. Lombardi
date: 2021-09-20
linktitle: Automated Companies in Flagrant Factions
summary: >
  An experimental option for non-player controlled Companies in Flagrant Factions
categories:
  - mechanisms
tags:
  - flagrant factions
  - experimental
weight: 10
bookComments: true
---
Thinking about play in [*Flagrant Factions*]({{/games/factions) it occurred to me that it would be useful to add automated procedures for playing solo or even just relegating one of multiple companies to automated activations for more complex scenarios.

The [onepagerules](https://onepagerules.com/) wargames include some fairly detailed automated processes for solo play and [Richard Cowen wrote some interesting procedures](https://richardcowen.wordpress.com/2020/04/12/wargaming-dragon-rampant-solo-rampant/) for [Dragon Rampant](https://ospreypublishing.com/dragon-rampant).
This post takes some inspiration from both.

## Are Automated Procedures Even Necessary?

In a word: no.

But they *can* be useful, of course.
It's not always easy to play the opposition fully in a skirmish and when there's multiple players at cross purposes, even less so.

Automated processes can help reduce cognitive load for players and/or make for play that *feels* more like facing opposition rather than playing with yourself otherwise might.

## On Efficacy and Standardization

Not only are these rules an optional subsystem, they should absolutely be considered malleable and hackable in the broad sense and be suborned to the needs of the table--like all rules, really.
If something isn't working or doesn't make sense, alter it for yourself.
Experiment, try things!

I believe in you.

## Setup

### Traits

Most traits, \[captain]({{< ref "/games/factions/rules#captains" >}}) and \[otherwise]({{< ref "/games/factions/rules#profile-traits" >}}), work fine regardless of whether the Group is automated or player-run.
Where the traits would be triggered by choice, unless otherwise specified, roll a d6: on a 4+, the trait is triggered.

### Personalities

Companies using automated procedures can have a Personality; this impacts the decisions they make and how they play. Roll a d6 or choose for each automated Company:

1. **Arcane:** Will prefer to use and acquire magic over mundanity
2. **Bold:** Will chase objectives and move without concern for enemy action
3. **Cautious:** Will attempt to steer clear of enemies unless odds are favorable
4. **Ferocious:** Will attempt to destroy the enemy whenever possible
5. **Guarded:** Will avoid attacking directly, preferring to hold and whittle
6. **Incompetent:** Will follow default/random orders

### Initiative

\[As usual]({{< ref "/games/factions/rules#setup" >}}), initiative is a 1d6 roll off, with some preferences:

* Bold and Ferocious Companies will prefer to be on the offensive
* Cuatious and Guarded Companies will prefer to be on the defensive
* Arcane Companies will prefer whichever role is more magical (e.g., the ritualists in the Ritual scenario)
* Incompetent Companies automatically forfeit their roll, counting as a 1 for all purposes

If the automated Company's Captain has the Shrewd trait, they will use it towards their preference.

### Deploying

Automated Companies deploy per the scenario's guidance, with some alterations.
First, define four quadrants on the table that include the valid deployment zones for this scenario.
Unless otherwise specified, follow this process:

1. Line up the automated Company's Groups from lowest to highest point value
2. Roll 1d6 to deploy the first Group:

   * If the result is *even*, deploy the group furthest right in the line to the nearest deployment zone
   * If the result is *odd*, deploy the group furthest left in the line to the furthest deployment zone
3. For each remaining Group, roll 1d6:

   * Select the Group from the right/left of the line if the result is even/odd respectively
   * If the result is *lower* than the previous roll, deploy in an adjacent quadrant
   * If the result is *equal* to the previous roll, deploy in the same quadrant
   * If the result is *higher* than the previous roll, deploy in the opposite quadrant
4. Depending on the Company's Personality, these deployments may need to be adjusted, either swapping Groups or moving them within their deployment quadrant:

   * Arcane Companies must deploy their magic using Groups within 6" of a friendly group if possible
   * Bold Companies must deploy their Groups as near as possible to an enemy or objective
   * Cautious Companies must deploy their Groups with Shooting, Casting, or Summoning orders within 6" of a friendly group and as far from enemy Groups as possible
   * Ferocious Companies must deploy their Groups within range to Attack or Shoot if at all possible
   * Guarded Companies must deploy their groups within 6" of a friendly Group; if any Groups have the Defensive trait, they must be evenly dispersed amongst Group clusters

### Ambitions

Automated Companies may have \[Ambitions]({{< ref "/games/factions/rules#ambitions" >}}).
For each Ambition listed for the Personality, roll a d6: on a 4+, they are choosing that Ambition.
Automated Company Ambitions always count as revealed.

* **Arcane:** Give Better Than We Get, Draw First Blood,They Will Know My Name
* **Bold:** They Will Reel Before Us, Give Better Than We Get, Draw First Blood, They Will KNow My Name
* **Cautious:** We Will Not Break, Give Better Than We Get, Rain Hell Upon Them
* **Ferocious:** They Will Reel Before Us, We Will Snap Their Spine, Break Even Their Anvil, Draw First Blood, We Will All Shed Blood
* **Guarded:** We Will Not Break, Win Without Moving, Do Not Waver, Give Better Than We Get, Rain Hell Upon Them
* **Incompetent:** None.

## Automated Turns

Automated Companies \[start their turn as normal]({{< ref "/games/factions/rules#activation-phase" >}}), rallying Shaken Groups and then testing for Reckless Groups.

When activating individual Groups, unless specified, they follow this process:

1. Must activate the Captain's Group first, then the closest Group to the Captain's Group which has not yet activated.
2. Roll 1d6 to determine the activation: Move (1-2), Attack (3-4), Shoot (5-6); if the group cannot perform the specified action, default to the lower-order action until they can.

   * If moving, roll 1d6 and: move away from nearest enemy (1-2), move towards nearest enemy (3-4), move towards nearest objective (5-6)
3. Resolve each activation as normal.

### Arcane Group Activations

Arcane Companies must activate any Groups with the Casting, Apprentice, or Summoner traits before others, from highest to lowest point value.
Groups capable of the Casting or Summoning order *must* use that order; if capable of both, alternate between them each time.

### Bold Group Activations

Bold Companies must activate the Group nearest an enemy or objective first, then the next closest Group, and so on.
Groups capable of seizing an objective or attacking an enemy must do so (preferring objectives over attacking).

### Cautious Group Activations

Cautious Companies activate as normal but may not activate to Attack an enemy Group whose R is equal to or greater than their own.
Groups more than 6" away from a friendly Group must Move towards one if possible.

### Ferocious Group Activations

Ferocious Companies must activate the Group nearest an enemy first, then the next closest Group, and so on.
Groups capable of Attacking or Shooting must do so, preferring whichever activation order has a better hit chance.
Groups not within range of an objective or enemy must Move towards the nearest enemy Group.

### Guarded Group Activations

Guarded Companies activate as normal but may not activate to Attack an enemy Group unless a friendly Group is within 12". Groups not within 12" of a friendly Group must move towards the nearest friendly Group or defensible position.

## Eccentrics

* Groups in Bold and Ferocious Companies with the Defiant trait must always test to activate it in response to being Attacked
* Groups in Cuatious and Guarded Companies with the Elusive trait must always test to activate it in response to being Attacked
* Spells are chosen randomly unless specified beforehand
* Groups with the Casting order may not activate to Cast the same spell twice in a row and cast in one of two orders:

  1. If the Company has the Arcane Personality, cast from highest activation difficulty to lowest if there is a valid target; otherwise cast the next highest difficulty spell; may not recast the same spell until all known spells have been attempted at least once
  2. Otherwise, cast randomly against nearest valid target
* Groups with Foe or Bane traits *must* Move towards and attempt to Attack the nearest specified Kind of Group if within 18"
* Groups with Self-Destruct trait *must* attempt to activate it once they are under half their starting R

## Wrapup

So! That's it for this first pass.
Mainly what this guidance does is point you in the direction of an automated procedure for narrative skirmish play;
in this draft most special rules hang off of the automated Company's Personality.

To write up your own custom Personality, consider:

* What's their overall approach to a skirmish?
* What preferences do they have when determining a side for a scenario?
* What special considerations make sense during deployment?
* Which ambitions is a Company with this Personality likely to take on?
* How will this Personality trait affect activation in terms of which Group to activate next and which activations they can be given?

I'll probably ruminate on this a bit more, I'd love to hear your thoughts and especially how any playtesting goes!

You can reach out to me on [Twitter](https://twitter.com/TrebuchetOps) if you'd like to get the link to a [Tabletop Simulator](https://store.steampowered.com/app/286160/Tabletop_Simulator/) mod which brings the base rules for Flagrant Factions into TTS along with a couple predefined groups!

Cheers, folks!