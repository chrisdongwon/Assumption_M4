---
layout: post
title:  "Naive Set Theory"
date:   2024-07-02 00:00:00 +0000
categories: lecture notes
katex: True
---

When we first started learning mathematics, we generally dealt with specific numbers one at a time, and then we learned Algebra in which we used variables to represent various numbers, and the collection of variables in which they formed a specific description of many numbers in general, such as the integers and the rational numbers to say the least. Such collections are referred to as **sets**, and they can be collections of any objects of mathematical interest, not just numbers. We denote the collection with curly braces, i.e. $$\{...\}$$. A set with no elements is referred to as the empty set, denoted $$\{\}$$ or $$\emptyset$$. 

Then, what kind of _elements_ can we have in a set? Believe it or not, it doesn't always have to be numbers. Of course, a collection of numbers is of general interest in terms of mathematics, but sometimes, it can be even more. As an example, consider the following: $$S = \{\emptyset\}$$. This is a set of sets, where the only member in this set is the empty set. Weird, right? Since this set contains at least one element, it is considered to be not empty, even though the only element in this set is an empty set! To denote a membership in a set, we use the symbol $$\in$$. As a concrete usage, we can say that $$\emptyset \in S$$. Think $$\in$$ as "e" for "element of."

## Set-builder Notation

Informally, or if the number of elements in the set is small enough, you can simply write out the elements in the set manually - and we refer to such listing as the _roster notation_. For example, integers from 0 to 10, inclusive, can be written out like $$\{0,1,2,3,4,5,6,7,8,9,10\}$$. The integers can be written out like $$\{...,-3,-2,-1,0,1,2,3,...\}$$. However, the usage of $$...$$, while intuitive, can be sometimes ambiguous. For example, let's say I have the following set $$\{1,2,...\}$$. One would normally say that this is a set of positive integers. However, the powers of $$2$$ starting with exponent $$0$$ will have the same values: $$2^0 = 1$$ and $$2^1 = 2$$. So, which is it?

For the sake of clarity, the set-builder notation is the preferred method of describing the elements of the set. For example, the integers from 0 to 10, inclusive, can also be written out like the following: $$\{x \in \mathbb{N} : x \leq 10\}$$. Since the natural numbers begin with $$0$$, we just need to specify that all elements of this set are less than or equal to $$10$$. The format for the set builder notation is:

$$\{\text{expression or the membership of the elements } : \text{ condition of such elements}\}$$.

For example, we can have the powers of $$2$$ with natural number exponents like the following: $$\{2^k : k \in \mathbb{N}\}$$. If you know the exact pattern or the restrictions of the set that you are trying to describe, the set-builder notation is rather a shorter and more concise way to denote the set of interest. 

## Operations on Sets

Just like how we can add, subtract, multiply, and divide numbers, we can do analogous activities on sets as well. So, let $$U$$ represent the universe - a set that contains all possible elements that you would like to refer to or describe. Let $$A$$ and $$B$$ represent sets whose elements come from $$U$$. Then, for $$A$$ and $$B$$, we can define the following operations:

    - Complement: $$A^{\prime} = \{x \in U : x \not \in A\}$$. In other words, complement refers to the negation - elements that are not in $$A$$ but still in $$U$$. The set complement is also denoted $$A^{C}$$, which is the notation that I prefer to use. 
    - Intersection: $$A \cap B = \{x \in U : x \in A \text{ and } x \in B\}$$. One way to remember the symbol for intersection is: $$\cap$$ kind of looks like $$n$$, and intersection is about elements in both $$A$$ and $$B$$ - so $$n$$ and "and" should go together. 
    - Union: $$A \cup B = \{x \in U : x \in A \text{ or } x \in B\}$$. The word "or" here is not so restrictive: $$x$$ can be in $$A$$, or in $$B$$, or even in both $$A$$ and $$B$$. This is called _inclusive or_. One way to highlight the usage of inclusive or is the the following phrase: "do you want pizza or burgers?" and your answer might be: "yes." This indicates that you are fine with either pizza, or burger, or if you are quite hungry, then why not both! In contrast, "exclusive or" is more restrictive: if your answer is "pizza" or "burger," then you are most likely saying you would like one or the other. In mathematics (and in computer science), "or" is almost always the inclusive type. Exclusive or is usually denoted "XOR," especially in computer science and engineering.

## Optional: De Morgan's Law

What happens when we mix set complement with set union or set intersection? There's a nice rule that allows to kind of think of set intersection and set union as opposite ideas.

    * $$(A \cup B)^{\prime} = A^{\prime} \cap B^{\prime}$$
    * $$(A \cap B)^{\prime} = A^{\prime} \cup B^{\prime}$$

So, you may hear me say that the complement of the union is the intersection of complements or that the complement of the union is the intersection of the complements. For a proof of this statement, I will refer you to the [wikipedia page](https://en.wikipedia.org/wiki/De_Morgan%27s_laws#Formal_proof). 

## Subsets
Subsets are important aspect of mathematics, as while it is nice to have the universe set $$U$$, we often times talk about more specific elements of $$U$$, namely the subsets of $$U$$. Let $$A$$ be a set.

    * Subset: $$A$$ is a subset of $$U$$, denoted $$A \subseteq U$$ if for all $$x \in A$$, it is the case that $$x \in U$$ as well. So, we have that $$A \subseteq A$$, and by convention, $$\emptyset \subseteq A$$ since nothing is already present in a set of some things, if that makes sense. 
    * Proper Subset: If $$A \subseteq U$$ but $$A \not = U$$, then we say that $$A$$ is a proper subset of $$U$$. This means there exists $$x \in U$$ such that $$x \not \in A$$, but for all $$x \in A$$, it is the case that $$x \in U$$. For example, the set of even integers is a proper subset of the set of integers $$\mathbb{Z}$$ because the odd integers are not present in the set of even integers. As you can clearly and intuitively see, the set of even integers is certainly not __equal__ to the set of all integers, but believe it or not, they are **equivalent**. Allow me to explain in the following section. 

## Set Equality and Set Equivalence

Let $$A$$ and $$B$$ be sets. If it is possible to take a look at the elements of the sets manually, maybe you can try to see if the two sets are equal by pairing the elements from $$A$$ and $$B$$ whenever they are equal, and if all of the elements in both sets can be paired. This brings us to the formal definition of _set equality_:

    * Set equality: We say that $$A = B$$ if and only if $$A \subseteq B$$ and $$B \subseteq A$$. 

With this definition, it is clear to see why $$\{1, 2, 3\} = \{3,2,1\}$$ as all elements in $$\{1,2,3\}$$ also appear in $$\{3,2,1\}$$ and vice versa, so they are subsets of one another. This implies that the ordering of the elements do not matter as long as they are still being represented in the set that you claim are equal. By convention, repeating elements in a set _collapse_ to a single representation. For example, we say that $$\{2,2,2\} = \{2\}$$. What if order does matter, and we do need to keep track of repetitive elements? This idea will be explored in the following section. 

## Example: Ordered Pairs

## Set Equivalence

## Countability and Infinity

## Optional: Russell's Paradox

## Optional: Naive Set Theory vs. Axiomatic Set Theory