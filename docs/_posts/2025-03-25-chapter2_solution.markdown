---
layout: post
title:  "Chapter 2 Solution Guide"
date:   2025-03-25 00:00:00 +0000
categories: lecture notes
katex: True
---

## Section 2.1: Naive Set Theory

1. Recall that **even integers are multiples of 2**, and the numbers that are **not even are called odd integers**. In roster notation, the only possible answer here is $$\{-9, -7, -5, -3, -1, 1, 3, 5, 7, 9\}$$

    With set-builder notation, we have multiple possibilities:
    - $$\{x \in \mathbb{Z} : -10 < x < 10 \text{ and } x \text{ is odd}\}$$
    - Let $$2\mathbb{Z} + 1$$ be the set of odd integers, similar to how $$2\mathbb{Z}$$ represents the multiples of 2. Then, a possible expression for the set is $$\{x \in 2\mathbb{Z}+1 : -10 < x < 10\}$$.
    - Notice that all odds are of the form $$2x + 1$$ for all $$x \in \mathbb{Z}$$. With $$-9 = 2(-5) + 1$$ and $$9 = 2(4)+1$$, we can say that the expression here is $$\{2x + 1 : x \in \mathbb{Z} \text{ and } -5 \leq x \leq 4\}$$
2. The set of all subsets is called a **power set**. For $$S = \{a,b,c\}$$, the powerset of $$S$$ is $$\{\{\}, \{a\}, \{b\}, \{c\}, \{a,b\}, \{b,c\}, \{a,c\},  \{a,b,c\}\}$$. Notice that the empty set is a subset of **any** set. 
3. Both $$(0,1)$$ and $$[0,1]$$ contain all numbers from $$0$$ to $$1$$. However, $$[0,1]$$ also contains $$0$$ and $$1$$, whereas $$(0,1)$$ does not. By the definition of proper subsets, it follows that $$(0,1) \subset [0,1]$$. 
4. Recall that set equality is when both sets have exactly the same elements, and set equivalence is when both sets have the same cardinality (i.e., the number of elements).
    - $$A$$ and $$B$$ are not equal, as you can see that all elements are different, respectively.
    - However, $$A$$ and $$B$$ are equivalent, because they have the same cardinality of 4.

5.  - The set-builder notation for the odd integers is $$\{2x + 1 : x \in \mathbb{Z}\}$$.
    - Notice that this set has **exactly** the same number of elements as $$\mathbb{Z}$$ - we have neither included nor excluded extra elements in the set of odd integers - we simply took each integer, and applied the formula $$2x+1$$.

## Section 2.2: Propositional Logic

1. Remember that I am not asking if the evaluation of these statements are _true_ or _false - I am simply asking if the statements are **propositions**. Refer back to the text for a clarification on what constitutes a proposition.
    - $$2+3 = 5$$ is a proposition, as there is the answer to the statement will be a definite true or false.
    - Without knowing what the value of $$x$$ is, we cannot determine if the numbers on the left and right will equal to each other. Therefore, we cannot say that this is a proposition. For your information, these kind of statements where the statements can be true or false for variable $$x$$ is called a **predicate**, which will be discussed in the actual academic year.
    - 1, by definition, is not a prime and not a composite number. This is a valid proposition, and as a matter of fact, it is evaluated to be a true statement.
2. Conjunctions are true if all the propositions are true. Are all the propositions here true?
3. Disjunctions are true if at least one of the propositions is true. Can you find at least one proposition amongst $$p,q,r$$?
4. Implications are true if the left side and the right side of the arrow are both true, or if the left side of the arrow is false (vacuous truth). $$r$$ states that $$\sqrt{2}$$ is _not_ an integer, and $$p \wedge \neg q$$ states that $$2$$ is even and $$3$$ is _not_ even. What do you conclude?
5.  - Negation: I do **not** eat somtum.
    - Conjunction: I eat somtum **and** my mouth is on fire. 
    - Disjunction: I eat somtum **or** my mouth is on fire.
    - Implication: **If** I eat somtum, **then** my mouth is on fire.

## Section 2.3: Truth Tables

