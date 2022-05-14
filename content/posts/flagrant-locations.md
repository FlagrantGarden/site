---
author: Michael T. Lombardi
date: 2021-10-08
linktitle: Locations in Flagrant Factions
summary: |
  An experimental option for non-player controlled Companies in Flagrant Factions
# menu:
#   main:
#     parent: tutorials
# next: /posts/shortcodes
# # prev: /posts/post-name
categories:
  - mechanisms
tags:
  - flagrant factions
  - experimental
title: Locations
weight: 10
bookComments: true
---

So, as usual, I've been talk to [Sean Richer](https://twitter.com/HypatiasAngst) [again]({{% ref "/posts/taunts" %}}), who is a wellspring of incredible ideas and work.
He struck upon a phenomenal idea I think worth sharing and maybe straight up incorporating into _Flagrant Factions_ at its core: _Locations_.

As written, FF assumes you're playing a fairly narrative game, leaning on scenarios and ambitions to change how every skirmish plays out, even if you're using the same two Companies over and over.

Locations would add another dimension to this: not just _what is this conflict about_ but _where is it taking place?_ and _how does that change things?_

For example, consider the following Locations:

## Location: Minotaur's Maze

> Seemless stone tunnels, winding and meandering; sharp turns and dead ends, plazas plated in bronze that shimmers in firelight.

### Special Rules

Any Group may activate freely to strike or douse a Light;
once a Light is struck, the Group is considered to be carrying Light until they douse it.

Groups not carrying Light move at half speed and cannot see more than 6" through the dark.
When Shooting at a Group not carrying Light, reroll hits.

When fighting in melee and neither side is carrying Light, reroll hits.

Groups carrying Light can see up to 12" and can be seen by any Group which has line of sight, even if they are in the dark.

### The Minotaur

_The Minotaur guards this maze, hunting anyone carrying Light or just foolish enough to get too close._

The Minotaur acts between each side, effectively taking twice as many turns as the players;
it must activate to Attack the nearest Group carrying Light if possible, or any other Group if not.
If the Minotaur cannot Attack a Group on its turn, it instead moves towards the nearest Group carrying Light.

|      ME      |  MI   |  MO   |   R   |   T   | Traits                                            |
| :----------: | :---: | :---: | :---: | :---: | :------------------------------------------------ |
| 3+ / 3+ / 4+ |   -   |  10"  |   6   |   5   | Defiant, Lightbane, Reckless, Terrifying, Vicious |

Defiant
: If the Minotaur is not Shaken and not already in melee, when anyone successfully activates to them,
  they may test at 7+ to meet the enemy halfway and count both sides as attacking for to-hit rolls.

Lightbane
: The Minotaur ignores the Terrifying trait for enemies carrying Light and may reroll to hit them.

Reckless
: If the Minotaur is not Shaken, it **must** activate to Attack if possible.

Terrifying
: When Attacked by the Minotaur, Groups must reroll their highest die when Testing Resilience.

Vicious
: To-hit rolls of 6 inflict two hits.

## Location: Skyboard

> Airships and gliders fill the air, the Leviathan sings softly, clouds battered aside by its great tail.

### Special Rules

Players must deploy their Groups onto one of the airships or the back of the Leviathan.

Any Group except for Engines may attempt to activate to Glide and Move across the open air up to 12" (10" if Heavy); Foot do so on a 5+, Beasts on a 6+, and Cavalry on a 7+.

A Group in uncontested control of an airship may activate on a 5+ to maneuver the airship 6" in any direction.

If any side has sole control of the Leviathan at the end of play, +3VP.
If any side kills the Leviathan they gain +2VP.

### The Leviathan

_The skywhale is a magnificent creature; a floating fortress, a supply of precious oil, and a catastrophic war weapon, if it wants to be._

On the first turn, roll a d6; the Leviathan will act after that many turns unless attacked, in which case it acts next.
After each of the Leviathan's turns, roll a d6; it activates again after that many turns.

The Leviathan moves lazily across the sky, indifferent to the puny airships in its way;
roll 2d6: if the result is even, the leviathan moves to its left; if odd, to its right.
If the result is less than or equal to seven, it moves backward; if more, forward.

The Leviathan cannot Attack but it will defend against any attackers.
On its next activation after being Attacked, it will sing the Skysunder Song.

If the Leviathan is reduced to less than 3R, it self destructs on its next activation unless reduced to 0R first.

If the Leviathan is killed, roll a d6; it plummets out of the sky after that many turns, automatically Routing any Group still aboard.

|     ME     |  MI   |  MO   |   R   |   T   |                       Traits                        |
| :--------: | :---: | :---: | :---: | :---: | :-------------------------------------------------: |
| - / - / 3+ |   -   |  6"   |  12   |   4   | Annihilator, Self-Destruct, Skysunder Song, Vicious |

Annihilator
: Whenever the Leviathan moves into any model from a Group, roll to-hit as if the Leviathan is defending from an Attack.
  Any airship the Leviathan moves into is destroyed and any Groups the airship was carrying are now on the Leviathan.

Self-Destruct
: Shoot every Group within 6", hitting on 3+; any Group aboard the Leviathan when it self-destructs is automatically Routed.

Skysunder Song
: The Leviathan croons to the eldritch winds; Shoot every Group except the Leviathan, hitting on 6.

Vicious
: To-hit rolls of 6 inflict two hits.

## Location: The Arena

_Bloodthirsty crowds look on in delight, excited to vote and change the game according to their whims_

### Special Rules

Groups may not Retreat off of the table; treat the edge as Impassable terrain.

The Crowd may grow bored with the game; after each turn, roll a d6; if the result is greater than the amount of R lost that turn, -1 from their Excitement.
The Crowd's Excitement starts at 6.

If the Crowd's Excitement reaches zero, roll 2d6 as they vote to shake things up:

| Result |    Name     | Effect                                                                                                                                 | Excitement Bonus |
| :----: | :---------: | :------------------------------------------------------------------------------------------------------------------------------------- | :--------------: |
|   2    |    Chant    | None.                                                                                                                                  |        +3        |
|   3    |    Stone    | All groups within 12" of the table edge are at risk; 6d6, hitting on 6                                                                 |        +2        |
|   4    |   Favour    | The Group that has hurt enemies the most regains up to 2R and may activate freely next turn                                            |        +2        |
|   5    |    Duel     | The most recent Groups to fight in melee must fight until one side is Routed; all other activations and effects are on hold until then |        +4        |
|   6    |  Inebriate  | Any Group that moves adjacent to the table edge may activate freely to drink divine wine; +1T but become Reckless and Unfeeling        |        +2        |
|   7    |  Blessing   | The Group that has hurt enemies the most returns to their starting R and rolls an additional 3 dice to hit                             |        +1        |
|   8    |   Unleash   | Add three Light Beast Groups to the arena; they always Attack the nearest Group if possible, else Move towards it                      |        +3        |
|   9    | Second Wind | All Groups in the Arena return to half their R if Bloodied or full if not                                                              |        +1        |
|   10   | Wallscythe  | All Groups within 6" of the table edge are at risk; 12d6, hitting on 4+                                                                |        +2        |
|   11   | Earthquake  | All Groups are at risk; 12d6, hitting on 5+                                                                                            |        +3        |
|   12   |    Flood    | The entire Arena becomes Difficult terrain                                                                                             |        +2        |
|   13   |    Curse    | The Group that has hurt enemies the least is targeted; 12d6, hitting on 3+; for the rest of the skirmish, -1T                          |        +1        |
|   14   |  Executor   | Add an Elite Foot Group to the arena; they always Attack the nearest Group if possible, else Move towards it                           |        +2        |
|   15   |   Inferno   | For the remainder of the skirmish, on any turn the Crowd would be bored, all Groups are at risk; 6d6, hitting on 3+                    |        +5        |

After a result is selected, cross it out, the crowd never does the same thing twice.
If a crossed out result is selected, choose the next highest result instead.

Each time the Crowd votes to shake things up, +1 to the result.

If all results are crossed out before the skirmish ends, all Groups are counted as Routed and everyone loses as flames burn all to ash.

## Location Design

These example locations are about as complex as I think could work, but you could lean much, much simpler, as Sean did in this example for his just-announced [_Crapland._](https://www.drivethrurpg.com/product/373346/crapland-splatter-edition-TROIKA-COMPATIBLE) supplement for _Flagrant Factions_:

> ### The Wide House
>
> wide enough to be a grocery store. Also has a good selection of local music. Also has a bowling alley. Also does like glow-in-the-dark smoothies after dark. > > That’s decidedly NOT crappy.
>
> Passive
> : Shaken Groups are knocked prone and must spend a move Action to get back up.
>
> Alternate Victory
> : Gain +1 VP every time you knock down a group within 6” of table edge. STRIKE!

Locations work best when they:

* Introduce new gameplay elements
* Bring a strong theme
* Incite interesting choices

I'm not yet sure if Locations will make it into the base game or not;
if you think they should, drop a line here or on Twitter and let me know!
