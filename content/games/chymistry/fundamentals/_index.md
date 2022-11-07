---
title: Fundamentals
description: |
  The basics of chymistry
bookCollapseSection: true
weight: 30
---

### Testing

Chymist's must often test their art to prepare or research formulae. To do so, they follow this
order of operations:

1. Determine the difficulty tier of the test. If the difficulty less than 1, no test is required. If
   the difficulty is higher than 6, it is impossible for the chymist.
2. Determine which rating to use as the expertise rating for the test.
   1. If preparing or researching a formula, any relevant rated quality may be used as the expertise
      rating.
   2. If preparing a memorized formula, that formula's rating may be used as the expertise rating.
   3. If the chymist has no relevant quality and is not preparing a memorized formula, they have no
      expertise rating for the test and must rely on their base chymistry alone.
3. Roll a d66:
   1. If the result is less than the difficulty tier (default 1), fail.
   2. If the result is less than the chymist's chymistry or expertise rating, pass.
   3. If the result is equal to the chymist's chymistry or expertise rating, triumph.
   4. If the result is over the chymist's chymistry and expertise rating but the degree die is less than
      the tier of their expertise, pass.
   5. Fail. If the result of the failure
      was a 66, and the test was not _already_ subject to a mishap, roll a d66 on the
      [Mishap Table](#mishaps).

#### Difficulty

The difficulty of a chymical test is represented by this equation:

{{< katex display >}}
\begin{aligned}
   \delta(\Pi, f^T, f^R, \phi^C, \Sigma^{^T_R}, \lambda, \rho) &=
   1 +
   \Delta_u(f^T_{\mu}, \phi^C, \Sigma^{^T_R}) +
   \begin{cases}
      \Delta_r &\text{if } \Pi \equiv \text{\textquotedblleft} Researching \text{\textquotedblright} \\
      \Delta_p &\text{if } \Pi \equiv \text{\textquotedblleft} Preparing \text{\textquotedblright} \\
   \end{cases} \\
   \\
   \Delta_u(\mu, \phi^C, \Sigma^{^T_R}) &=
   \Sigma^{^T_R} +
   \bigl( \thinspace \mu \gt \phi^C_T \to \mu - \phi^C_T \thinspace \bigr) \\
   \\
   \Delta_r(\lambda) &= \nexists \lambda \to 1 \\
   \\
   \Delta_p(f^R, f^T, \Mu, \phi^f) &=
   \begin{pmatrix}
      \begin{aligned}
         &\bigl(
            \thinspace f^R_{\iota} \setminus f^T_{\iota} \thinspace
         \bigr)
         \\
         +
         &\bigl(
            \thinspace f^R_{\mu} \ne f^T_{\mu} \to \vert f^R_{\mu} - f^T_{\mu} \vert \thinspace
         \bigr)
         \\
         +
         &\begin{cases}
            -1 &\text{if } \nexists{\Mu} \\
            -\phi^M_T &\text{if } \exists{\Mu} \And \exists{\phi^f} \\
         \end{cases}
      \end{aligned}
   \end{pmatrix}
   \centerdot
   \begin{cases}
      1 &\text{if } f^R_{\pi} \equiv f^T_{\pi} \\
      2 &\text{if } f^R_{\pi} \ne f^T_{\pi} \\
   \end{cases} \\
\end{aligned}
{{< /katex >}}

These complexities becomes clear with mere inspection. For a step-by-step summary in plain language,
see the ordered list at the end of this section.

The difficulty of any chymistry test, {{< katex >}}\delta{{< /katex >}}, is defined as
{{< katex >}}1{{< /katex>}} plus the universal modifier ({{< katex >}}\Delta_u{{< /katex >}})
plus either the research modifier ({{< katex >}}\Delta_r{{< /katex >}}) or preparation modifier
({{< katex >}}\Delta_p{{< /katex >}}), depending on the purpose of the test.

The input variables are:

- {{< katex >}}\Pi{{< /katex >}}, the purpose of the test,
- {{< katex >}}f^T{{< /katex >}}, the formula being prepared or researched,
- {{< katex >}}f^R{{< /katex >}}, the reference formula (undefined except when preparing a formula),
- {{< katex >}}\phi^C{{< /katex >}}, the chymist's rating in chymistry,
- {{< katex >}}\Sigma^{^T_R}{{< /katex >}}, the steps of time reduction the chymist has chosen to
  take,
- {{< katex >}}\lambda{{< /katex >}}, whether or not the chymist has reliable access to an
  appropriate laboratory for research,
- and {{< katex >}}\Mu{{< /katex >}}, whether or not the chymist is using reference materials for
  preparation.

##### {{< katex >}}\Delta_u{{< /katex >}} (Universal Modifier)

{{< katex display >}}
\Delta_u(\mu, \phi^C, \Sigma^{^T_R}) =
\Sigma^{^T_R} +
\bigl( \thinspace \mu \gt \phi^C_T \to \mu - \phi^C_T \thinspace \bigr)
{{< /katex >}}

The input variables are:

- {{< katex >}}\mu{{< /katex >}}, the magnitude of the formula being researched or prepared
- {{< katex >}}\phi^C{{< /katex >}}, the chymist's rating in chymistry,
- and {{< katex >}}\Sigma^{^T_R}{{< /katex >}}, the number of steps of time reduction the chymist is taking.

To determine the universal modifier, first note the number of steps of time reduction the chymist is
taking. The modifier scales linearly with the steps of time reduction. Next, compare the magnitude
of the formula being prepared or researched to the tier of the chymist's rating in chymistry. If the
magnitude exceeds the tier ({{< katex >}}\mu > \phi^C_T{{< /katex >}}), the modifier increases by the
difference of the magnitude and tier ({{< katex >}}\mu - \phi^C_T{{< /katex >}}).

Consider the following examples for a chymist with a rating of 42 in chymistry:

- They are attempting to research a magnitude 3 formula with 1 step of time reduction.

  {{< katex display >}}
    \begin{aligned}
      \mu &:= 3
      \\
      \phi^C &:= 4_2
      \\
      \Sigma^{^T_R} &:= 1
      \\
      \Delta_u(\mu, \phi^C, \Sigma^{^T_R}) &=
      \Sigma^{^T_R} +
      \bigl( \thinspace \mu \gt \phi^C_T \to \mu - \phi^C_T \thinspace \bigr)
      \\
      \Delta_u(3, 4_2, 1) &=
      1 +
      \underbrace{
         \bigl( \thinspace 3 \gt 4 \to 3 - 4 \thinspace \bigr)
      }_{\text{A rating of }4_2\text{ has a T of }4}
      \\
      \Delta_u(3, 4_2, 1) &= 1 + 0
      \\
      \Delta_u &= 1
    \end{aligned}
  {{< /katex >}}

  The value of {{< katex >}}\Delta_u{{< /katex >}} is 1. This value will be substituted into the
  general equation for difficulty.

- They are attempting to prepare a magnitude 6 formula with 2 steps of time reduction.

  {{< katex display >}}
    \begin{aligned}
      \mu &:= 6
      \\
      \phi^C &:= 4_2
      \\
      \Sigma^{^T_R} &:= 2
      \\
      \Delta_u(\mu, \phi^C, \Sigma^{^T_R}) &=
      \Sigma^{^T_R} +
      \bigl( \thinspace \mu \gt \phi^C_T \to \mu - \phi^C_T \thinspace \bigr)
      \\
      \Delta_u(6, 4_2, 2) &=
      2 +
      \bigl( \thinspace 6 \gt 4 \to 6 - 4 \thinspace \bigr)
      \\
      \Delta_u(6, 4_2, 2) &= 2 + 2
      \\
      \Delta_u &= 4
    \end{aligned}
  {{< /katex >}}

  The value of {{< katex >}}\Delta_u{{< /katex >}} is 4. This value will be substituted into the
  general equation for difficulty.

##### {{< katex >}}\Delta_r{{< /katex >}} (Research Modifier)

{{< katex display >}}
\Delta_r = \nexists \lambda \to 1
{{< /katex >}}

To determine the research modifier, you need to know if the chymist has reliable access to an
appropriate laboratory ({{< katex >}}\lambda{{< /katex >}}) for their work. If they do not
({{< katex>}}\nexists \lambda{{< /katex >}}), the modifier is 1. Otherwise, it is 0.

##### {{< katex >}}\Delta_p{{< /katex >}} (Preparation Modifier)

{{< katex display >}}
\Delta_p(f^R, f^T, \Mu, \phi^f) =
\begin{pmatrix}
   \begin{aligned}
      &\bigl(
         \thinspace f^R_{\iota} \setminus f^T_{\iota} \thinspace
      \bigr)
      \\
      +
      &\bigl(
         \thinspace f^R_{\mu} \ne f^T_{\mu} \to \vert f^R_{\mu} - f^T_{\mu} \vert \thinspace
      \bigr)
      \\
      +
      &\begin{cases}
         1 &\text{if } \nexists{\Mu} \\
         ^-\phi^M_T &\text{if } \exists{\Mu} \And \exists{\phi^f} \\
      \end{cases}
   \end{aligned}
\end{pmatrix}
\centerdot
\begin{cases}
   1 &\text{if } f^R_{\pi} \equiv f^T_{\pi} \\
   2 &\text{if } f^R_{\pi} \ne f^T_{\pi} \\
\end{cases}
{{< /katex >}}

The input variables are:

- {{< katex >}}f^R{{< /katex >}}, the reference formula--the formula as memorized and/or referenced from materials,
- {{< katex >}}f^T{{< /katex >}}, the test formula--the formula actually being prepared,
- {{< katex >}}\Mu {{< /katex >}}, whether or not the chymist is using reference materials,
- and {{< katex >}}\phi^f{{< /katex >}}, the chymist's rating in the formula, if any.

First, compare the ingredient list of the reference and test formulae
({{< katex >}} f^R_{\iota} \setminus f^T_{\iota}{{< /katex >}}). The modifier increases for every
substituted ingredient. Consider these example formulae:

{{< katex display >}}
\begin{aligned}
   f^R_{\iota} &:= \lbrace
      \footnotesize
      Activated \text{\thickspace} Charcoal, \text{\thickspace}
      Child\text{\textquoteright} s \text{\thickspace} Drawing, \text{\thickspace}
      Galena
   \rbrace
   \\
   f^T_{\iota} &:= \lbrace
      \footnotesize
      Gascon \text{\thickspace} Saliva, \text{\thickspace}
      Child\text{\textquoteright} s \text{\thickspace} Drawing, \text{\thickspace}
      Lemon
   \rbrace
\end{aligned}
{{< /katex >}}

Because {{< katex >}}f^T_{\iota}{{< /katex >}} differs from {{< katex >}}f^R_{\iota}{{< /katex >}} by two ingredients, the value of this subexpression is 2.

Next, compare the magnitude of the reference formula, {{< katex >}}f^R_{\mu}{{< /katex >}}, to the magnitude of the test formula, {{< katex >}}f^T_{\mu}{{< /katex >}}. If they are not equal ({{< katex >}}f^R_{\mu} \ne f^T_{\mu}{{< /katex >}}), then the modifier increases linearly with the difference in their values ({{< katex >}}\vert f^R_{\mu} - f^T_{\mu} \vert{{< /katex >}}). Consider these examples:

- The reference formula and the test formula have the same magnitude.

  {{< katex display >}}
  \begin{aligned}
  f^R_{\mu} &:= 2 \\
  f^T_{\mu} &:= 2 \\
  f^R_{\mu} \ne f^T_{\mu} &\to \vert f^R_{\mu} - f^T_{\mu} \vert \\
  2 \ne 2 &\to \vert f^R_{\mu} - f^T_{\mu} \vert \\
  &\thickspace\thickspace 0
  \end{aligned}
  {{< /katex >}}

  Because the values are equal, the comparison is not true and the subtraction operation never needs
  to be called. While this is _nominally_ identical to having no conditional, it is often easier for novice chymists to compare the values before thinking about subtraction.
- The reference formula has a greater magnitude than the test formula.

  {{< katex display >}}
  \begin{aligned}
  f^R_{\mu} &:= 4 \\
  f^T_{\mu} &:= 2 \\
  f^R_{\mu} \ne f^T_{\mu} &\to \vert f^R_{\mu} - f^T_{\mu} \vert \\
  4 \ne 2 &\to \vert f^R_{\mu} - f^T_{\mu} \vert \\
  \vert 4 &- 2 \vert \\
  &\thickspace\thickspace 2
  \end{aligned}
  {{< /katex >}}

  Because the values are unequal, the comparison is true and the subtraction operation is executed,
  yielding 2. In this case, the absolute value was the yielded result and so the modifier increases
  by 2.
- The reference formula has a lesser magnitude than the test formula.

  {{< katex display >}}
  \begin{aligned}
  f^R_{\mu} &:= 1 \\
  f^T_{\mu} &:= 2 \\
  f^R_{\mu} \ne f^T_{\mu} &\to \vert f^R_{\mu} - f^T_{\mu} \vert \\
  1 \ne 2 &\to \vert f^R_{\mu} - f^T_{\mu} \vert \\
  \vert 1 &- 2 \vert \\
  &\thickspace\thickspace 1
  \end{aligned}
  {{< /katex >}}

  Because the values are unequal, the comparison is true and the subtraction operation is executed,
  yielding -1. In this case, the absolute value is 1 and so the modifier increases by 1.

##### Procedural Difficulty

By default, the difficulty of any chymical test is 1. The following contexts modify difficulty:

- If a chymist is preparing or researching a formula at a higher magnitude than the tier of their
  chymistry rating, +1 difficulty for each point of magnitude above their tier.
- If a chymist is preparing or researching a formula more quickly, +1 difficulty per step of time
  reduction.
- If a chymist is researching a formula without an appropriate laboratory, +1 difficulty.
- If a chymist is preparing a formula without reference materials, +1 difficulty.
- If a chymist is preparing a formula with alternate ingredients, +1 difficulty per substitution.
- If a chymist is preparing a formula at a different magnitude than memorized or referenced, +1
  difficulty per difference in magnitude.
- If a chymist is preparing a memorized formula, ignore additional difficulty up to the tier of
  their rating for that formula.
- If a chymist is preparing a memorized formula with reference materials, -1 difficulty.
- If a chymist is preparing a formula with an alternate form, double the final difficulty.

For example:

1. If a chymist wants to research a magnitude 1 formula one step faster (+1 difficulty) and
   without an appropriate laboratory (+1 difficulty), the difficulty for the test is 3. Any roll of
   26 or lower fails regardless of other factors.
2. For a chymist with a rating of 24 in a memorized formula:
   1. If they prepare that memorized formula with reference materials (-1 difficulty), they do not
      need to test to prepare the formula as the difficulty is 0.
   2. They could increase the magnitude of the formula by 1 and substitute an ingredient without
      incurring a difficulty penalty because the tier of their memorized formula rating is 2. With
      reference materials, they would not need to test to prepare the formula. Without reference
      materials, the test would be difficulty 1.
   3. Any additional difficulty-incurring contexts would increase the difficulty of the test as
      normal. So if they increased the magnitude by 2 and substituted 2 ingredients, the difficulty
      without reference materials would be 3. With reference materials (-1 difficulty), the
      difficulty would be 2.

#### Results

Pass
: The chymist achieved whatever they attempted.

Fail
: The chymist was unsuccessful and must live with the usual consequences.

Triumph
: The chymist achieved the best possible outcome for whatever they attempted.

Botch
: The chymist made a terrible mistake and must endure the worst possible outcome for their failure.

#### Examples

Consider the following example contexts and how the tests might proceed. Each numbered item beneath
a context is a different possible result. In this example, the Chymist has a rating of 23 for
chymistry, their highest-rated quality is at 21, and the formula they are preparing is one they
memorized at a rating of 14.

The chymist is preparing their memorized formula without reference materials and with a substitute
ingredient. The difficulty is 2 (the tier of their memorized formula is 1, allowing them to ignore
the +1 difficulty modifier of preparing a formula without reference materials, but the +1 difficulty
modifier of using a substitute ingredient still applies). Consider the following results when they
roll a d66 for the test:

1. The result is a 16. This is under the difficulty. They fail.
2. The result is a 21. This is equal to the difficulty and under their chymistry rating. They pass.
3. The result is a 23. This is equal to the difficulty and their chymistry rating. They triumph.
4. The result is a 34. This is over the difficulty as well as their chymistry and quality ratings.
   The degree of the result (4) is not lower than the tier of their quality (2). They fail.
5. The result is a 41. This is over the difficulty as well as their chymistry and quality ratings.
   The degree of the result (1) is lower than the tier of their quality. They pass.
6. The result is a 66. They botch.

## Formulae

A formula is the defined process for converting material ingredients into an effect on reality.
Every formula is constituted by its effect, qualities, magnitude, ingredients, form, and
predictability.

### Effects

The effect of a chymical formula is the way it alters reality when consumed. Effects are limited only by the inventiveness and acumen of the chymist.

Some well-known examples include:

- Transforming flesh to stone
- Granting the ability to see thermal signatures
- Making an entity weightless
- Turning breath to flame
- Defoliation
- Linking minds

### Magnitude

All formulae are rated by their magnitude, the approximation of their power for altering reality,
rated from 1-6. The higher a formula's magnitude, the more powerful its effect.

Formulae of a higher magnitude are more complex, arduous to research, and take more time to prepare.

The tier of a chymist's rating in chymistry is a limiting factor for the magnitude of formula they
are capable of researching and preparing. If the magnitude of the formula is greater than the tier
of the chymistry rating, the difference is added to the difficulty for the test.

### Qualities

### Ingredients

### Forms

### Predictability

## Preparing Formulae

To prepare a formula, a chymist must either have the formula memorized or be working from reference
materials, have the appropriate ingredients, and take the time to follow the specific process for
that formula.

If a chymist is preparing a memorized formula, they may ignore difficulty penalties up to the tier
of their rating for the memorized formula. If a chymist is preparing a memorized formula with
reference materials, -1 difficulty.

By default, preparing a formula takes as many hours as its magnitude. A chymist can prepare a
formula more quickly at the danger of increased difficulty (+1 per step):

1. 30 minutes per magnitude
2. 5 minutes per magnitude
3. 1 minute per magnitude
4. 1 moment per magnitude

When a chymist alters a memorized or referenced formula when preparing it, they are executing
dynamic research. The process is subject to mishaps and the delay, duration, and batch size are all
determined by the result. For more information, see [Researching Formulae](research.md).

The following alterations all constitute dynamic research and modify the difficulty of the test:

- +1 difficulty to alter the predictability, if permitted by its form
- +1 difficulty per substitution if using any alternate ingredients
- Double difficulty to alter the form

Every time a chymist passes a test to prepare a formula, mark up to one per difficulty of the test:

- The chymistry rating
- A relevant rated quality
- The formula's rating (if memorized)

Each rating may only ever have one mark at a time. The next time the chymist has downtime, defined
as at least one week of rest and safety without pressing concerns, they may clear each mark by
rolling a d66. The result relative to the rating and the rating's category determine the effect:

| Category  | Result              | Rating Increase |
| :-------: | :------------------ | :-------------: |
| Chymistry | Equal to the rating |       +2        |
| Chymistry | Above the rating    |       +1        |
|  Formula  | Below the rating    |       +1        |
|  Formula  | Equal to the rating |       +4        |
|  Formula  | Above the rating    |       +2        |
|  Quality  | Equal to the rating |       +4        |
|  Quality  | Above the rating    |       +2        |


### Magnitude

Magnitude is the rough _potency_ of a chymical formula; if there are any mechanical effects, tie
them to the magnitude. Here are a few examples of effects and how their magnitude might be used:

1. A cap of incense which causes anyone who inhales it to share thoughts might allow them to share
   magnitude words at a time, or send increasingly complex thoughts (words at magnitude 1, voice at
   magnitude 2, audio-visual at magnitude 3, etc).
1. A potion which fills the imbibers hands with throwable lightning might allow them to throw a
   number of lightning bolts each minute up to the magnitude, or have each bolt deal magnitude d6
   damage, or stun targets for magnitude rounds.
1. A pill which inures the swallower against magic might last for magnitude effects or disperse any
   incoming magic of a lower magnitude.
1. A powder which increases the reaction time of the snorter might give them an additional magnitude
   actions per round, increase their reflex saves by the magnitude, or provide a bonus equal to the
   magnitude on initiative checks.
1. A salve which turns the underlying flesh to stone might provide a bonus to AC equal to magnitude,
   add magnitude d6 temporary hit points, or be used to block magnitude attacks before breaking.
1. A wafer which causes the eater to grow wings might enable them to fly magnitude rounds at a time,
   or fly faster, or only glide at magnitude 1 but soar with perfect control at magnitude 6.

As always, use your best judgement and do what works for your table and play.

### Preparing Formulae with Alternate Ingredients

Sometimes, it might be necessary to attempt to prepare a known formula with different ingredients.
Each substituted ingredient increases the difficulty tier by one.

Using _any_ substitutions counts as on-the-fly research; the process is subject to mishaps and the
delay, duration, and batch size are all determined by the result. For more information, see the
section on [Researching Formulae](research).
