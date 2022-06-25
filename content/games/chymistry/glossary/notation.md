---
title: Notation
description: |
  Defines the marks, signs, figures, and symbols used to represent the system of chymistry.
weight: 20
---

This text includes numerous equations with special marks, signs, figures, and symbols. Although they
are fully defined and explicated in-line where they are used, but this section includes overviews
for them.

### Dice Notation

{{< katex >}}d{{< /katex >}}
: Read as "die" or "dice."

{{< katex >}}ndy{{< /katex >}}
: Read as "x y-sided dice."

  For example:

  - Read {{< katex >}}\footnotesize 1d6{{< /katex >}} as "one six-sided die."
  - Read {{< katex >}}\footnotesize 3d8{{< /katex >}} as "three eight-sided dice."

{{< katex >}}xdy{\uparrow}z{{< /katex >}}
: Read as "x y-sided dice, exploding on results of z or higher." If
  {{< katex >}}z{{< /katex >}} is omitted, it is equal to {{< katex >}}y{{< /katex >}}.

  For example:

  - Read {{< katex >}}\footnotesize 1d6{\uparrow}{{< /katex >}} as one six-sided die, exploding
    on results of 6.
  - Read {{< katex >}}\footnotesize 1d6{\uparrow}6{{< /katex >}} as one six-sided die, exploding
    on results of 6.
  - Read {{< katex >}}\footnotesize 3d6{\uparrow}4{{< /katex >}} as three six-sided dice,
    exploding on results of 4 or higher.

{{< katex >}}xdy{\upuparrows}z{{< /katex >}}
: Read as "x y-sided dice, chain-exploding on results of z or higher." If
  {{< katex >}}z{{< /katex >}} is omitted, it is equal to {{< katex >}}y{{< /katex >}}.

  For example:

  - Read {{< katex >}}\footnotesize 1d6{\upuparrows}{{< /katex >}} as one six-sided die,
    chain-exploding on results of 6.
  - Read {{< katex >}}\footnotesize 1d6{\upuparrows}6{{< /katex >}} as one six-sided die,
    chain-exploding on results of 6.
  - Read {{< katex >}}\footnotesize 3d6{\upuparrows}4{{< /katex >}} as three six-sided dice,
    chain-exploding on results of 4 or higher.

{{< katex >}}d6_6{{< /katex >}}
: Read as "the test dice."

  To roll the test dice, roll of two six-sided dice, one for the tier and one for the degree.
  Interpret the rolls as a rating.

  To distinguish between the tier die and the degree die when rolling test dice, consider:

  - If using visually distinct dice, select one die as the tier die and the other as the degree die.
  - If using identical dice, then use the nearest die to the chymist after rolling (or furthest left
    if they are equidistant) as the tier die and the other as the degree die.
  - If using only one die, use the first roll as the tier die and the second as the degree die.

  For the representation of the result of rolling {{< katex >}}d6_6{{< /katex >}}, see...
{ .dt-10 }

### General Notation

{{< katex >}}x_y{{< /katex>}}
: Read as "rated at a tier of {{< katex >}}x{{< /katex>}} with a degree of
  {{< katex >}}y{{< /katex>}}."

  For example, read {{< katex >}}4_2{{< /katex >}} as "rated at a tier
  of 4 with a degree of 2."

{{< katex >}}\lnot{{< /katex >}}
: Read as "not."

  This term is always used with another, where it negates the term that follows it. It is used
  with boolean variables (that is, terms whose value can be either true or false) to indicate that
  the value is false for a conditional expression.

{{< katex >}}
\begin{cases}
  Q_1 & P_1 \\
  Q_2 & P_2 \\
  Q_{...} & P_{...} \\
  Q_n & \text{otherwise}
\end{cases}
{{< /katex >}}
: This expression is called a branching statement and is read as "If {{< katex >}}P_1{{< /katex >}}
  then the value is {{< katex >}}Q_1{{< /katex >}}, else if {{< katex >}}P_2{{< /katex >}} then the
  value is {{< katex >}}Q_2{{< /katex >}}, else if ..., otherwise the value is
  {{< katex >}}Q_n{{< /katex >}}."

  Each line represents an antecedent-consequent pair in branching logic for the equation.

  The antecedents {{< katex >}}P{{< /katex >}} may be terms by themselves or conditional
  expressions evaluating one or more terms. When a term is specified on its own as an antecedent,
  it is implied that the term is being evaluated for truthiness.

  The consequents {{< katex >}}Q{{< /katex >}} may be numerals, terms, or expressions.

  This notation is a way to express branching conditional behavior in an equation. Branch statements
  must always define their antecedent-consequent pairs such that there is a branch for all
  possibilities and the consequent is never indeterminate when the referenced variables are known.

  Consider the following examples:

  1. {{< katex >}}
     \begin{cases}
       25 & x \ge 10 \\
       2x & 0 \lt x \lt 10 \\
       0 & \text{otherwise}
     \end{cases}
     {{< /katex >}}

     Read this branching statement as "if {{< katex >}}x{{< /katex >}} is greater than or equal to
     10 then the value is 25, else if {{< katex >}}x{{< /katex >}} is greater than 0 and less than
     10 then the value is two times {{< katex >}}x{{< /katex >}}, otherwise the value is 0."

     When {{< katex >}}x{{< /katex >}} is 17 then the value is 25.

     When {{< katex >}}x{{< /katex >}} is 3 then the value is 6.

     When {{< katex >}}x{{< /katex >}} is 0 then the value is 0.
  2. {{< katex >}}
     \begin{cases}
       1 & x \\
       0 & \text{otherwise}
     \end{cases}
     {{< /katex >}}

     Read this branching statement as "if {{< katex >}}x{{< /katex >}} is true then the value is 1,
     otherwise the value is 0." This branching statement is also identical to the inference
     statement {{< katex >}}x \to 1{{< /katex >}} which can be simpler to use in a complex equation.

{{< katex >}} P \to Q {{< /katex >}}
: This expression is called an inference statement and is read as "if {{< katex >}}P{{< /katex >}}
  then the value is {{< katex >}}Q{{< /katex >}}, otherwise the value is 0."

  The antecedent {{< katex >}}P{{< /katex >}} may be a term by itself or a conditional expression
  evaluating one or more terms. When a term is specified on its own as an antecedent, it is implied
  that the term is being evaluated for truthiness.

  The consequent {{< katex >}}Q{{< /katex >}} may be a numeral, term, or expression.

  Consider the following examples:

  1. If {{< katex >}}\Omega{{< /katex >}} means "the sun is up", read
     {{< katex >}}\Omega \to 1{{< /katex >}} as "if the sun is up then the value is 1, otherwise the
     value is 0."
  2. Read {{< katex >}}x \gt 0 \to 10{{< /katex >}} as "if {{< katex >}}x{{< /katex >}} is greater
     than 0 then the value is 10, otherwise the value is 0."
{ .dt-20 }

### Chymical Notation

{{< katex >}}\Phi{{< /katex >}}
: Read as "rating."

  The finite set of possible ratings, {{< katex >}}\Phi{{< /katex >}}, is defined as:

  {{< katex display >}}
  \Phi = \begin{Bmatrix}
  1_1 & 1_2 & 1_3 & 1_4 & 1_5 & 1_6 \\
  2_1 & 2_2 & 2_3 & 2_4 & 2_5 & 2_6 \\
  3_1 & 3_2 & 3_3 & 3_4 & 3_5 & 3_6 \\
  4_1 & 4_2 & 4_3 & 4_4 & 4_5 & 4_6 \\
  5_1 & 5_2 & 5_3 & 5_4 & 5_5 & 5_6 \\
  6_1 & 6_2 & 6_3 & 6_4 & 6_5 & 6_6 \\
  \end{Bmatrix}
  {{< /katex >}}

{{< katex >}}\phi{{< /katex >}}
: Read as "the chymist's rating in..."

  {{< katex >}}\phi{{< /katex >}} is always specified with a superscript defining the type of
  rating:

  {{< katex >}}\phi^C{{< /katex >}}
  : Read as "the chymist's rating in chymistry."

  {{< katex >}}\phi^f{{< /katex >}}
  : Read as "the chymist's rating in the formula."

  {{< katex >}}\phi^Q{{< /katex >}}
  : Read as "the chymist's rating in the quality."

  {{< katex >}}\phi^R{{< /katex >}}
  : Read as "the chymist's rating in the result of the test."
  { .dt-5 }

  When the value of a rating's tier or degree is required for an equation, the notation is extended
  with a subscript:

  {{< katex >}}\phi^C_T{{< /katex >}}
  : Read as "the tier of the chymist's rating in chymistry."

  {{< katex >}}\phi^C_D{{< /katex >}}
  : Read as "the degree of the chymist's rating in chymistry."

  {{< katex >}}\phi^Q_T{{< /katex >}}
  : Read as "the tier of the chymist's rating in the quality."

  {{< katex >}}\phi^Q_D{{< /katex >}}
  : Read as "the degree of the chymist's rating in the quality."

  {{< katex >}}\phi^f_T{{< /katex >}}
  : Read as "the tier of the chymist's rating in the formula."

  {{< katex >}}\phi^f_D{{< /katex >}}
  : Read as "the degree of the chymist's rating in the formula."
  { .dt-5 }


{{< katex >}}\mu{{< /katex >}}
: Read as "magnitude."

  {{< katex >}}\mu{{< /katex >}} is sometimes used on its own as when the source of the magnitude is
  clear in the context or as subscript when attached to a specific formula
  (i.e.{{< katex >}}f_{\mu}{{< /katex >}}).

{{< katex >}}f{{< /katex >}}
: Read as "the formula."

  The subscript of {{< katex >}}f{{< /katex >}} denotes the particular component of the formula
  being referenced:

  {{< katex >}}f_{\iota}{{< /katex >}}
  : The formula's set of ingredients.

  {{< katex >}}f_{\pi}{{< /katex >}}
  : The formula's set of qualities.

  {{< katex >}}f_{\mu}{{< /katex >}}
  : The formula's magnitude.

  {{< katex >}}f_{\beta}{{< /katex >}}
  : The formula's form.
  { .dt-5 }

  When more than one formula is referenced in an equation, they are distinguished with a prefixed
  superscript identifying them.

  For example, in the equation for determining the preparation modifier, the term
  {{< katex >}}^Rf{{< /katex >}} is read as "the reference formula."
{ .dt-5 }

### Specific Notation

{{< katex >}}\delta{{< /katex >}}
: Read as "difficulty tier."

  The following terms are specific to the difficulty tier equation and its modifier equations in the
  order they are used:

  {{< katex >}}\Pi{{< /katex >}}
  : Read as "the purpose of the test."

    The value of this term is always either researching or preparing.

  {{< katex >}}f^T{{< /katex >}}
  : Read as "the test formula."

    This value is never null.

  {{< katex >}}f^R{{< /katex >}}
  : Read as "the reference formula."

    This value is null when researching a formula because there the purpose of research is to
    discover a reference formula. When preparing a formula, {{< katex >}}f^R{{< /katex >}} may be
    identical to {{< katex >}}f^T{{< /katex >}} (when the chymist is preparing the formula
    exactly as defined) or differ, as when substituting ingredients, adjusting the magnitude, or
    preparing an alternate form.

  {{< katex >}}t{{< /katex >}}
  : Read as "the count of the steps of time reduction."

    {{< katex >}}\displaystyle \sum_{n=0}^{t}n{{< /katex >}}
    : Read as "the sum of the count of the steps of time reduction."

      This notation sums each step of the time reducion the chymist is taking for a given test. For
      example, if the chymist is reducing the time to prepare a formula by three steps, this
      notation expands out as:

      {{< katex >}}
      \begin{aligned}
      \sum_{n=0}^{t}n &= n_1 + n_2 + ... + n_t \\
      \\
      \sum_{n=0}^{3}n &= 1 + 2 + 3 \\
      \\
      \sum_{n=0}^{3}n &= 6 \\
      \end{aligned}
      {{< /katex>}}

  {{< katex >}}\lambda{{< /katex >}}
  : Read as "the chymist has reliable access to an appropriate laboratory."

    If prefixed with a {{< katex >}}\lnot{{< /katex >}}, read as "the chymist does not have reliable
    access to an appropriate laboratory."

  {{< katex >}}\rho{{< /katex >}}
  : Read as "the chymist is using reference materials to prepare the formula."

    If prefixed with a {{< katex >}}\lnot{{< /katex >}}, read as "the chymist is not using reference
    materials to prepare the formula."

  {{< katex >}}\Delta{{< /katex >}}
  : Read as "the modifier."

    The subscript of {{< katex >}}\Delta{{< /katex >}} denotes the particular modifier being
    referenced.

  {{< katex >}}\Delta_u{{< /katex >}}
  : Read as "the universal modifier."

    Determined by the formula:

    {{< katex display >}}
    \Delta_u(
      \mu, \thickspace
      \phi^C, \thickspace
      t
    ) = \sum_{n=0}^{t}n + \bigl(
      \thinspace \mu \gt \phi^C_T \to \mu - \phi^C_T \thinspace
    \bigr)
    {{< /katex >}}

    Which reads as:

    > Given the magnitude, the chymist's rating in chymistry, and count of the steps of time
    > reduction, the universal modifier is equal to the sum of the steps of time reduction plus
    > either the difference between the magnitude and the tier of the chymist's rating in chymistry
    > (if the magnitude is greater than the tier) or 0.

  {{< katex >}}\Delta_r{{< /katex >}}
  : Read as "the research modifier."

    Determined by the formula:

    {{< katex display >}}
    \Delta_r(\lambda) = \lnot \lambda \to 1
    {{< /katex >}}

    Which reads as:

    > Given whether or not the chymist has reliable access to an appropriate laboratory, the
    > research modifier is equal to 1 if the chymist does not have reliable access to an appropriate
    > laboratory, otherwise 0.

  {{< katex >}}\Delta_p{{< /katex >}}
  : Read as "the preparation modifier."

    Determined by the formula:

    {{< katex display >}}
    \Delta_p(f^R, f^T, \rho, \phi^f) =
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
            1 &  \lnot{\rho} \\
            ^-\phi^f_T & \rho \And \phi^f \\
          \end{cases}
      \end{aligned}
    \end{pmatrix}
    \centerdot
    \begin{cases}
      1 &\text{if } f^R_{\pi} \equiv f^T_{\pi} \\
      2 &\text{if } f^R_{\pi} \ne f^T_{\pi} \\
    \end{cases}
    {{< /katex >}}

    Which reads as:

    > Given the reference formula, the test formula, whether or not the chymist is using reference
    > materials to prepare the formula, and the chymist's rating in the reference formula, the
    > preparation modifier is equal to the sum of the set difference of the ingredients of the
    > reference formula and the ingredients of the test formula plus either the absolute difference
    > between the magnitude of the reference formula and the test formula if those magnitudes are
    > unequal or 0 if they are equal, plus 1 if the chymist is not using reference materials, or
    > minus the tier of the chymist's rating in the formula if the chymist is using reference
    > materials and has a rating in the formula, times 2 if the form of the reference formula is not
    > the same as the form of the test formula.
