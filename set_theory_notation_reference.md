# Set Theory Notation — Quick Reference

A practical reference for reading and writing expressions in elementary
set theory. Mathematical expressions use LaTeX notation and render on
GitHub (and in other Markdown viewers that support MathJax or KaTeX).

> **Notation varies:** Some books use symbols differently. In
> particular, $\subset$, $\subseteq$, and the vertical bar $\mid$ can
> have different conventions. Follow the definitions used by your course
> or textbook.

## 1. Basic set notation

| Symbol | LaTeX | Meaning | Read it as |
|---|---|---|---|
| $x \in A$ | `x \in A` | $x$ is an element of $A$ | x belongs to A |
| $x \notin A$ | `x \notin A` | $x$ is not an element of $A$ | x does not belong to A |
| $\lbrace \, \rbrace$ | `\{\,\}` | Braces delimit a set | the set containing … |
| $\varnothing$ or $\emptyset$ | `\varnothing` or `\emptyset` | Empty set | the empty set |
| $A = B$ | `A = B` | The sets have exactly the same elements | A equals B |
| $A \ne B$ | `A \ne B` | The sets are not equal | A is not equal to B |
| $\lvert A \rvert$ | `\|A\|` | Cardinality: the number of elements of $A$ | the cardinality of A |
| $A \times B$ | `A \times B` | Cartesian product | A cross B |

### Example

```math
A = \{1,2,3\}
```

Then $2 \in A$, while $5 \notin A$. Also, $\lvert A \rvert = 3$.

## 2. Subsets and set equality

| Symbol | LaTeX | Meaning | Read it as |
|---|---|---|---|
| $A \subseteq B$ | `A \subseteq B` | Every element of $A$ is also in $B$ | A is a subset of B |
| $A \subsetneq B$ | `A \subsetneq B` | $A$ is a subset of $B$, but $A \ne B$ | A is a proper subset of B |
| $A \supseteq B$ | `A \supseteq B` | $A$ contains every element of $B$ | A is a superset of B |
| $A \supsetneq B$ | `A \supsetneq B` | $A$ properly contains $B$ | A is a proper superset of B |

**Important:** Some textbooks use $\subset$ for "subset"
(allowing equality); others use it for "proper subset". The unambiguous
symbols are $\subseteq$ and $\subsetneq$.

### Example

Let $A = \lbrace 1,2 \rbrace$ and $B = \lbrace 1,2,3 \rbrace$.

```math
A \subseteq B \qquad \text{and} \qquad A \subsetneq B
```

But $B \not\subseteq A$.

## 3. Operations on sets

| Symbol | LaTeX | Meaning | Read it as |
|---|---|---|---|
| $A \cup B$ | `A \cup B` | Elements in $A$, in $B$, or in both | A union B |
| $A \cap B$ | `A \cap B` | Elements common to both sets | A intersect B |
| $A \setminus B$ | `A \setminus B` | Elements in $A$ that are not in $B$ | A minus B / A without B |
| $A^c$ | `A^c` | Complement of $A$, relative to a specified universal set | complement of A |
| $A \triangle B$ | `A \triangle B` | Symmetric difference: elements in exactly one of the two sets | symmetric difference |
| $\mathcal{P}(A)$ | `\mathcal{P}(A)` | Power set: the set of all subsets of $A$ | power set of A |

### Example

Let $A = \lbrace 1,2,3 \rbrace$ and $B = \lbrace 3,4 \rbrace$.

```math
\begin{aligned}
A \cup B &= \{1,2,3,4\}\\
A \cap B &= \{3\}\\
A \setminus B &= \{1,2\}\\
B \setminus A &= \{4\}\\
A \triangle B &= \{1,2,4\}
\end{aligned}
```

The complement $A^c$ cannot be determined unless the universal set is
specified.

## 4. Set-builder notation

Set-builder notation describes a set by stating a condition its elements
must satisfy.

```math
A = \{x \in \mathbb{N} \mid x < 5\}
```

Read this as:

"A is the set of all $x$ in the natural numbers such that $x$ is less
than 5."

| Symbol | Meaning in this context |
|---|---|
| $\lbrace$ and $\rbrace$ | The beginning and end of the set description |
| $x$ | A variable representing a possible element |
| $\in$ | Belongs to |
| $\mathbb{N}$ | The set of natural numbers |
| $\mid$ or $:$ | Such that |
| $x < 5$ | The condition that the element must satisfy |

The same set can be written using a colon:

```math
A = \{x \in \mathbb{N} : x < 5\}
```

The vertical bar $\mid$ has other meanings in mathematics. Its
meaning depends on context.

## 5. Quantifiers and logical symbols

These symbols are used to state conditions about elements and sets.

| Symbol | LaTeX | Meaning | Read it as |
|---|---|---|---|
| $\forall$ | `\forall` | Universal quantifier | for all / for every |
| $\exists$ | `\exists` | Existential quantifier | there exists |
| $\exists!$ | `\exists!` | There exists exactly one | there exists a unique |
| $\neg$ | `\neg` | Logical negation | not |
| $\land$ | `\land` | Logical conjunction | and |
| $\lor$ | `\lor` | Logical disjunction | or |
| $\Rightarrow$ | `\Rightarrow` | Implication | implies |
| $\Leftrightarrow$ | `\Leftrightarrow` | Logical equivalence | if and only if |
| $\therefore$ | `\therefore` | Conclusion marker | therefore |

### Examples

```math
\forall x \in A,\; x > 0
```

"For every $x$ in $A$, $x$ is greater than zero."

```math
\exists x \in A \text{ such that } x > 10
```

"There exists an element $x$ in $A$ that is greater than 10."

```math
x \in A \Rightarrow x \in B
```

"If $x$ belongs to $A$, then $x$ belongs to $B$."

## 6. Common number sets

| Symbol | Meaning | Typical elements |
|---|---|---|
| $\mathbb{N}$ | Natural numbers | $1, 2, 3, \ldots$ (sometimes including $0$) |
| $\mathbb{Z}$ | Integers | $\ldots, -2, -1, 0, 1, 2, \ldots$ |
| $\mathbb{Q}$ | Rational numbers | Fractions such as $\frac{1}{2}$, $-\frac{3}{4}$ |
| $\mathbb{R}$ | Real numbers | Rational and irrational numbers |
| $\mathbb{C}$ | Complex numbers | Numbers of the form $a + bi$ |

**Convention note:** Whether $0$ belongs to $\mathbb{N}$ depends
on the author. Check the definition in your textbook.

## 7. Other useful notation

| Symbol | LaTeX | Meaning | Read it as |
|---|---|---|---|
| $\lbrace a,b,c \rbrace$ | `\{a,b,c\}` | A set whose elements are $a, b, c$ | the set containing a, b and c |
| $\lbrace x_1, x_2, \ldots, x_n \rbrace$ | `\{x_1,x_2,\ldots,x_n\}` | A finite list of elements forming a set | x one, x two, and so on, up to x n |
| $\ldots$ | `\ldots` | Continuation of a pattern | and so on |
| $\mathbb{N}_0$ | `\mathbb{N}_0` | Often the natural numbers including zero | natural numbers including zero |
| $A \times B$ | `A \times B` | Set of ordered pairs $(a,b)$, with $a \in A$, $b \in B$ | Cartesian product of A and B |
| $\lbrace (a,b) \mid \cdots \rbrace$ | `\{(a,b)\mid \cdots\}` | A set described by a condition on ordered pairs | the set of pairs such that … |

## 8. A few expressions to practise reading

1. $\lbrace x \in \mathbb{Z} \mid -2 \le x \le 2 \rbrace$

   The set of integers $x$ such that $x$ is between $-2$ and $2$,
   inclusive.

   Result: $\lbrace -2, -1, 0, 1, 2 \rbrace$.

2. $A \cap B = \varnothing$

   The intersection of $A$ and $B$ is empty. The sets have no elements
   in common.

3. $A \subseteq B$

   Every element of $A$ is also an element of $B$.

4. $\forall x \in A,\; x \in B$

   Every element of $A$ belongs to $B$. This is another way to express
   $A \subseteq B$.

5. $\mathcal{P}(A)$

   The set of all subsets of $A$. For example, if $A = \lbrace 1,2 \rbrace$, then

   ```math
   \mathcal{P}(A) = \{\varnothing, \{1\}, \{2\}, \{1,2\}\}.
   ```

---

## A useful reading habit

When you meet an unfamiliar expression:

1. Identify the symbols.
2. Read the expression from left to right in ordinary language.
3. Identify the condition being imposed.
4. Try a small example with concrete elements.

Do not try to memorize every expression at once. Keep this reference
nearby and return to it as new notation appears.
