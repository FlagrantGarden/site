---
title: "Fleets"
description: "Rules, groups, and traits for naval forces."
draft: false
weight: 60
---

## Fighting on the Water

For naval skirmishes, characters must join a Group. They still fight as a [Champion][1] if
[Duelling][2]. Naval skirmishes involve fleets of Ship Groups.

Ship Groups have their own profile and are crewed by one or more Crewing Groups. Each Ship Group
requires a minimum number of Crewing Groups to row at full speed. Count each Bloodied Crewing Group
as 1/2 a Group for this purpose. If the Ship Group is reduced to fewer than half their required
Crewing Groups, they may only move 1" or [Drift][3].

Ship Groups have an alternate ME profile for [Boarding][4] or [Ramming][5]. The first value is the
target for activating to Board. The second value is the target for activating to Ram. The third
value is the target when rolling to hit while Ramming.

Ship Groups do not have an MI profile. For more information, see [Artillery and Shooting][6].

Ship Groups have an alternate MO profile. The first value is the target for activating to Move. The
second number is their speed when rowing. The third number is their speed when sailing across the
wind. For more information, see [Moving and Drifting][3].

Ship Groups do not have Resolve. Their FS represents how capable the ship physically is of
continuing to fight. When a Ship Group loses FS, all Crewing Groups test Resolve. For more
information, see [Resolve, Jumping Ship, and Mutiny][7]

### Moving and Drifting

Moving on the water is different from on land. After a Ship Group Moves, they continue half that
distance in the same direction on their next turn unless they Weigh Anchor or Move again.

Ship Groups can freely activate to Weigh Anchor, holding themselves in position. Unless a Ship Group
Weighs Anchor, they Drift every turn they are not Moving or Attacking. Ship Groups are less prone to
drifting the larger they are. Ship Groups that are Drifting always move at least 1". Adjust how much
a Ship Group Drifts by their initial FS:

|  FS   | Drift Rate Reduction |
| :---: | :------------------: |
|  <4   |          -           |
| 4--5  |         --1"         |
| 6--8  |         --2"         |
| 9--11 |         --3"         |
|  12+  |         --4"         |

In a river, Ship Groups move downstream with the current. The distance they move is the river's
Drift Rate, based on the size and speed of the river.

| Size / Speed | Slow  | Moderate | Fast  |
| :----------: | :---: | :------: | :---: |
|  **Small**   |  1"   |    2"    |  3"   |
|  **Medium**  |  2"   |    3"    |  4"   |
|  **Large**   |  3"   |    4"    |  5"   |

When sailing upriver, subtract the river's Drift Rate from the Ship Group's speed. When sailing
downriver, add it. A Ship Group's size modifier affects both directions.

At sea, Ship Groups drift with the wind. The wind's Drift Rate correlates to its strength:

|     Wind      | Distance |
| :-----------: | :------: |
|     Calm      |  - / -  |
| Light Breeze  | 1" / 1"  |
| Strong Breeze | 3" / 2"  |
| Gale / Storm  | 5" / 3"  |

When Drifting with sails unfurled, move the Drift Rate's first value in the wind's direction. When
Drifting with sails furled, move the Drift Rate's second value instead.

If Moving with sails unfurled, the wind's Drift Rate affects a Ship Group's speed:

- Subtract the first value of the Drift Rate if sailing directly into the wind.
- Subtract the second value of the Drift Rate if sailing into-and-across the wind.
- Ignore the Drift Rate if sailing across the wind.
- Add the second value of the Drift Rate if sailing before-and-across the wind.
- Add the first value of the Drift Rate if sailing directly before the wind.

### Artillery and Shooting

A Ship Group with Crewing Groups that have an MI profile can Shoot as part of the Ship Group's Shoot
or Move activation. When Crewing Groups Shoot, they do so together. Choose whether they are
targeting the enemy Ship Group or its Crewing Groups. Unless the Crewing Group is using flaming
missiles, they can't harm an enemy Ship Group.

Choose the Crewing Groups that are Shooting. Use the worst profile from the participating Groups for
range and to-hit. For every participating Group after the first, roll +1 dice to hit. Unless the
Ship Group has [Weighed Anchor][3], reroll hits.

If the Crewing Group Shoots flaming missiles at a Ship Group and inflict enough hits to reduce its
FS, the target Ship Group catches fire. For more information, see [Fire][8].

If the Crewing Group Shoots at a Ship Group's Crewing Groups, distribute the inflicted hits amongst
those Groups. If any of them lose FS they Test Resolve. If they fail, all Crewing Groups test
Resolve one by one to see if panic spreads with a --1 penalty for every prior Group that failed.
For more information on failing Resolve tests, see [Resolve, Jumping Ship, and Mutiny][7].

Ship Groups may be fitted with artillery, but never by default. Artillery includes the ballista,
catapult, and mangonel.

Ballista
: Shoots bolts or stones accurately. Hit on 5+ (4+ if the Group has Weighed Anchor). Must activate
  once to load, once to prepare, and once to loose.

Catapult
: Lobs heavy missiles inaccurately. Hit on 6+ (5+ if the Group has Weighed Anchor), Ignore T, reroll
  hits, and count 6s as two hits. Must activate once to load, once to prepare, and once to loose.

Mangonel
: Lobs moderate missiles inaccurately. Hit on 6+ (5+ if the Group has Weighed Anchor), reroll hits,
  and count 6s as two hits. Must activate once to load and once to loose.

### Beaching and Disembarking

A Crewing Group can always disembark in shallow water by activating to Move and leaping overboard.
They treat the shallow water as difficult terrain unless they have the Sealegged trait. If the Ship
Group has not Weighed Anchor, reroll their activation test.

Ship Groups with the Beachable trait may Move onto the beach. Their Crewing Groups may immediately
disembark and fight on land as normal.

A disembarked Crewing Group may Move back onto a Ship Group to join or rejoin the crew.

### Boarding

A Ship Group may Attack another Ship Group to Board them. If successful, choose any number of
Crewing Groups to commit to the Attack. Each participating Group must activate to Attack. Only
successfully activating Groups join the Boarding Party.

Groups that are in a Boarding Party combine their FS and:

- +1 to Resolve tests per Group in the Boarding Party
- +1 dice per Group in the Boarding Party when rolling to hit.

Choose an enemy Crewing Group to Attack directly.

When a Ship Group is Boarded, their Crewing Groups can fight the Boarding Party or form their own
Boarding Party and Board the enemy Ship Group following the same procedure, except that a Crewing
Groups already in melee can't join a Boarding party.

Groups fighting on ship decks without training and experience make more mistakes than usual. When
rolling to hit while Boarding, reroll any 6s unless half the involved Crewing Groups have the
Sealegged trait.

### Ramming a Ship

Most ships are not made for ramming. Unless a Ship Group has the Ramming trait, roll 1d6 when they
ram another Ship Group. On a 1--2, --1 FS. On a 3--4, --2 FS. On a 5, --3 FS. On a 6, they begin
Sinking. Refer to _Wolves Upon the Coast_ for details on sinking ships.

Roll 12d6 (6d6 if Bloodied) against the rammed Ship Group. If ramming inflicts enough hits to reduce
the target's FS, it may start to sink.

After successfully ramming, test to activate again immediately: Move away (8+) or Board (7+).

### Fire

When a Ship Group catches fire, the crew may activate (6+) to put it out. --1 to the result for the
initial FS loss that caused the fire and --1 to the result for each turn the Ship Group has been on
fire.

### Resolve, Jumping Ship, and Mutiny

If at least half the Crewing Groups of a Ship Group are Shaken, the Ship Group Retreats and the
Crewing Groups must Rally next turn. Until at least half the Crewing Groups successfully Rally, the
Ship Group Drifts.

If a Crewing Group's result when testing Resolve is 0 or less while on a river or in sight of the
shore, that Group Jumps Ship and Retreats off the field at full speed. If an enemy Ship Group moves
adjacent to them while in the water, they may activate to Capture the fleeing Group.

If a Crewing Group's result when testing Resolve is 0 or less while on the open sea, they Mutiny.
They immediately Attack non-shaken Crewing Groups. Resolve the Attack, then test Resolve for other
Shaken Crewing Groups one by one to see if the Mutiny spreads with a --1 penalty for every
Mutinying Group.

If a Ship Groups remaining Crewing Groups are all in Mutiny, roll 1d6. On 1--3, they Ship Group
surrenders and is Captured. On a 4--6, they Retreat and flee the skirmish. If Boarded, they
surrender and are Captured.

## Ship Groups

The following Groups represent common vessels. Their profiles are already adjusted for any traits
they have.

|     Name      |      ME      |       MO       |  FS   |   T   |  Traits   |
| :------------ | :----------: | :------------: | :---: | :---: | :-------- |
| Raft          |  5+ / - / -  |  5+ / 6" / -   |   2   |       | Beachable |
| Boat          |  5+ / 6 / 6  |  5+ / 8" / 8"  |   4   |   1   | Beachable |
| Karvi         | 4+ / 6 / 5+  | 5+ / 8" / 12"  |   6   |   2   | Beachable |
| Knarr         | 5+ / 6 / 5+  | 5+ / 6" / 14"  |   6   |   2   | -         |
| Snekkja       | 4+ / 6 / 4+  | 5+ / 8" / 16"  |   8   |   2   | Beachable |
| Galley, Noos  | 5+ / 4+ / 3+ | 5+ / 6" / 16"  |   8   |   3   | Ramming   |
| Galley, Small | 5+ / 6 / 4+  | 5+ / 6" / 16"  |   8   |   3   | -         |
| Galley, Large | 5+ / 6 / 3+  | 5+ / 8" / 20"  |  12   |   4   | -         |
| Skeid         | 3+ / 5+ / 4+ | 5+ / 10" / 18" |  10   |   4   | Beachable |

## Ship Group Traits

### Beachable

Ship Groups with the Beachable trait may Move onto the beach. Their Crewing Groups may immediately
disembark and fight on land as normal.

### Ramming

Improve activation and to-hit when activating to Ram another Ship Group. Ship Groups with this trait
do not take damage when they Ram another Ship Group.

[1]: characters-and-duels.md#champions
[2]: characters-and-duels.md#duelling
[3]: #moving-and-drifting
[4]: #boarding
[5]: #ramming-a-ship
[6]: #artillery-and-shooting
[7]: #resolve-jumping-ship-and-mutiny
[8]: #fire
