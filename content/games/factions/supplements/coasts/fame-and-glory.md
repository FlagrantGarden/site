---
title: Fame and Glory
summary: Subystems for measuring Captains and Groups
draft: false
weight: 10
---

## Fame

Fame is the measure of a Captain's -- and by extension, their Company's -- luck and prowess.

A Captain's Fame affects their ability to recruit and command Groups:

- A Captain can't recruit a Group with more Glory than the Captain's Fame.
- If the point value of a Captain's Company (not counting Champions) exceeds their Fame and they
  face an enemy with more Fame _or_ Glory, roll 1d6 for every company. On a 1--2, the Group refuses
  to fight. If the enemy has more Fame _and_ Glory, roll 1d6 again. On a 1, the Group defects and
  joins the enemy.
- If a Captain has more Fame than a surrendering Group's Glory, roll 1d6. On a 5+, the Group offers
  to join the Captain.
- A Captain's Fame can earn special traits. See [Fame Traits](#fame-traits) for more information.

Captains gain Fame when they lead their folk to battle:

- +VP difference for every victorious skirmish.
- +VP for every revealed Ambition they fulfill.
- +1 for engaging an enemy with more Fame.
- +1 for engaging an enemy worth more points.
- +1 for engaging an enemy that cast any Spells.
- +1 for every skirmish without any of their Groups Routing or Surrendering.
- +1 for every skirmish where every enemy Group Routs or Surrenders.

Captains lose Fame when they fail or act without honor:

- --VP difference for every losing skirmish.
- --VP for every revealed ambition they don't fulfill
- --1d6 whenever they refuse a Duel
- --1 whenever one of their Champions refuse a Duel
- --1d6 whenever the Captain's Group Routs or Surrenders
  - --1 if the enemy had less Glory
  - --1 if the enemy was worth fewer points
  - --1 if the Captain's Group wasn't Bloodied

### Fame Traits

As a Captain's Fame grows, they gain special Traits that affect their leadership, if they meet the
requirements. If they are unable to select a trait because they meet none of the requirements, they
earn the first trait they meet the requirements of.

- At 5 Fame, choose one:
  - **Competent**

    _Must have won more Skirmishes than lost._

    Groups only refuse to fight on a roll of 1 when facing an enemy with more Fame or Glory.
  - **Likable**

    _Must have won a Skirmish, fought in melee, and fought a Duel._

    Groups never defect to join the enemy.
  - **Willing**

    _Must have fought in melee against 3 different Groups._

    +3 Fame for the purposes of recruiting Groups.
- At 10 Fame, choose any prior unselected trait, or:
  - **Brave**

    _Must have the Willing Trait and Attacked 5 Groups with more FS while Bloodied._

    Captain's Group ignores the Terrifying trait and +1 when testing Resolve for Groups within 12".
  - **Clever**

    _Must have the Competent Trait and won 3 consecutive Skirmishes against enemies with more Fame._

    Once per turn, a Group may reroll when activating.
  - **Lucky**

    _Must never have lost a Skirmish._

    Double Fame for the purposes of recruiting Groups. Until the Captain loses a Skirmish, Groups
    never refuse to fight.
- At 25 Fame, choose any prior unselected trait, or:
  - **Charismatic**

    _Must have the Likable Trait and had at least 1 enemy Group defect to their side._

    Enemy Group fighting for a Captain with less Fame refuse to fight on 1--3 and defect on 1--2.
  - **Generous**

    _Must have given at least twice the silver owed after three Skirmishes._

    Groups may reroll failed activations to Move towards an Objective and Resolve tests when not
    Bloodied.
  - **Passionate**

    _Must have passed 5 Resolve tests while Bloodied._

    Groups within 6" ignore penalties on their Resolve test due to lost FS.
- At 50 Fame, choose any prior unselected trait, or:
  - **Fearless**

    _Must have the Brave trait and Attacked at least 20 Groups with more FS or Glory._

    Groups within 12" are immune to the Terrifying trait and reroll failed activations to Attack.
  - **Implacable**

    _Must have fully Routed or Captured at least 3 Companies._

    Groups reroll successful Resolve tests when Attacked by the Captain's Group or a Shieldwall with
    them in it.
  - **Sea Wolf**

    _Must have won at least 10 naval Skirmishes and captured 20 ships._

    Enemy Groups test Resolve when Boarded, rerolling if successful.
- At 100 Fame, choose any prior unselected trait, or:
  - **Blessed**

    _Must have won at least 20 Skirmishes, 3 without any of their Groups Routing or Surrendering._

    +2FS for all Groups. Groups within 12" have +2 when testing Resolve or activating.
  - **Chieftain**

    _Must hold a domain, have won 5 Duels, and have at least 50 Glory._

    Enemy Groups that Rout with remaining FS roll 2d6. If the result is less than their FS, they
    defect instead.
  - **Terror**

    _Must have conquered a domain and Routed at least 25 Groups directly._

    All enemy Groups test Resolve before the Skirmish begins. If they fail, they refuse to fight and
    roll to defect.

## Glory

Glory is the measure of a Group's skill and bravery.

A Group's Glory affects their ability to fight:

- When activating to Attack a Group with more Glory, --1 to the test result.
- When Attacked by a Group with more than twice their Glory, test Resolve.
- When within 6" of a friendly Group with more than twice their Glory, reroll failed Activations.
- A Group's Glory is a prerequisite for Bynames. For more information, see [Bynames][1].

All groups gain Glory:

- +1 for every enemy routed, captured, or vanquished in a Duel.
  - +1 if the enemy had more Glory
  - +1 if the enemy was worth more points
  - +1 if the Group was Bloodied
- +1 for every fulfilled Taunt

They also lose Glory:

- Halve their Glory if they Surrender.
- --1 whenever they Rout  or lose a Duel.
  - --1 if the enemy had less Glory
  - --1 if the enemy was worth fewer points
  - --1 if the Group wasn't Bloodied
- --1 if they fail to fulfill a declared Taunt

[1]: bynames.md
