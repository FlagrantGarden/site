---
title: Testing
description: |
  On the general process for testing a chymist's competency.
weight: 20
---

In the practice of chymistry, it is often necessary to test our competency. Any time we attempt to
prepare or research a formula, we are testing our expertise against the art itself, so it is
critical that we examine this process in some detail.

# The Test Dice

The mechanisms in this text rely on rolling dice to generate a rating for a test. The notation
{{< katex >}}d6_6{{< /katex >}} is used as shorthand for "the test dice." To roll the test dice,
roll of two six-sided dice, one for the tier and one for the degree. Interpret the rolls as a
rating.

To distinguish between the tier die and the degree die when rolling test dice, consider:

- If using visually distinct dice, select one die as the tier die and the other as the degree die.
- If using identical dice, then use the nearest die to the chymist after rolling (or furthest left
  if they are equidistant) as the tier die and the other as the degree die.
- If using only one die, use the first roll as the tier die and the second as the degree die.

# Test Results

There are four possible outcomes of a test, listed here from best to worst:

Triumph
: The best possible outcome for a test. The chymist has demonstrated competency at the literal edge
  of their capabilities and it shows in the results.

Pass
: The chymist has succeeded in their test. They have prepared or researched the formula as intended.

Fail
: The chymist has made too many mistakes and their efforts are thwarted. Depending on the context,
  they might have merely wasted time and materials or they might be in danger of a chymical mishap.

Botch
: The chymist has made what may well be a fatal error. They have wasted time and materials and are
  subject to dangerous chymical mishaps.

# The Test Definition

The general process for evaluating a chymical test can be defined by this equation:

{{< katex display >}}
\begin{aligned}
  \phi^R &:= d6_6 \\
  R &=
  \begin{cases}
    R_P & \enspace \delta \lt 1 \\
    R_F & \enspace \delta \gt 6 \\
    R_F & \enspace \phi^R_T \lt \delta \\
    R_B & \enspace \phi^R \equiv 6_6 \\
    R_P & \enspace (\phi^R \lt \phi^C) \lor (\phi^R \lt \phi^E) \\
    R_T & \enspace (\phi^R \equiv \phi^C) \lor (\phi^R \equiv \phi^E) \\
    R_P & \bigl((\phi^R \gt \phi^C) \land (\phi^R \gt \phi^E)\bigr) \land (\phi^R_D \lt \phi^E_T) \\
    R_F & \text{otherwise}
  \end{cases}
\end{aligned}
{{< /katex >}}

For new chymists, this may be a little daunting, but with inspection and explication we can make
things clear. For the rest of this section, we will step through the equation, defining the notation
and expressions.

We read the first line {{< katex >}}(\phi^R := d6_6){{< /katex >}} as "let the rating of the
chymist's demonstrated expertise be defined by rolling the test dice."

Next, we determine the result ({{< katex >}}R{{< /katex >}}) by examining several cases. The
notation {{< katex >}}\scriptsize\begin{cases}\thinspace&\end{cases}{{< /katex >}} denotes a
branching statement.

Each line in the branching statement represents a different possible outcome, called a case. The
first term is the result, the expression to the right is called a conditional. If the conditional is
true, then that case of the branching statement is used as the value for the result.

{{< katex >}} R_P \quad \delta \lt 1 {{< /katex >}}
: We read this case of the branching statement as "the test is passed if the difficulty tier is less
  than 1" where {{< katex >}}R_P{{< /katex >}} represents a passing result,
  {{< katex >}}\delta{{< /katex >}} represents the difficulty tier, and
  {{< katex >}}\lt{{< /katex >}} is a symbol meaning "true if the value to the left is less than the
  value to the right."

  We examine the difficulty tier and how to determine it later in this text.

{{< katex >}} R_F \quad \phi^R_T \lt \delta {{< /katex >}}
: We read this case of the branching statement as "the test is failed if the tier of the result's
  rating is less than the difficulty tier" where {{< katex >}}\phi^R_T{{< /katex >}} denotes the
  tier of the result of rolling the test dice.

{{< katex >}} R_B \quad \phi^R \equiv 6_6 {{< /katex >}}
: We read this case of the branching statement as "the test is botched if the result is rated at a
  tier of 6 with a degree of 6," i.e. if the face-values of the test dice are both 6.

{{< katex >}} R_P \quad (\phi^R \lt \phi^C) \lor (\phi^R \lt \phi^E) {{< /katex >}}
: We read this case of the branching statement as "the test is passed if the result's rating is
  less than the chymist's rating in chymistry or their highest relevant expertise." We will expand
  on {{< katex >}}\phi^E{{< /katex >}} in the [Procedure](#procedure) section, but for now just know
  that this could be the chymist's rating in a quality or a particular formula.

{{< katex >}} R_T \quad (\phi^R \equiv \phi^C) \lor (\phi^R \equiv \phi^E) {{< /katex >}}
: We read this case of the branching statement as "the test is triumphed if the result's rating is
  equivalent to either the chymist's rating in chymistry or their highest relevant expertise."

{{< katex >}} R_P \quad \bigl((\phi^R \gt \phi^C) \land (\phi^R \gt \phi^E)\bigr) \land (\phi^R_D \lt \phi^E_T) {{< /katex >}}
: We read this case of the branching statement as "the test is passed if the result's rating is greater than both the chymist's rating in chymistry and their highest relevant expertise and the degree of the result is less than the tier of their expertise rating."

{{< katex >}} R_F \quad \text{otherwise} {{< /katex >}}
: We read this case of the branching statement as "the test is failed otherwise."
{ .dt-flat }

## Example Test Results

Let us consider a few examples to see how this branching statement behaves. Each example begins with the relevant values needed to determine the final result: the difficulty tier ({{< katex >}}\delta{{< /katex >}}), the rating of our demonstratedd expertise ({{< katex >}}\phi^R{{< /katex >}}), our rating in chymistry ({{< katex >}}\phi^C{{< /katex >}}), and our expertise rating (({{< katex >}}\phi^E{{< /katex >}})). If {{< katex >}}\phi^E{{< /katex >}} is {{< katex >}}\text{\O}{{< /katex >}}, it is null - we do not have a relevant expertise rating to use for the test.

In our notation {{< katex >}}:={{< /katex >}} means "let the term to the left be defined as the value to the right." So when we read {{< katex >}}\delta := 3{{< /katex >}} we should interpret that as "let the difficulty tier be defined as 3."

Similarly, in our notation {{< katex >}}\bot{{< /katex >}} means "the conditional expression evaluated to false" while {{< katex >}}\top{{< /katex >}} means "the conditional expression evaluated to true." This is particularly important in the later cases, which are complex conditionals and use the {{< katex >}}\lor{{< /katex >}} ("if either the expression to the left or right is true, then this condition is true") and {{< katex >}}\land{{< /katex >}} ("if both the expression on the left _and_ the right is true, then this condition is true") symbols. For those complex conditionals, the examples will determine the truthiness of each subexpression before moving on.

In these examples, when we see {{< katex>}}\bot{{< /katex >}}, we should understand that the case we are examining did not return the final result and we must examine the next case in the statement.

{{< details "**Example Case 1: When the Difficulty Tier is Less Than 1**" >}}
{{< katex display >}}
\begin{matrix}
  \delta := 0   & \qquad
  \phi^R := 6_5 & \qquad
  \phi^C := 3_2 & \qquad
  \phi^E := 2_6
\end{matrix}
{{< /katex >}}

In this example, the only term we ever _need_ to examine is the difficulty tier, because the very first case statement (remember, we always check the case statements in the order they are defined) returns a final result:

{{< katex display>}}
\begin{aligned}
R_P & \enspace \delta \lt 1 \\
R_P & \enspace 0 \lt 1 \\
R_P & \enspace \top \\
&R_P \\
\end{aligned}
{{< /katex >}}

Because the difficulty tier is 0, which is less than 1, we automatically pass the test.

> Note that although we defined the other terms here, the rating of our demonstrated expertise is
> null. In practice, we only roll the test dice when we need to, which isn't until the third case
> statement.

{{< /details >}}

{{< details "**Example Case 2: When the Difficulty Tier is  Greater Than 6**" >}}
{{< katex display >}}
\begin{matrix}
  \delta := 6   & \qquad
  \phi^R := 6_5 & \qquad
  \phi^C := 3_2 & \qquad
  \phi^E := 2_6
\end{matrix}
{{< /katex >}}

As always, we examine each case statement in order:

{{< katex display>}}
\begin{aligned}
R_P & \enspace \delta \lt 1 \\
R_P & \enspace 8 \lt 1 \\
&\bot \\
\end{aligned}
{{< /katex >}}

Because the difficulty tier is 8, which is not less than 1, we need to examine the next case:

{{< katex display>}}
\begin{aligned}
R_F & \enspace \delta \gt 6 \\
R_F & \enspace 8 \gt 6 \\
R_F & \enspace \top \\
&R_F \\
\end{aligned}
{{< /katex >}}

Because the dificulty tier is 8, which is greater than 6, we automatically fail the test.

> Note that although we defined the other terms here, the rating of our demonstrated expertise is
> null. In practice, we only roll the test dice when we need to, which isn't until the third case
> statement.

{{< /details >}}

{{< details "**Example Case 3: When We Roll Under the Difficulty Tier**" >}}
{{< katex display >}}
\begin{matrix}
  \delta := 5   & \qquad
  \phi^R := 1_5 & \qquad
  \phi^C := 3_2 & \qquad
  \phi^E := 2_6
\end{matrix}
{{< /katex >}}

As always, we examine each case statement in order:

{{< katex display>}}
\begin{aligned}
R_P & \enspace \delta \lt 1 \\
R_P & \enspace 5 \lt 1 \\
&\bot \\
\end{aligned}
{{< /katex >}}

Because the difficulty tier is 5, which is not less than 1, we need to examine the next case:

{{< katex display>}}
\begin{aligned}
R_F & \enspace \delta \gt 6 \\
R_F & \enspace 5 \gt 6 \\
&\bot \\
\end{aligned}
{{< /katex >}}

Because the dificulty tier is 5, which is not greater than 6, we need to examine the next case:

{{< katex display>}}
\begin{aligned}
R_F & \enspace \phi^R_T \lt \delta \\
R_F & \enspace 1 \lt 5 \\
R_F & \enspace \top \\
&R_F \\
\end{aligned}
{{< /katex >}}

Because the tier of our roll is 1, which is less than the difficulty tier, we failed the test.

> Note that, in practice, it is only when we need to evaluate this case that we roll the test dice;
> until now, merely knowing the difficulty tier has told us whether or not the cases were true or
> false.

{{< /details >}}

{{< details "**Example Case 4: When We Roll a 6<sub>6</sub>**" >}}
{{< katex display >}}
\begin{matrix}
  \delta := 5   & \qquad
  \phi^R := 6_6 & \qquad
  \phi^C := 3_2 & \qquad
  \phi^E := 2_6
\end{matrix}
{{< /katex >}}

As always, we should examine each case statement in order. However, as we have stepped through the first two cases several times and this example (as well as the following ones) focuses on the next unexamined case in the branching statement, we will forego them here. From this example on, we will only examine the named case and the one immediately prior.

With that in mind, the third case:

{{< katex display>}}
\begin{aligned}
R_F & \enspace \phi^R_T \lt \delta \\
R_F & \enspace 6 \lt 5 \\
&\bot \\
\end{aligned}
{{< /katex >}}

Because the tier of our roll is 6, which is not less than the difficulty tier, we need to examine the next case:

{{< katex display>}}
\begin{aligned}
R_B & \enspace \phi^R \equiv 6_6 \\
R_B & \enspace 6_6 \equiv 6_6 \\
R_B & \enspace \top \\
&R_B\\
\end{aligned}
{{< /katex >}}

Because our the rating of our demonstrated competency (determined by rolling the test dice) is 6<sub>6</sub>, we botched the test.

{{< /details >}}

{{< details "**Case 5a: When We Roll Under Our Chymistry Rating Only**" >}}
{{< katex display >}}
\begin{matrix}
  \delta := 1   & \qquad
  \phi^R := 3_1 & \qquad
  \phi^C := 3_2 & \qquad
  \phi^E := \text{\O}
\end{matrix}
{{< /katex >}}

As always, we should examine each case statement in order. For brevity, however, we will start with the fourth case, because we know that the difficulty tier (1) is greater than 0 and less than 6, and that the tier of our roll (3) is not less than the difficulty tier.

{{< katex display>}}
\begin{aligned}
R_B & \enspace \phi^R \equiv 6_6 \\
R_B & \enspace 3_1 \equiv 6_6 \\
&\bot \\
\end{aligned}
{{< /katex >}}

Because our the rating of our demonstrated competency (determined by rolling the test dice) is not 6<sub>6</sub>, we need to examine the next case:

{{< katex display>}}
\begin{aligned}
R_P & \enspace (\phi^R \lt \phi^C) \lor (\phi^R \lt \phi^E) \\
R_P & \enspace (3_1 \lt 3_2) \lor (3_1 \lt \text{\O}) \\
R_P & \enspace \top \lor \bot \\
R_P & \enspace \top \\
&R_P
\end{aligned}
{{< /katex >}}

This is our first complex conditional case, where we pass if the rating of our demonstrated competency is less than either our rating in chymistry or our chosen relevant expertise, if any.

In this case, we did not have a relevant expertise, so we know the subexpression on the right evaluates to false. When we compare our rolled result (3<sub>1</sub>) to our chymistry rating (3<sub>2</sub>), we see that it is less, so the left subexpression evaluates to true.

> In practice, for a logical-or expressions like this where the first subexpression evaluates to
> true, we would not bother to evaluate the next subexpression, because we already know that the
> expression has evaluated to true. We show it here to help us see how reality actually works.

Because the subexpressions are part of a logical-or expression and at least one of them evaluated to true, this case also evaluates to true and we passed the test.

{{< /details >}}

{{< details "**Case 5b: When We Roll Under Our Expertise Rating Only**" >}}
{{< katex display >}}
\begin{matrix}
  \delta := 1   & \qquad
  \phi^R := 3_5 & \qquad
  \phi^C := 3_2 & \qquad
  \phi^E := 4_4
\end{matrix}
{{< /katex >}}

As always, we should examine each case statement in order. For brevity, however, we will start with the fourth case, because we know that the difficulty tier (1) is greater than 0 and less than 6, and that the tier of our roll (3) is not less than the difficulty tier.

{{< katex display>}}
\begin{aligned}
R_B & \enspace \phi^R \equiv 6_6 \\
R_B & \enspace 3_5 \equiv 6_6 \\
&\bot \\
\end{aligned}
{{< /katex >}}

Because our the rating of our demonstrated competency (determined by rolling the test dice) is not 6<sub>6</sub>, we need to examine the next case:

{{< katex display>}}
\begin{aligned}
R_P & \enspace (\phi^R \lt \phi^C) \lor (\phi^R \lt \phi^E) \\
R_P & \enspace (3_5 \lt 3_2) \lor (3_5 \lt 4_4) \\
R_P & \enspace \bot \lor \top \\
R_P & \enspace \top \\
&R_P
\end{aligned}
{{< /katex >}}

Remember from Example Case 5a, we pass if the rating of our demonstrated competency is less than either our rating in chymistry _or_ our chosen relevant expertise.

In this case, when we compare our rolled result (3<sub>5</sub>) to our chymistry rating (3<sub>2</sub>), we see that it is greater, so the left subexpression evaluates to false. When we compare our rolled result to our expertise rating (4<sub>4</sub>), we see that it is less, so the right subexpression evaluates to true.

Because the subexpressions are part of a logical-or expression and at least one of them evaluated to true, this case also evaluates to true and we passed the test.

{{< /details >}}

{{< details "**Case 5c: When We Roll Under Our Both Our Ratings**" >}}
{{< katex display >}}
\begin{matrix}
  \delta := 1   & \qquad
  \phi^R := 2_6 & \qquad
  \phi^C := 3_2 & \qquad
  \phi^E := 4_4
\end{matrix}
{{< /katex >}}

As always, we should examine each case statement in order. For brevity, however, we will start with the fourth case, because we know that the difficulty tier (1) is greater than 0 and less than 6, and that the tier of our roll (2) is not less than the difficulty tier.

{{< katex display>}}
\begin{aligned}
R_B & \enspace \phi^R \equiv 6_6 \\
R_B & \enspace 2_6 \equiv 6_6 \\
&\bot \\
\end{aligned}
{{< /katex >}}

Because our the rating of our demonstrated competency (determined by rolling the test dice) is not 6<sub>6</sub>, we need to examine the next case:

{{< katex display>}}
\begin{aligned}
R_P & \enspace (\phi^R \lt \phi^C) \lor (\phi^R \lt \phi^E) \\
R_P & \enspace (2_6 \lt 3_2) \lor (2_6 \lt 4_4) \\
R_P & \enspace \top \lor \top \\
R_P & \enspace \top \\
&R_P
\end{aligned}
{{< /katex >}}

Remember from Example Case 5a, we pass if the rating of our demonstrated competency is less than either our rating in chymistry _or_ our chosen relevant expertise.

In this case, when we compare our rolled result (2<sub>6</sub>) to our chymistry rating (3<sub>2</sub>), we see that it is less, so the left subexpression evaluates to true. When we compare our rolled result to our expertise rating (4<sub>4</sub>), we see that it is less, so the right subexpression evaluates to true.

Because the subexpressions are part of a logical-or expression and at least one of them evaluated to true, this case also evaluates to true and we passed the test.

{{< /details >}}

{{< details "**Case 6a: When We Roll Equal to Our Chymistry Rating**" >}}
{{< katex display >}}
\begin{matrix}
  \delta := 1   & \qquad
  \phi^R := 3_2 & \qquad
  \phi^C := 3_2 & \qquad
  \phi^E := 4_4
\end{matrix}
{{< /katex >}}

As always, we should examine each case statement in order. For brevity, however, we will start with the fifth case, because we know that the difficulty tier (1) is greater than 0 and less than 6, that the tier of our roll (3) is not less than the difficulty tier, and we did not roll a 6<sub>6</sub>.

{{< katex display>}}
\begin{aligned}
R_P & \enspace (\phi^R \lt \phi^C) \lor (\phi^R \lt \phi^E) \\
R_P & \enspace (3_2 \lt 3_2) \lor (3_2 \lt 4_4) \\
R_P & \enspace \bot \lor \top \\
R_P & \enspace \top \\
&R_P
\end{aligned}
{{< /katex >}}

Remember from Example Case 5a, we pass if the rating of our demonstrated competency is less than either our rating in chymistry _or_ our chosen relevant expertise.

In this case, when we compare our rolled result (2<sub>6</sub>) to our chymistry rating (3<sub>2</sub>), we see that it is less, so the left subexpression evaluates to true. When we compare our rolled result to our expertise rating (4<sub>4</sub>), we see that it is less, so the right subexpression evaluates to true.

Because the subexpressions are part of a logical-or expression and at least one of them evaluated to true, this case also evaluates to true and we passed the test.

{{< /details >}}

# The Test Procedure

Now that we know the equation for testing our expertise, we will examing the procedure for doing so.
When we test our expertise, we always follow this order of operations, stopping at the first step that
returns a result.

1. Note the test formula.
2. Determine the difficulty tier of the test. This is covered in detail in the
   [Difficulty](#difficulty) section.
   1. If the difficulty tier is less than 1, we automatically pass; there is no need to test at all.
   2. If the difficulty tier is greater than 6, we automatically fail; it is impossible for us.
3. Note our chymistry rating.
4. Choose a rating to use for expertise in the test and note it.
   - We can always choose to use any relevant quality we are rated in.
   - If preparing a formula, we can always choose to use our rating in that formula, if we have it.
   - A higher rating for our expertise increases our chance of success, but only our ratings in
     chymistry and the expertise we choose may improve as a result of a test.
   - If we don't have a rating in a relevant quality or the formula, we have no expertise rating for
     this test and it will be much harder to pass.
5. Roll {{< katex >}}d6_6{{< /katex >}} and note the result rating for comparison. Check each of the
   following conditions in order:
   1. If the tier of the result is less than the difficulty tier we fail.
   2. If the result rating is {{< katex >}}6_6{{< /katex >}} we botch.
   3. If the result rating is less than either our chymistry or expertise ratings, we pass.
   4. If the result rating is equal to either our chymistry or expertise rating, we triumph.
   5. If the result rating is greater than both our chymsitry and expertise ratings:
      1. If the degree of the result is less than the tier of our expertise rating, we pass.
      2. If we have reached this step, we fail.

> Note that failure may cause a mishap and botching always does. Mishaps are covered later in their
> own section, [Mishaps]().

# The Difficulty Tier

## Difficulty Tier Definition

As with the general equation for determining the outcome of a test, there is a general equation for
determining the difficulty tier of a test. It is defined thus:

{{< katex display >}}
\delta \bigl(
  \Pi, \thinspace
  f^T, \thinspace
  f^R, \thinspace
  \phi^C, \thinspace
  t, \thinspace
  \lambda, \thinspace
  \rho) =
1 +
\Delta_u(f^T_{\mu}, \thinspace \phi^C, \thinspace t) +
\begin{cases}
  \Delta_r(f^T_{\mu}, \thinspace \lambda) &\text{if } \Pi \equiv \text{Research} \\
  \Delta_p(f^R, f^T, \thinspace \rho, \thinspace \phi^f) &\text{if } \Pi \equiv \text{Preparation} \\
\end{cases}
{{< /katex >}}

Before we go any further, let us define the terms used in this equation.

Remember that {{< katex >}}\delta{{< /katex >}} represents the difficulty tier. The terms inside the
parentheses are the inputs to the equation. They are, in the order they are listed:

{{< katex >}}\Pi{{< /katex >}}
: The set of purpose of the test, either research or preparation.

{{< katex >}}f^T{{< /katex >}}
: The test formula.

{{< katex >}}f^R{{< /katex >}}
: The reference formula. This value is null when the purpose of the test is research. When the
  purpose of the test is preparation, this value is the formula as explicated in the reference
  materials or rated as expertise. When the test formula differs from the reference formula, the
  difficulty of the test increases.

{{< katex >}}\phi^C{{< /katex >}}
: Our rating in chymistry. The higher our rating, the higher the preparation difficulty we can
  handle as a matter of course.

{{< katex >}}t{{< /katex >}}
: The number of steps of time reduction we chose to take. When we want to research or prepare a
  formula more quickly, the difficulty of the test increases alongside the dangers of mishaps if we
  fail.

{{< katex >}}\lambda{{< /katex >}}
: Whether or not we have access to an appropriate laboratory for our research. Without reliable
  access to a laboratory, the difficulty of the test increases alongside the dangers of mishaps if
  we fail.

{{< katex >}}\rho{{< /katex >}}
: Whether or not we are using reference materials during our preparation. To prepare a formula, we
  _must_ use reference materials or have a rating in the reference formula. If we are preparing a
  formula we are rated in _and_ using reference materials, the difficulty is reduced, perhaps
  obviating the need for a test at all.

Next, we must examine the expression that defines the difficulty tier itself:

{{< katex display >}}
1 +
\Delta_u(f^T_{\mu}, \thinspace \phi^C, \thinspace t) +
\begin{cases}
  \Delta_r(f^T_{\mu}, \thinspace \lambda) &\text{if } \Pi \equiv \text{Research} \\
  \Delta_p(f^R, f^T, \thinspace \rho, \thinspace \phi^f) &\text{if } \Pi \equiv \text{Preparation} \\
\end{cases}
{{< /katex >}}

We read this as "1 plus the universal modifier plus either the research modifier or the preparation modifier, depending on the purpose of the test." In other words, the difficulty tier of a test always starts at 1 and is modified depending on the context and purpose of the test.

We will now examine each of these modifiers in detail.

### Universal Modifier

The universal modifier ({{< katex >}}\Delta_u{{< /katex >}}) applies to every test, regardless of purpose. It is defined thus:

{{< katex display >}}
\Delta_u(
  f^T_\mu, \thinspace
  \phi^C, \thinspace
  t
) = \sum_{n=0}^{t}n + \bigl(
  \thinspace f^T_\mu \gt \phi^C_T \to f^T_\mu - \phi^C_T \thinspace
\bigr)
{{< /katex >}}

Here we see the inputs for the universal modifier are the magnitude of the test formula ({{< katex >}}f^T_\mu{{< /katex >}}), our rating in chymistry ({{< katex >}}\phi^C{{< /katex >}}), and the number of steps of time reduction we chose to take.

Let us explicate each of the addends that define the universal modifier in turn:

{{< katex display >}}\sum_{n=0}^{t}n{{< /katex >}}
: We read this notation as "the sum of {{< katex >}}n{{< /katex >}}, from 0 to the number of steps of time reduction we chose to take." It is a compact shorthand and expands like this:

  {{< katex display >}}
  \sum_{n=0}^{t}n = 0 + 1 + 2 + ... + n_t
  {{< /katex >}}

  This becomes clearer with a few examples.

  {{< details "**Example: 0 Steps of Time Reduction**" >}}
  {{< katex display >}}
  t := 0 \qquad \sum_{n=0}^{t}n = ... \qquad \sum_{n=0}^{0}n = 0
  {{< /katex >}}

  In this example, we are have chosen not to reduce the time it takes to prepare or research a formula by any steps (i.e. {{< katex >}}t := 0{{< /katex >}}). The sum of steps from 0 to 0 is 0.
  {{< /details >}}

  {{< details "**Example: 0 Steps of Time Reduction**" >}}
  {{< katex display>}}
  t := 3 \quad \sum_{n=0}^{t}n = ... \quad \sum_{n=0}^{3}n = 1 + 2 + 3 \quad \sum_{n=0}^{t}n = 6
  {{< /katex >}}

  In this example, we have chosen to reduce the time it takes to prepare or research a formula by 3 steps (i.e. {{< katex >}}t := 3{{< /katex >}}). We see that it sums each iteration of the steps together, equalling 6.
  {{< /details >}}

{{< katex display >}}
\bigl( \thinspace f^T_\mu \gt \phi^C_T \to f^T_\mu - \phi^C_T \thinspace \bigr)
{{< /katex >}}
: We read this notation as "if the magnitude of the test formula is greater than the tier of our rating in chymistry, then this value is equal to the magnitude of the test formula minus the tier of our rating in chymistry."

  > This type of notation, where a conditional expression on the left is separated from another
  > expression on the right by a {{< katex >}}\to{{< /katex>}}, is called an inference
  > statement because we _infer_ that the value is defined if and only if the conditional expression
  > is true. Otherwise, the value is zero (or empty, if a set).

  In short, the tier of our rating in chymistry is the upper limit of the magnitude of formulae we can research or prepare without extra difficulty.

  Let us inspect this truth with a few examples:

  {{< details "**Example: Magnitude 2, Chymistry {{< katex >}}3_3{{< /katex >}}**" >}}
  {{< katex display >}}
  \begin{aligned}
  f^T_\mu &:= 2 \\
  \phi^C &:= 3_3 \\
  \bigl( \thinspace f^T_\mu \gt \phi^C_T &\to f^T_\mu - \phi^C_T \thinspace \bigr) \\
  \bigl( \thinspace 2 \gt 3 &\to 2 - 3 \thinspace \bigr) \\
  &\enspace 0
  \end{aligned}
  {{< /katex >}}

  In this example, the magnitude (2) is not greater than the tier of our rating in chymistry (3), so the value is zero.
  {{< /details >}}

  {{< details "**Example: Magnitude 5, Chymistry {{< katex >}}3_3{{< /katex >}}**" >}}
  {{< katex display >}}
  \begin{aligned}
  f^T_\mu &:= 5 \\
  \phi^C &:= 3_3 \\
  \bigl( \thinspace f^T_\mu \gt \phi^C_T &\to f^T_\mu - \phi^C_T \thinspace \bigr) \\
  \bigl( \thinspace 5 \gt 3 &\to 5 - 3 \thinspace \bigr) \\
  &\enspace 2
  \end{aligned}
  {{< /katex >}}

  In this example, the magnitude (5) is greater than the tier of our rating in chymistry (3), so we subtract the tier of our rating in chymistry from the magnitude and find the value is 2.
  {{< /details >}}
{ .dt-30 }

To summarize the terms, the difficulty of any test increases with every step of time reduction we chose to take and for every point of magnitude the test formula exceeds the tier of our rating in chymistry.

Let us examine one final example, bringing it all together:

{{< details "**Example: Magnitude 3, Chymistry {{< katex >}}2_4{{< /katex >}}, 2 Steps of Time Reduction**" >}}
{{< katex display >}}
\begin{aligned}
\Delta_u(f^T_\mu, \thinspace \phi^C, \thinspace t) &=
\sum_{n=0}^{t}n +
\bigl(\thinspace f^T_\mu \gt \phi^C_T \to f^T_\mu - \phi^C_T \thinspace \bigr)
\\
\Delta_u(3, \thinspace 2_4, \thinspace 2) &=
\sum_{n=0}^{2}n +
\bigl(\thinspace 3 \gt 2 \to 3 - 2 \thinspace \bigr)
\\
&= 1 + 2 + \bigl( 1 \bigr)
\\
&= 4
\end{aligned}
{{< /katex >}}

In this example, we see that taking 2 steps of time reduction increases the universal difficulty modifier by 3 (1 + 2 = 3) and, because the magnitude of the test formula (3) exceeds the tier of our rating in chymistry (2), the modifier further increases by 1 (3 - 2 = 1).

The total for this modifer is thereby 4.

{{< /details >}}

### Research Modifier

The research modifier ({{< katex >}}\Delta_r{{< /katex >}}) applies only to tests where the purpose is researching a new formula. It is defined thus:

{{< katex display >}}
\Delta_r(f^T_{\mu}, \thinspace \lambda) = \lnot \lambda \to f^T_{\mu}
{{< /katex >}}

Here we see the inputs for the research modifier are the magnitude of the test formula and whether
or not we have access to an appropriate laboratory for our research. The definition for this
modifier is comparatively simple: if we have access to an appropriate laboratory, the modifier is 0;
if we do not, the modifier is equal to the magnitude of the test formula.

The higher the magnitude of a formula, the more complex it is to manifest its effect(s).
Laboratories provide us with measures of safety and convenience. We should only conduct our research
without a laboratory when absolutely necessary.

### Preparation Modifier

The preparation modifier ({{< katex >}}\Delta_p{{< /katex >}}) applies only to tests where the purpose is preparing a formula. It is defined thus:

{{< katex display >}}
\Delta_p(
  f^R, \thinspace
  f^T, \thinspace
  \rho, \thinspace
  \phi^f
) =
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
        \hphantom{^-} 6 & \lnot{\rho} &\thickspace\land &\lnot{\phi^f} \\
        \hphantom{^-} 0 & \lnot{\rho} &\thickspace\land &\hphantom{\lnot}\phi^f \\
        ^-\phi^f_T & \hphantom{\lnot}\rho &\thickspace\land &\hphantom{\lnot}\phi^f \\
      \end{cases}
  \end{aligned}
\end{pmatrix}
\centerdot
\begin{cases}
  1 &\text{if } f^R_{\pi} \equiv f^T_{\pi} \\
  2 &\text{if } f^R_{\pi} \ne f^T_{\pi} \\
\end{cases}
{{< /katex >}}

Here we see the inputs for the preparation modifier are the reference formula
({{< katex>}}f^R{{< /katex >}}), the test formula formula ({{< katex>}}f^T{{< /katex >}}), whether
or not we are using reference materials during our preparation formula
({{< katex>}}\rho{{< /katex >}}), and our rating in the formula formula
({{< katex>}}\phi^f{{< /katex >}}), if any.

Let us examine the equation itself to explicate each term.

#### Summand Expressions

This first complex term is the sum of several expressions, called the summands. We will explicate each in term, but it may first be useful to know that while it is typically written in multiple lines for compactness, like this:

{{< katex display >}}
\begin{pmatrix}
  \begin{aligned}
      &\bigl(\begin{vmatrix}
        \thinspace f^R_{\iota} \setminus f^T_{\iota} \thinspace
      \end{vmatrix}\bigr)
      \\
      +
      &\bigl(
        \thinspace f^R_{\mu} \ne f^T_{\mu} \to \vert f^R_{\mu} - f^T_{\mu} \vert \thinspace
      \bigr)
      \\
      +
      &\begin{cases}
        \hphantom{^-} 6 & \lnot{\rho} &\thickspace\land &\lnot{\phi^f} \\
        \hphantom{^-} 0 & \lnot{\rho} &\thickspace\land &\hphantom{\lnot}\phi^f \\
        ^-\phi^f_T & \hphantom{\lnot}\rho &\thickspace\land &\hphantom{\lnot}\phi^f \\
      \end{cases}
  \end{aligned}
\end{pmatrix}
{{< /katex >}}

It can also be written as a single line, like this:

{{< katex display >}}
\begin{pmatrix}\begin{vmatrix} f^R_{\iota} &\setminus &f^T_{\iota} \end{vmatrix} \end{pmatrix} +
\bigl( \thinspace f^R_{\mu} \ne f^T_{\mu} \to \vert f^R_{\mu} - f^T_{\mu} \vert \thinspace \bigr) +
\begin{cases}
  \hphantom{^-} 6 & \lnot{\rho} &\thickspace\land &\lnot{\phi^f} \\
  \hphantom{^-} 0 & \lnot{\rho} &\thickspace\land &\hphantom{\lnot}\phi^f \\
  ^-\phi^f_T & \hphantom{\lnot}\rho &\thickspace\land &\hphantom{\lnot}\phi^f \\
\end{cases}
{{< /katex >}}

Now, let us explicate each summand:

{{< katex display >}}
\begin{vmatrix} f^R_{\iota} &\setminus &f^T_{\iota} \end{vmatrix}
{{< /katex >}}
: We read this expression as "the cardinality of the relative complement of the set of the test formula's ingredients in the
  reference formula."

  We find the relative complement of the set of test formula's ingredients in the reference formula to be all of the ingredients in the reference formula that are _not_ in the test formula.

  We find the cardinality of the resulting set by counting the members in it.

  In short, this means that for every ingredient listed in the reference
  formula not used in the test, the modifier increases by 1. If we are not substituting any
  ingredients when preparing our formula, this expression evaluates to 0.

  Consider these examples:

  {{< details "**Example: Identical Formulas**" >}}
  {{< katex display>}}
  \footnotesize
  \begin{vmatrix} f^R_{\iota} &\setminus & f^T_{\iota} \end{vmatrix}
  \\ \thinspace \\
  \scriptsize \begin{vmatrix}
  \begin{Bmatrix}
    \text{Activated Charcoal,} \\
    \text{Child's Drawing,} \\
    \text{Galena} \\
  \end{Bmatrix}
  &\setminus
  &\begin{Bmatrix}
    \text{Activated Charcoal,} \\
    \text{Child's Drawing,} \\
    \text{Galena} \\
  \end{Bmatrix}
  \end{vmatrix}
  \\ \thinspace \\
  \scriptsize \begin{vmatrix}
  \scriptsize \begin{Bmatrix}
    \thinspace & \thinspace & \thinspace
  \end{Bmatrix}
  \end{vmatrix}
  \\ \thinspace \\
  0
  {{< /katex >}}

  Here, we see that the set of ingredients in the reference formula is identical to the set of ingredients in the test formula.

  The relative complement of the ingredients for the test formula in the reference formula is an empty set--there are no ingredients in the reference formula that are not also in the test formula.

  Remember that the cardinality of a set is the count of members in the set. In this case, there are no members in the relative complement set, so the cardinality is 0.

  The term then increases the modifier by 0 points.
  {{< /details >}}

  {{< details "**Example: 2 Substitutions**" >}}
  {{< katex display>}}
  \footnotesize
  \begin{vmatrix} f^R_{\iota} &\setminus & f^T_{\iota} \end{vmatrix}
  \\ \thinspace \\
  \scriptsize \begin{vmatrix}
  \begin{Bmatrix}
    \text{Activated Charcoal,} \\
    \text{Child's Drawing,} \\
    \text{Galena} \\
  \end{Bmatrix}
  &\setminus
  &\begin{Bmatrix}
    \text{Child's Drawing,} \\
    \text{Gascon Saliva,} \\
    \text{Lemon} \\
  \end{Bmatrix}
  \end{vmatrix}
  \\ \thinspace \\
  \scriptsize \begin{vmatrix}
  \scriptsize \begin{Bmatrix}
    \text{Activated Charcoal,} \\
    \text{Child's Drawing,}
  \end{Bmatrix}
  \end{vmatrix}
  \\ \thinspace \\
  2
  {{< /katex >}}

  Here, we see that the set of ingredients in the reference formula differs from the set of ingredients in the test formula.

  The relative complement of the ingredients for the test formula in the reference formula is made up of the ingredients activated charcoal and galena. Because there are two ingredients in the reference formula not included in the test formula, the cardinality is 2.

  This term then increases the modifier by 2 points.
  {{< /details >}}

  {{< details "**Example: Additional Ingredients**" >}}
  {{< katex display>}}
  \footnotesize
  \begin{vmatrix} f^R_{\iota} &\setminus & f^T_{\iota} \end{vmatrix}
  \\ \thinspace \\
  \scriptsize \begin{vmatrix}
  \begin{Bmatrix}
    \text{Activated Charcoal,} \\
    \text{Child's Drawing,} \\
    \text{Galena} \\
  \end{Bmatrix}
  &\setminus
  &\begin{Bmatrix}
    \text{Activated Charcoal,} \\
    \text{Child's Drawing,} \\
    \text{Galena} \\
    \text{Diamond Dust} \\
  \end{Bmatrix}
  \end{vmatrix}
  \\ \thinspace \\
  \scriptsize \begin{vmatrix}
  \scriptsize \begin{Bmatrix}
    \thinspace & \thinspace & \thinspace
  \end{Bmatrix}
  \end{vmatrix}
  \\ \thinspace \\
  0
  {{< /katex >}}

  Here, we see that the set of ingredients in the reference formula differs from the set of ingredients in the test formula.

  However, the relative complement of the ingredients for test formula in the reference formula is an empty set--while the test formula has ingredients not included in the reference formula, there are no ingredients in the reference formula that are not included in the test formula. Because the relative complement is an empty set, the cardinality is 0.

  This term then increases the modifier by 0 points.
  {{< /details >}}

{{< katex display >}}
f^R_{\mu} \ne f^T_{\mu} \to \vert f^R_{\mu} - f^T_{\mu} \vert
{{< /katex>}}
: We read this expression as "if the magnitude of the reference formula is not equal to the magnitude of the test formula, infer the value to be the absolute value of the magnitude of the reference formula minus the magnitude of the test formula."

{{< katex display >}}
\begin{cases}
    \hphantom{^-} 6 & \lnot{\rho} &\thickspace\land &\lnot{\phi^f} \\
    \hphantom{^-} 0 & \lnot{\rho} &\thickspace\land &\hphantom{\lnot}\phi^f \\
    ^-\phi^f_T & \hphantom{\lnot}\rho &\thickspace\land &\hphantom{\lnot}\phi^f \\
  \end{cases}
{{< /katex >}}
: We read this expression as "if we are not using reference materials, the value is 1; else if we are using reference materials and have a rating in the formula, the value is the negative of our tier in the rated formula; otherwise, the value is zero."

  NB: This might need modifying. Considering an alternative where we say instead that if we are not using reference materials and do not have a rating in the formula, the value is six; else if we are using reference materials and do not have a rating in the formula, the value is 0; otherwise, the value is the negative of our tier in the rated formula. i.e.

  {{< katex display >}}
  \begin{cases}
    \hphantom{^-} 6 & \lnot{\rho} &\thickspace\land &\lnot{\phi^f} \\
    \hphantom{^-} 0 & \lnot{\rho} &\thickspace\land &\hphantom{\lnot}\phi^f \\
    ^-\phi^f_T & \hphantom{\lnot}\rho &\thickspace\land &\hphantom{\lnot}\phi^f \\
  \end{cases}
  {{< /katex >}}
{ .dt-25 }