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

    - Complement: $$A^{\prime} = \{x \in U : x \not \in A\}$$. In other words, complement refers to the negation - elements that are not in $$A$$ but still in $$U$$. The set complement is also denoted $$A^{C}$$, which is the notation that I prefer to use. Also, if the notion of $$U$$ is not explicit, another notation for the set complement is, say, $$A \setminus B = \{x \in A: x \not in B\}$$ (sometimes, $$A - B$$ is also used). Just like how we have subtraction of numbers and a negative of numbers, set complement will depend on the context as in is it an operation on a single set with respect to the universe set $$U$$ or an operation on two sets. 
    - Intersection: $$A \cap B = \{x \in U : x \in A \text{ and } x \in B\}$$. One way to remember the symbol for intersection is: $$\cap$$ kind of looks like $$n$$, and intersection is about elements in both $$A$$ and $$B$$ - so $$n$$ and "and" should go together. If $$A$$ and $$B$$ have no elements in common, then it follows that $$A \cap B = \emptyset$$, and when this happens, we say that $$A$$ and $$B$$ are **disjoint sets**. We also say that $$A$$ and $$B$$ are "mutually exclusive" to denote disjoint sets. 
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

Let us briefly think of the _ordered pairs_, colloquially known as $$(x,y)$$ on the two dimensional plane, known as the Cartesian coordinates. As the name suggests, the ordered pairs are two numbers in which the ordering does matter: first number is the value on the $$x$$ axis and the second number is the value on the $$y$$ axis. Here is an abstract way to think of ordered pairs as sets: $$(x,y) = \{\{x,y\}, \{x\}\}$$. $$\{x,y\}$$ kind of makes sense as it looks awfully like the original ordered pair, but what about $$\{x\}$$? If $$x \not = y$$, then it makes sense to say that $$\{x,y\}$$ also contains two elements. However, if $$x = y$$, then $$\{x, y\} = \{x, x\} = \{x\}$$.

## Cardinality and Set Equivalence

**Cardinality** is just a fancy name for the number of elements in a set. Cardinality of set $$A$$ is denoted as either $$n(A)$$ or $$\lvert A \rvert$$, where I prefer the latter notation. Does this remind you of the absolute value of a number?

For example, it is clear that $$\lvert \emptyset \rvert = 0$$ and $$\lvert \{2,4,6\} \rvert = 3$$, and similarly, we see that $$\lvert \{1,3,5\} \rvert = 3 $$. While $$\{2,4,6\} \not = \{1,3,5\}$$, we say that two sets are **equivalent** if they have the same cardinality. Thus, the aforementioned sets are equivalent as $$\lvert \{2,4,6} \rvert = \lvert \{1,3,5\} \rvert$$.

Things get extremely mind-bending when we start to consider sets with infinitely many elements. Here is something to consider: $$\lvert \mathbb{Z} \rvert = \lvert \{2k : k \in \mathbb{Z}\}\rvert$$ because the latter set, the set of multiples of 2, is simply the set of integers but all elements have been multiplied by $$2$$, thus they actually should have the same number of elements. In other words, there are _just as many_ even integers as the set of integers themselves, although the set of integers have gaps between them!!! This brings us to the formal definition of set equality: we actually say that two sets are equivalent if and only if there exists a bijective mapping between those two sets, meaning all elements can be paired in a general manner without skipping any elements in either of the sets. For more information on this including the definition of bijection, I refer you to the [wikipedia page](https://en.wikipedia.org/wiki/Bijection) as this information is slightly out of the scope at this level in mathematics. Funnily enough, one can have [a similar argument](https://www.youtube.com/watch?v=kf2Xwr22oGM) as to why the cardinality of the real numbers between $$0$$ and $$1$$ is the same as the cardinality of all real numbers, which is also very counterintuitive.

## Application: Inclusion-Exclusion Principle

There's a very useful formula known as the _inclusion-exclusion principle_ which allows us to have a consistent way of counting the number of elements in a set union. Let $$A$$ and $$B$$ be sets. By the inclusion-exclusion principle, we can say that $$\lvert A \cup B \rvert = \lvert A \rvert + \lvert B \rvert - \lvert A \cap B \rvert$$. If we want to know the cardinality of three sets, then the known identity is $$\lvert A \cup B \cup C \rvert = \lvert A \rvert + \lvert B \rvert + \lvert C \rvert - \lvert A \cap B \rvert - \lvert B \cap C \rvert - \lvert A \cap C \rvert + - \lvert A \cap B \cap C \rvert$$, and of course, if you have the patience for it, we can even go further and have a formula for _any_ finite number of sets. For a proof and an explanation on this, I refer you to an [article](https://people.maths.bris.ac.uk/~mb13434/incl_excl_n.pdf). 

## Countability and Infinity

## Optional: Russell's Paradox

## Optional: Naive Set Theory vs. Axiomatic Set Theory