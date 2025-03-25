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
5.
    - The set-builder notation for the odd integers is $$\{2x + 1 : x \in \mathbb{Z}\}$$.
    - Notice that this set has **exactly** the same number of elements as $$\mathbb{Z}$$ - we have neither included nor excluded extra elements in the set of odd integers - we simply took each integer, and applied the formula $$2x+1$$.


## Section 2.2: Propositional Logic

## Section 2.3: Truth Tables

