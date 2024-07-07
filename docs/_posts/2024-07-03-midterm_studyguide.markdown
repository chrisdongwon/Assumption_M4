---
layout: post
title:  "Midterm Exam Study Guide"
date:   2024-07-02 00:00:00 +0000
categories: announcement
katex: True
---

Answer the following as a review for your upcoming midterm exam. Make sure to show as much work as possible in order to maximize your points on the exam - any unsupported answers will warrant partial credit.

1. Let $$S$$ be a nonempty set and let $$U = \mathcal{P}(S)$$, the powerset of $$S$$, and let $$A, B \in \mathcal{P}(S)$$. Recall that the powerset of $$S$$ is a set of all subsets of $$S$$, hence $$A$$ and $$B$$ are simply subsets of $$S$$. Using the set-builder notation, suggest a definition for the following operations:

    * The complement of $$A$$: $$A^{\prime}$$. 
    * The union of $$A$$ and $$B$$: $$A \cup B$$.
    * The intersection of $$A$$ and $$B$$: $$A \cap B$$.

    Solution: The following are the definition of the set operations.

    * $$A^{\prime} = \{x \in U : x \not \in A\}$$
    * $$A \cup B = \{x \in U: x \in A \text{ or } x \in B\}$$
    * $$A \cap B = \{x \in U: x \in A \text{ and } x \in B\}$$

1. Let $$U = \mathbb{Z}$$, $$A = \{x \in \mathbb{Z} : 0 \leq x \leq 100\}$$, $$E = \{x \in \mathbb{Z} : x \text { is divisible by } 2\}$$, and $$O = \{x \in \mathbb{Z} : x \text { is not divisible by } 2\}$$.

    * Are $$E$$ and $$O$$ disjoint sets? Why or why not?
    * What is $$A \cap E$$?
    * What is $$A \cup O$$?
    * What is $$(A \cap E)^{\prime}$$?
    * What is the cardinality of $$A \cap E$$?
    * Is $$A \cup O$$ a proper subset of $$A$$? Why or why not?
    * Classify $$U,A,E,O$$ as either finite or infinite.

    Solution: As you may have noticed, $$E$$ indicates the set of even integers and $$O$$ indicates the set of odd integers.
    * Notice that an integer is either an even or an odd but not both nor neither at the same time. Hence, $$A \cap B = \{\}$$ and this is precisely the definition of disjoint sets - they have nothing in common.
    * $$A$$ is the set of integers from $$0$$ to $$100$$, inclusive. Hence, $$A \cap E = \{x \in A : x \text{ is divisible by } 2\} = \{0,2,4,...,98,100\}$$.
    * Notice that integers from $$0$$ to $$100$$, inclusive, will still include the odd integers within that range. Hence, $$A \cup O = \{x \in U : 0 \leq x \leq 100 \text{ or } x \text{ is not divisible by } 2\} = \{...,-5,-3,-1,0,1,2,3,...,98,99,100,101,103,105,...\}$$.
    * Let's simply exclude the elements from the first problem: $$(A \cap E)^{\prime} = \{...,-3,-2,-1,1,3,5,7,...,97,99,101,102,103,...\}$$.
    * Cardinality refer to the countable number of elements in a set. With $$51$$ even numbers from $$0$$ to $$100$$, it follows that $$n(A \cap E) = 51$$. 
    * Notice that there are more elements in $$A \cup O$$ than $$A$$. Thus, $$A \cup O$$ is certainly not a subset of $$A$$ and definitely not a _proper_ subset of $$A$$. For sets $$A$$ and $$B$$, we say that $$A$$ is a proper subset of $$B$$ if $$A \subset B$$ and $$A \not = B$$, meaning there exists $$x \in B$$ such that $$x \not in A$$. However, this implies that $$A$$ is a proper subset of $$A \cup O$$. 

1. What is the definition of **set equality**? What is the definition of **set equivalence**? Are equal sets also equivalent? Are equivalent sets also equal? Explain.

    Solution: We say that the sets $$A$$ and $$B$$ are equal if $$A \subseteq B$$ and $$B \subseteq A$$, i.e. $$A$$ is contained in $$B$$ and $$B$$ is contained in $$A$$. A similar analogy would be: for any numbers $$x$$ and $$y$$, $$x = y$$ if and only if $$x \leq y$$ and $$x \geq y$$. On the other hand, we say that $$A$$ and $$B$$ are equivalent if their cardinalities are the same, i.e. $$n(A) = n(B)$$. More formally, we say that two sets are equivalent if there exists a bijective function from $$A$$ to $$B$$. For more information on this, take a look into the [wikipedia page](https://en.wikipedia.org/wiki/Bijection) on this topic.

1. What is the difference between a **Venn diagram** and an **Euler diagram**? Compare and contrast.

    Solution: Venn diagrams are actually Euler diagrams, but Euler diagrams are not Venn diagrams. What do I mean by this? Venn diagrams will display all possible configurations in terms of the set intersections, while Euler diagrams will make sure to visually distinguish that disjoint sets are indeed disjoint by drawing them separately. Venn diagrams will still display the intersection even if the sets are disjoint. For more information, please refer to the [wikipedia page](https://en.wikipedia.org/wiki/Euler_diagram#Relation_between_Euler_and_Venn_diagrams). 

1. Write the general formula for the cardinality of a union of two sets, i.e. $$n(A \cup B)$$. What is the formula when $$A$$ and $$B$$ are disjoint? Hint: inclusion-exclusion principle.

1. True or false? $$ab = GCD(a,b) + LCM(a,b)$$. If false, what is the correct statement?

1. Describe the steps to the Euclidean Algorithm, and find $$GCD(194, 268)$$ using the algorithm. 